# TimeOrganiser - Agenda assisté par IA

Application mobile de gestion de calendrier pilotée par un assistant d'intelligence artificielle.

## 📋 Description

TimeOrganiser est une application d'agenda moderne qui utilise l'intelligence artificielle pour simplifier la gestion de votre calendrier. Au lieu de remplir des formulaires complexes, décrivez simplement vos événements en langage naturel, et l'IA s'occupe du reste !

## ✨ Fonctionnalités principales

### 🤖 Assistant IA
- **Saisie en langage naturel** : "Réunion demain à 14h avec Paul pendant 1 heure"
- **Saisie vocale** : Dictez vos événements
- **Mode aperçu** : Validez les propositions avant ajout
- **Mode automatique** : Ajout direct des événements

### 📅 Gestion de calendrier
- **Vues multiples** : Jour, Semaine, Mois
- **Événements récurrents** : Support du format RRULE (RFC 5545)
- **Détection de conflits** : Avertissement en cas de chevauchement
- **Rappels personnalisables** : Notifications locales

### 🔒 Sécurité & Confidentialité
- **Offline-first** : Fonctionne sans connexion
- **Données chiffrées** : Base locale SQLite chiffrée
- **Consentement IA** : Contrôle total sur l'utilisation de l'IA
- **Synchronisation sécurisée** : Gestion des conflits

### 🎯 Autres fonctionnalités
- Partage d'événements avec invitations
- Interface responsive
- Mode hors ligne avec file d'attente
- Gestion des exceptions de récurrence

## 🚀 Démarrage rapide

### Prérequis
- Node.js 18+
- npm 11+

### Installation

```bash
# Cloner le projet
git clone <repository-url>
cd timeorganiser

# Installer les dépendances
npm install

# Lancer l'application en mode développement
npm start
```

L'application sera accessible sur `http://localhost:4200`

### Compte de démonstration

Au premier lancement, un compte démo est automatiquement créé :
- **Email** : demo@timeorganiser.com
- **Mot de passe** : demo123

## 🏗️ Architecture

### Stack technique
- **Frontend** : Angular 22 avec Signals
- **Base de données locale** : SQLite (simulation via localStorage)
- **Styling** : CSS natif avec design moderne
- **IA** : Integration API LLM (simulation pour la démo)

### Structure du projet

```
src/
├── app/
│   ├── components/          # Composants UI
│   │   ├── ai-input/       # Saisie assistée par IA
│   │   └── calendar-view/  # Vues calendrier
│   ├── services/           # Services métier
│   │   ├── auth.service.ts
│   │   ├── calendar.service.ts
│   │   ├── ia.service.ts
│   │   └── preferences.service.ts
│   └── models/             # Modèles de données
│       ├── event.model.ts
│       ├── ia.model.ts
│       ├── user.model.ts
│       └── sync.model.ts
```

## 📖 Utilisation

### Créer un événement avec l'IA

1. Cliquez sur l'icône 🤖 pour ouvrir l'assistant IA
2. Décrivez votre événement en langage naturel :
   - "Réunion demain à 14h pendant 1 heure"
   - "Cours de maths tous les lundis et mercredis de 8h à 10h"
   - "Rendez-vous chez le dentiste vendredi prochain à 15h30"
3. Vérifiez l'aperçu généré
4. Validez pour ajouter l'événement au calendrier

### Navigation dans le calendrier

- **Vue Jour** : Grille horaire complète de la journée
- **Vue Semaine** : 7 jours côte à côte
- **Vue Mois** : Vue mensuelle avec compteur d'événements
- Utilisez les flèches pour naviguer entre les périodes
- Cliquez sur "Aujourd'hui" pour revenir à la date actuelle

### Paramètres

Accédez aux paramètres via l'icône ⚙️ :
- **Mode d'ajout** : Aperçu ou Automatique
- **Consentement IA** : Activer/Désactiver l'assistant
- **Notifications** : Gérer les rappels

## 🔧 Configuration

### Clé API IA

La clé API fournie dans le code est à des fins de démonstration. Pour utiliser une vraie API LLM :

1. Obtenez votre clé API auprès de votre fournisseur
2. Modifiez `src/app/services/ia.service.ts` :

```typescript
private readonly API_KEY = 'VOTRE_CLE_API';
private readonly API_ENDPOINT = 'https://api.votre-fournisseur.com';
```

## 🧪 Tests

```bash
# Lancer les tests unitaires
npm test

# Tests end-to-end
npm run e2e

# Coverage
npm run test:coverage
```

## 📦 Build

```bash
# Build de production
npm run build

# Les fichiers compilés se trouvent dans dist/
```

## 🎨 Personnalisation

### Thème

Les couleurs principales peuvent être modifiées dans `src/app/app.css` :

```css
:root {
  --primary-color: #2196F3;
  --success-color: #4CAF50;
  --danger-color: #f44336;
}
```

## 🐛 Problèmes connus

- La reconnaissance vocale nécessite une connexion HTTPS
- Certains constructeurs Android peuvent limiter les notifications en arrière-plan
- La synchronisation multi-appareils n'est pas encore implémentée

## 🚀 Roadmap

- [ ] Import d'événements depuis image/PDF
- [ ] Synchronisation avec Google Agenda/Outlook
- [ ] Mode collaboratif temps réel
- [ ] Application pour montre connectée
- [ ] Support multilingue complet
- [ ] Suggestions proactives de créneaux

## 📄 Licence

Ce projet est sous licence MIT.

## 👥 Contribution

Les contributions sont les bienvenues ! N'hésitez pas à ouvrir une issue ou une pull request.

## 📞 Support

Pour toute question ou problème, veuillez ouvrir une issue sur GitHub.

---

**Version** : 1.0.0  
**Date** : Janvier 2027  
**Auteur** : Équipe TimeOrganiser
"# Projet_Agil" 
