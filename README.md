<p align="center">
  <img width="327" height="327" alt="image" src="https://github.com/user-attachments/assets/c3488b80-5907-4d09-abd2-20d19c3dc098" />
</p>

# MindBridge Africa

**Plateforme intelligente de dépistage, d'orientation et de suivi en santé mentale pour l'Afrique subsaharienne.**

> *Listen · Understand · Support*



## Le problème

L'Afrique traverse une crise de santé mentale silencieuse :

- **+116 millions** de personnes vivent avec un trouble mental
- **1 psychiatre pour 1 million** d'habitants en Afrique subsaharienne (contre 9 en Europe)
- **+90 %** des patients ne reçoivent aucun traitement formel
- **< 1 %** des budgets de santé est consacré à la santé mentale

Au-delà du manque de médecins, c'est l'**absence d'un système de détection précoce** qui pose problème : stigmatisation, éloignement des soins, délais de plusieurs mois. La crise n'est visible que lorsqu'elle éclate à l'hôpital, ou pire, lorsqu'il est trop tard.

## La solution

MindBridge Africa automatise le parcours de soins en trois étapes :

| Étape | Description |
|---|---|
| **Dépister** | Questionnaire conversationnel adapté culturellement (anxiété, dépression, SSPT), rempli par le patient ou assisté par un agent de santé communautaire, dans sa langue |
| **Orienter** | Un score de détresse généré par IA (faible, modéré, élevé, critique) déclenche l'orientation automatique vers la ressource la plus adaptée et la plus proche : ligne d'écoute, centre de santé, psychiatre |
| **Suivre** | Relances SMS automatiques à J+7, J+14 et J+30, suivi longitudinal du score et alertes d'escalade pour les superviseurs médicaux |

## Utilisateurs

| Persona | Rôle |
|---|---|
| **Patient** | Effectue son auto-évaluation, reçoit son orientation et ses rappels de suivi, peut utiliser l'application de manière anonyme |
| **Agent de Santé Communautaire (ASC)** | Crée et gère les dossiers des patients sans smartphone, les assiste lors de l'évaluation |
| **Superviseur Médical** | Surveille les cas, reçoit les alertes d'escalade, valide les orientations |
| **Administrateur Régional de la Santé** | Consulte les statistiques agrégées et alloue les ressources de soins |

Le Blueprint définit au total **7 personas**.

## Fonctionnalités

### Côté patient
- Auto-évaluation conversationnelle multilingue (français, wolof, fon, etc.)
- Score de détresse généré par IA
- Orientation automatique selon le score et la localisation
- Notifications SMS de suivi
- Mode anonyme pour réduire la stigmatisation

### Côté agent de santé communautaire
- Création et gestion des dossiers patients
- Assistance à l'évaluation
- Application des recommandations de l'IA
- Tableau de bord de performance

### Côté superviseur et administration
- Suivi des scores de détresse dans le temps
- Alertes d'escalade en cas d'aggravation ou de risque de rechute prédit
- Validation des orientations proposées par l'IA ou les ASC
- Tableau de bord statistique régional et aide à l'allocation des ressources

### Côté système
- Génération du score de détresse par IA
- Routage automatique vers les parcours de soins
- Mise en correspondance avec la ressource disponible la plus proche
- Génération automatique de lettres de référence
- Envoi de notifications SMS aux patients et aux établissements receveurs
- Suivi et confirmation des référencements
- Suivi longitudinal et prédiction du risque de rechute
- Intégration avec les rapports des autorités de santé

## Architecture

Application générée avec **Pega GenAI Blueprint™** (Blueprint ID : `BP-2028285`).

**6 workflows (case types)**

1. **Mental Health Screening** : dépistage automatisé
2. **Crisis Intervention** : urgences et ligne d'écoute
3. **Patient Care Journey** : suivi de bout en bout
4. **Family Support Program** : accompagnement des familles
5. **Awareness Campaign** : sensibilisation multilingue contre la stigmatisation
6. **Partner Collaboration** : ONG, hôpitaux, ministères

**7 personas · 15 objets de données**

**Intégrations**
- Passerelle SMS africaine
- Géolocalisation
- Télépsychologie
- OpenID Connect

## Accessibilité et inclusion

Conçue pour celles et ceux qui ne sont jamais entendus, dès le premier écran :

- **Pictogrammes universels** : utilisable sans savoir lire
- **Questionnaires audio** en langues nationales (susu, pular, malinké, fon, éwé, kabiyè, wolof)
- **SMS et USSD** : fonctionne sur un téléphone basique, sans internet
- **Agents de santé communautaires** : une personne de confiance du même village accompagne chaque étape

## Modèle économique

| Public | Offre |
|---|---|
| **Patients** | Gratuit (dépistage, score, orientation, suivi SMS) |
| **Professionnels de santé** | Abonnement (module de télépsychologie, gestion des dossiers, tableau de bord clinique) |
| **Institutions** (hôpitaux, ONG, ministères) | Contrats annuels (intégration hospitalière, rapports agrégés, campagnes de sensibilisation) |

## Feuille de route

- **Phase 1 (6 mois)** : pilote en Guinée, au Bénin et au Togo
- **Phase 2 (12 à 18 mois)** : extension au Sénégal, en Côte d'Ivoire, au Cameroun et au Nigeria
- **Phase 3 (2 à 3 ans)** : modèle panafricain en franchises locales

## Aperçu

<img width="1567" height="857" alt="image" src="https://github.com/user-attachments/assets/1a457b98-1ef0-45fb-b185-1302a3f43013" />

## Stack

`Pega GenAI Blueprint™` · `Pega Launchpad` · `SMS / USSD` · `Géolocalisation` · `OpenID Connect`
