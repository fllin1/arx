<template>
  <div class="cv-container">
    <div class="cv-page">
      <!-- Header -->
      <header class="cv-header">
        <h1 class="name">FLORENT LIN</h1>
        <div class="contact-info">
          <div class="contact-row">
            <span class="contact-item">
              <i class="fa fa-github"></i> github.com/fllin1
            </span>
            <span class="contact-item">
              <i class="fa fa-linkedin"></i> linkedin.com/in/florentlin/
            </span>
            <span class="contact-item">
              <i class="fa fa-envelope"></i> 1florentlin@gmail.com
            </span>
          </div>
          <div class="contact-row">
            <span class="contact-item">
              <i class="fa fa-map-marker"></i> 12 Rue Lieutenant Albert Vasseur,
              28300 Champhol, France
            </span>
            <span class="contact-item">
              <i class="fa fa-phone"></i> 07 81 63 66 63
            </span>
          </div>
        </div>
        <div class="subtitle">
          <strong>Consultant en Data Sciences - Aubay Data & AI</strong>
        </div>
      </header>

      <!-- Formation Académique -->
      <section class="cv-section">
        <h2>Formation Académique</h2>

        <div class="experience-item">
          <div class="experience-header">
            <strong>ENSAE Paris - IP Paris</strong>
            <span class="location">Palaiseau, France</span>
            <span class="date">Septembre 2021 - Juin 2024</span>
          </div>
          <div class="subtitle-italic">
            Cycle d'ingénieur (Probabilités, Statistiques, Machine Learning,
            Économétrie)
          </div>
          <div class="description">
            Théorie des Probabilités, Statistique Bayésienne, Séries Temporelles
            Linéaires, Optimisation Avancée, Économétrie<br />
            Deep Learning, Natural Language Processing, Machine Learning,
            Transport Optimal Statistique, Apprentissage en Ligne et
            Agrégation, Infrastructures et systèmes logiciels
          </div>
        </div>

        <div class="experience-item">
          <div class="experience-header">
            <strong>Lycée Saint-Louis</strong>
            <span class="location">Paris, France</span>
            <span class="date">Septembre 2019 - Juin 2021</span>
          </div>
          <div class="subtitle-italic">
            Classes préparatoires aux Grandes Écoles (filière Physique-Chimie)
          </div>
          <div class="description">
            Mathématiques, Physique, Chimie, Informatique
          </div>
        </div>
      </section>

      <!-- Expériences Professionnelles -->
      <section class="cv-section">
        <h2>Expériences Professionnelles</h2>

        <div class="experience-item">
          <div class="experience-header">
            <strong>Aubay Data & AI</strong>
            <span class="location">Boulogne-Billancourt, France</span>
            <span class="date">Depuis Janvier 2025</span>
          </div>
          <div class="subtitle-italic">
            Consultant Data Scientist - Contrat annuel chez SNCF Réseau
          </div>
          <div class="description">
            - Référent Data Science et ML pour l'optimisation de la maintenance prédictive des infrastructures ferroviaires<br/>
            - Ingénierie de données complexes : traitement et harmonisation de datasets temporels et géospatiaux multi-sources avec gestion des valeurs manquantes et des incohérences inter-fournisseurs<br/>
            - Utilisation d'algorithmes supervisés classqiues (XGBoost, Random Forest, Decision Tree, Régression Linéaire) pour la prédiction de l'apparition de défauts sur les voies ferrées<br/>
            - Optimisation de modèles sur données déséquilibrées par techniques de rééchantillonnage (SMOTE), ajustement des seuils de classification et métriques adaptées (Recall, F1-Score, ROC-AUC)<br/>
            - Calcul de matrices de corrélation croisée, algorithmes de recalage géospatial pour la correction de biais spatiaux<br/>
            - Création d'outils de visualisation interactive (dashboards) pour l'aide à la décision des équipes maintenance<br/>
            - Vulgarisation d'analyses statistiques, production de rapports de synthèse et recommandations opérationnelles
          </div>
        </div>

        <div class="experience-item">
          <div class="experience-header">
            <strong>Aubay</strong>
            <span class="location">Boulogne-Billancourt, France</span>
            <span class="date">Août 2024 - Décembre 2024</span>
          </div>
          <div class="subtitle-italic">
            Stage en Data Science - Machine Unlearning
          </div>
          <div class="description">
            - Rédaction d'un état de l'art sur le désapprentissage des LLMs
            (Concept Erasure, DPO, Prompt Corruption...)<br />
            - Fine-tuning d'un modèle LLaMA (approche LoRA) et implémentation
            d'un classificateur de prompt avec RoBERTa<br />
            - Mesure des performances à l'aide de métriques adaptées (Truth
            Ratio, probabilités conditionnelles, ROUGE score...)<br />
            - Exploration des techniques cross-linguales et développement
            d'approches innovantes pour le désapprentissage
          </div>
        </div>

        <div class="experience-item">
          <div class="experience-header">
            <strong>CARTEA Notaires</strong>
            <span class="location">Lèves, France</span>
            <span class="date">Juillet 2023 - Août 2023</span>
          </div>
          <div class="subtitle-italic">Collaborateur de Me TEA</div>
          <div class="description">
            - Conception et développement du site internet du Cabinet Notarial,
            renforçant sa visibilité numérique<br />
            - Optimisation complète du système informatique, incluant la
            restructuration intégrale des données du serveur
          </div>
        </div>
      </section>

      <!-- Projets Académiques Collaboratifs -->
      <section class="cv-section">
        <h2>Projets Académiques Collaboratifs</h2>

        <div class="experience-item">
          <div class="experience-header">
            <strong>Projet de ML (Multi-Armed Bandit Problem)</strong>
            <span class="date">Octobre 2023 - Janvier 2024</span>
          </div>
          <div class="subtitle-italic">
            Projet académique en Machine Learning
            <i class="fa fa-github"></i>
            <a href="https://github.com/fllin1/aml_mab" target="_blank">Lien</a>
          </div>
          <div class="description">
            - Documentation approfondie de l'état de l'art et identification
            d'une base de données appropriée à la problématique<br />
            - Implémentation puis mise en œuvre de divers algorithmes de Bandit
            Manchot Multi-Bras via apprentissage en ligne<br />
            - Évaluation des performances des algorithmes et comparaison
            statistique des résultats
          </div>
        </div>

        <div class="experience-item">
          <div class="experience-header">
            <strong>Projet de Statistique Bayésienne</strong>
            <span class="date">Novembre 2023 - Janvier 2024</span>
          </div>
          <div class="subtitle-italic">
            Projet académique en Statistique Bayésienne
            <i class="fa fa-github"></i>
            <a
              href="https://github.com/arthursabre/bayesian_statistics_project"
              target="_blank"
              >Lien</a
            >
          </div>
          <div class="description">
            - Traitement, structuration et analyse statistique d'une base de
            données à large dimension<br />
            - Étude mathématique d'un modèle de statistique Bayésienne et
            isolation des variables pertinentes<br />
            - Prédiction de variables à l'aide d'outils statistiques : Algorithme
            de Gibbs Sampling, régression Lasso, linéaire...
          </div>
        </div>

        <div class="experience-item">
          <div class="experience-header">
            <strong>Optimisation de Planning</strong>
            <span class="date">Novembre 2022 - Mai 2023</span>
          </div>
          <div class="subtitle-italic">
            Projet semi-professionnel : ENSAE Paris / Deloitte Conseil AIM
          </div>
          <div class="description">
            - Modélisation de contraintes paramétrables patients et infirmiers
            et formalisation mathématique de la problématique<br />
            - Implémentation des solutions les plus adéquates à un problème
            d'optimisation d'emploi du temps<br />
            - Définition et résolution d'un problème de routing à multiples
            entrées positionnelles et temporelles
          </div>
        </div>
      </section>

      <!-- Compétences -->
      <section class="cv-section">
        <h2>Compétences</h2>
        <table class="skills-table">
          <tbody>
            <tr>
              <td class="skill-label">Langues:</td>
              <td>Français (langue maternelle), Anglais (C1+), Chinois (B2)</td>
            </tr>
            <tr>
              <td class="skill-label">Programmation:</td>
              <td>
                Python (PyTorch, JAX, Scikit-learn, Pandas), R, SQL, HTML, CSS, JavaScript (basique)
              </td>
            </tr>
            <tr>
              <td class="skill-label">Outils Techniques:</td>
              <td>AWS, Docker, Office365, Latex, Git, (Firebase, Supabase)</td>
            </tr>
          </tbody>
        </table>
      </section>

      <!-- Page 2 - Projets Individuels -->
      <section class="cv-section">
        <h2>Projets Individuels</h2>
        
        <div class="experience-item">
          <div class="experience-header">
            <strong>Application Web MWPLU (Plans Locaux d'Urbanisme)</strong>
            <span class="date"> Mars 2025 - Mai 2025</span>
          </div>
          <div class="subtitle-italic">
            Développement Full-Stack
            <i class="fa fa-github"></i>
            <a href="https://github.com/fllin1/mwplu_webapp" target="_blank">Link</a>
          </div>
          <div class="description">
            - Développement d'une Single Page Application (SPA) avec Vue 3, backend Supabase et déploiement Firebase Hosting<br/>
            - Implémentation complète avec gestion des sessions, Row Level Security (RLS) et intégration CAPTCHA Turnstile<br/>
            - Intégration Google Analytics 4 avec événements personnalisés, respect GDPR et politique de confidentialité<br/>
            - Composants Vue réactifs pour la sélection hiérarchique de données, système de commentaires et notation en temps réel<br/>
            - Gestion de données géospatiales complexes avec API Supabase, Edge Functions et stockage sécurisé de documents<br/>
            - OCR et synthèse de centaines de pages de documents d'urbanisme via Python, Mistral API et Google AI<br/>
          </div>
        </div>

        <div class="experience-item">
          <div class="experience-header">
            <strong>Classification d'Acheteurs en Ligne</strong>
            <span class="date">Juillet 2024</span>
          </div>
          <div class="subtitle-italic">
            Machine Learning
            <i class="fa fa-github"></i>
            <a
              href="https://github.com/fllin1/classification-online-shoppers"
              target="_blank"
              >Lien</a
            >
          </div>
          <div class="description">
            - Prétraitement des données, extraction de caractéristiques et
            analyse des variables explicatives pour la classification<br />
            - Implémentation d'algorithmes de classification supervisée afin de
            prédire le comportement d'achat<br />
            - Implémentation de métriques adéquates à des données
            déséquilibrées (précision, rappel et courbe ROC)<br />
            - Analyse approfondie des résultats et optimisation des
            hyperparamètres pour améliorer la prédiction
          </div>
        </div>

        <div class="experience-item">
          <div class="experience-header">
            <strong>Prédiction du Genre à partir de Données Textuelles</strong>
            <span class="date">Février 2024 - Mars 2024</span>
          </div>
          <div class="subtitle-italic">
            Projet académique en NLP
            <i class="fa fa-github"></i>
            <a href="https://github.com/fllin1/nlp_project" target="_blank"
              >Lien</a
            >
          </div>
          <div class="description">
            - Analyse de données contenant des prénoms et des transcriptions
            avec des informations associées au genre<br />
            - Nettoyage et structuration des données en séparant les colonnes
            combinées et en filtrant les entrées ambiguës<br />
            - Implémentation de fonctions utilisant des expressions régulières
            pour extraire des informations spécifiques<br />
            - Exploration de techniques de classification supervisée pour la
            prédiction du genre à partir des données
          </div>
        </div>

        <div class="experience-item">
          <div class="experience-header">
            <strong>Bot d'échecs</strong>
            <span class="date">Septembre 2023</span>
          </div>
          <div class="subtitle-italic">
            Algorithme Minimax
            <i class="fa fa-github"></i>
            <a href="https://github.com/fllin1/chess_bot" target="_blank"
              >Lien</a
            >
          </div>
          <div class="description">
            - Implémentation de l'algorithme Minimax pour la prise de décisions
            stratégiques dans une partie d'échecs<br />
            - Développement d'une fonction d'évaluation basique permettant
            d'estimer la qualité des positions de jeu
          </div>
        </div>
      </section>
    </div>
  </div>
</template>

<script setup lang="ts">
// Le composant est prêt à être utilisé
</script>

<style scoped>
/* Import Font Awesome */
@import url("https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css");

/* Container principal */
.cv-container {
  max-width: 210mm;
  margin: 0 auto;
  font-family: "Times New Roman", Times, serif;
  font-size: 11pt;
  line-height: 1.3;
  color: #000;
}

.cv-page {
  padding: 10mm 10mm 10mm 10mm;
  background: white;
  min-height: 297mm;
}

/* Header */
.cv-header {
  text-align: center;
  margin-bottom: 10px;
}

.name {
  font-size: 18pt;
  font-weight: bold;
  margin: 0 0 5px 0;
  letter-spacing: 0.5px;
}

.contact-info {
  font-size: 10pt;
  margin: 5px 0;
}

.contact-row {
  margin: 2px 0;
}

.contact-item {
  margin: 0 10px;
  display: inline-block;
}

.contact-item a {
  color: #000;
  text-decoration: none;
}

.contact-item i {
  margin-right: 3px;
}

.subtitle {
  text-align: center;
  margin-top: 8px;
  font-size: 11pt;
}

/* Sections */
.cv-section {
  margin-bottom: 15px;
}

.cv-section h2 {
  font-size: 14pt;
  font-weight: bold;
  margin: 10px 0 5px 0;
  border-bottom: 1px solid #000;
  padding-bottom: 2px;
  page-break-after: avoid; /* Empêche la coupure juste après un titre */
  break-after: avoid;
}

/* Experience items */
.experience-item {
  margin-bottom: 10px;
  page-break-inside: avoid; /* Empêche la coupure à l'intérieur */
  break-inside: avoid; /* Pour les navigateurs modernes */
}

.experience-header {
  display: flex;
  justify-content: space-between;
  align-items: baseline;
  margin-bottom: 2px;
}

.experience-header strong {
  font-weight: bold;
  page-break-inside: avoid;
  break-inside: avoid;
}

.location {
  font-weight: normal;
  margin-left: 8px;
}

.date {
  font-style: italic;
  margin-left: auto;
  white-space: nowrap;
}

.subtitle-italic {
  font-style: italic;
  margin: 2px 0;
  font-size: 10.5pt;
}

.subtitle-italic a {
  color: #000;
  text-decoration: none;
  margin-left: 5px;
}

.subtitle-italic i {
  margin-left: 10px;
}

.description {
  margin: 3px 0;
  font-size: 10.5pt;
  line-height: 1.4;
  orphans: 1; /* Minimum 1 ligne en bas de page */
  widows: 1;  /* Minimum 1 ligne en haut de page */
}

/* Skills table */
.skills-table {
  width: 100%;
  font-size: 10.5pt;
  border-collapse: collapse;
}

.skills-table tr {
  vertical-align: top;
}

.skill-label {
  font-weight: bold;
  width: 150px;
  padding-right: 20px;
  padding-bottom: 5px;
}

/* Page break */
.page-break {
  page-break-before: always;
  margin-top: 0;
}

/* Print styles */
@media print {
  .cv-container {
    max-width: 100%;
  }

  .cv-page {
    padding: 10mm 20mm 10mm 10mm;
    box-shadow: none;
  }

  .page-break {
    page-break-before: always;
  }
}

/* Responsive - uniquement pour les très petits écrans */
@media (max-width: 600px) {
  .cv-page {
    padding: 15px;
  }

  .experience-header {
    flex-direction: column;
    align-items: flex-start;
  }

  .date {
    margin-left: 0;
  }

  .contact-item {
    display: block;
    margin: 3px 0;
  }
}
</style>
