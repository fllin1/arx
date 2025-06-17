<template>
  <div class="cv-page-container">
    <!-- Barre d'actions -->
    <div class="action-bar">
      <h1 class="page-title">Mon CV</h1>
      <div class="actions">
        <button
          @click="downloadPDF"
          class="download-btn"
          :disabled="isDownloading"
        >
          <span v-if="!isDownloading">📄 Télécharger PDF</span>
          <span v-else>⏳ Génération...</span>
        </button>
        <button @click="print" class="print-btn">🖨️ Imprimer</button>
      </div>
    </div>

    <!-- CV Component avec isolation complète des styles -->
    <div ref="cvContent" class="cv-wrapper">
      <div class="cv-isolator">
        <CVFlorentLin />
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from "vue";
import html2pdf from "html2pdf.js";
import CVFlorentLin from "../components/CVFlorentLin.vue";

// Refs
const cvContent = ref<HTMLElement>();
const isDownloading = ref(false);

// Télécharger le CV en PDF
const downloadPDF = async () => {
  if (!cvContent.value || isDownloading.value) return;

  isDownloading.value = true;

  try {
    const options = {
      margin: 0,
      filename: "CV_Florent_Lin.pdf",
      image: { type: "jpeg", quality: 0.98 },
      html2canvas: {
        scale: 2,
        useCORS: true,
        letterRendering: true,
      },
      jsPDF: {
        unit: "mm",
        format: "a4",
        orientation: "portrait",
      },
      pagebreak: { mode: ["avoid-all", "css", "legacy"] },
    };

    await html2pdf().set(options).from(cvContent.value).save();
  } catch (error) {
    console.error("Erreur lors de la génération du PDF:", error);
    alert("Une erreur est survenue lors de la génération du PDF");
  } finally {
    isDownloading.value = false;
  }
};

// Imprimer le CV
const print = () => {
  window.print();
};
</script>

<style scoped>
.cv-page-container {
  min-height: 100vh;
  background-color: #f5f5f5;
  padding: 20px 20px 40px;
}

.action-bar {
  max-width: 850px;
  margin: 0 auto 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: white;
  padding: 20px;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.page-title {
  margin: 0;
  font-size: 24px;
  color: #333;
}

.actions {
  display: flex;
  gap: 10px;
}

.download-btn,
.print-btn {
  padding: 10px 20px;
  border: none;
  border-radius: 6px;
  font-size: 16px;
  cursor: pointer;
  transition: all 0.3s ease;
  font-weight: 500;
}

.download-btn {
  background-color: #2563eb;
  color: white;
}

.download-btn:hover:not(:disabled) {
  background-color: #1d4ed8;
  transform: translateY(-1px);
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.download-btn:disabled {
  opacity: 0.6;
  cursor: not-allowed;
}

.print-btn {
  background-color: #10b981;
  color: white;
}

.print-btn:hover {
  background-color: #059669;
  transform: translateY(-1px);
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.cv-wrapper {
  max-width: 850px;
  margin: 0 auto;
}

/* Isolation complète des styles pour le CV */
.cv-isolator {
  /* Reset de tous les styles hérités */
  all: initial;

  /* Affichage en bloc pour contenir le CV */
  display: block !important;

  /* Alignement par défaut (pas de centrage forcé) */
  text-align: initial !important;

  /* Réinitialisation des propriétés de positionnement */
  position: static !important;

  /* Largeur et hauteur naturelles */
  width: auto !important;
  height: auto !important;

  /* Marges et padding reset */
  margin: 0 !important;
  padding: 0 !important;

  /* Couleurs par défaut */
  color: initial !important;
  background: initial !important;

  /* Police par défaut du système */
  font-family: initial !important;
  font-size: initial !important;
  font-weight: initial !important;
  line-height: initial !important;

  /* Bordures */
  border: initial !important;
  border-radius: initial !important;

  /* Ombres */
  box-shadow: initial !important;
  text-shadow: initial !important;

  /* Transformations */
  transform: initial !important;

  /* Débordement */
  overflow: initial !important;

  /* Z-index */
  z-index: initial !important;
}

/* Assurer que tous les éléments enfants héritent de la réinitialisation */
.cv-isolator * {
  /* Ne pas forcer de styles sur les enfants, laisser le CV gérer ses propres styles */
}

/* Responsive */
@media (max-width: 768px) {
  .action-bar {
    flex-direction: column;
    gap: 15px;
    text-align: center;
  }

  .actions {
    width: 100%;
    justify-content: center;
  }

  .download-btn,
  .print-btn {
    font-size: 14px;
    padding: 8px 16px;
  }
}

/* Print styles */
@media print {
  .action-bar {
    display: none;
  }

  .cv-page-container {
    background: white;
    padding: 0;
  }

  .cv-wrapper {
    max-width: none;
    margin: 0;
  }
}
</style>
