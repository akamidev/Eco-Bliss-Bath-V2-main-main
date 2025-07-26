# Projet Eco-Bliss-Bath V2## 🎬 Démonstration

[![Démonstration Eco-Bliss-Bath](https://img.shields.io/badge/📽️%20Voir%20la%20Démonstration-Vidéo%20Locale-4A90E2?style=for-the-badge&logo=video&logoColor=white)](./Cypress1024.mp4)

> **🎥 Cliquez sur le badge ci-dessus pour voir la démonstration complète du projet**
> 
> La vidéo présente :
> - 🐳 Démarrage de l'environnement Docker
> - 🅰️ Lancement du frontend Angular
> - 🧪 Exécution des tests Cypress
> - 📊 Génération des rapports Mochawesome
> - 🔧 Résolution de problèmes courants

*Alternative avec image de démonstration :*

[![Démonstration du Projet](https://via.placeholder.com/800x400/4A90E2/ffffff?text=🎬+Cypress+Demo+▶️)](./Cypress1024.mp4)

📹 **Fichier vidéo :** `Cypress1024.mp4` (situé à la racine du projet)rrage Complet

![Angular](https://img.shields.io/badge/Angular-13.3-DD0031?style=for-the-badge&logo=angular&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-4.6-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Symfony](https://img.shields.io/badge/Symfony-API-000000?style=for-the-badge&logo=symfony&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-7.4+-777BB4?style=for-the-badge&logo=php&logoColor=white)
![MariaDB](https://img.shields.io/badge/MariaDB-11.7-003545?style=for-the-badge&logo=mariadb&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-Compose-2496ED?style=for-the-badge&logo=docker&logoColor=white)

![Cypress](https://img.shields.io/badge/Cypress-14.5-17202C?style=for-the-badge&logo=cypress&logoColor=white)
![Mochawesome](https://img.shields.io/badge/Mochawesome-Reports-FF6B6B?style=for-the-badge&logo=javascript&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-16%2B-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![npm](https://img.shields.io/badge/npm-Package%20Manager-CB3837?style=for-the-badge&logo=npm&logoColor=white)
![Git](https://img.shields.io/badge/Git-Version%20Control-F05032?style=for-the-badge&logo=git&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger-API%20Doc-85EA2D?style=for-the-badge&logo=swagger&logoColor=black)

## 📋 Présentation du Projet

Ce projet constitue une plateforme de tests automatisés pour l'application e-commerce **Eco-Bliss-Bath**, spécialisée dans la vente de produits de bain écologiques. Il comprend une API backend développée avec Symfony, une interface frontend Angular, une base de données MariaDB, et une suite complète de tests automatisés avec Cypress.

### 🎯 Objectifs du Projet
- Automatiser les tests fonctionnels critiques (connexion, panier, API)
- Effectuer des tests de régression et de smoke testing
- Générer des rapports de tests détaillés avec Mochawesome
- Valider la sécurité avec des tests XSS

## � Démonstration

[![Démonstration Eco-Bliss-Bath](https://img.shields.io/badge/📽️%20Voir%20la%20Démonstration-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://youtu.be/VOTRE_VIDEO_ID)

> **🎥 Cliquez sur le badge ci-dessus pour voir la démonstration complète du projet**
> 
> La vidéo présente :
> - 🐳 Démarrage de l'environnement Docker
> - 🅰️ Lancement du frontend Angular
> - 🧪 Exécution des tests Cypress
> - 📊 Génération des rapports Mochawesome
> - 🔧 Résolution de problèmes courants

*Vous pouvez également utiliser cette image de démonstration alternative :*

[![Démonstration du Projet](https://via.placeholder.com/800x400/1e3a8a/ffffff?text=🚀+Eco-Bliss-Bath+Demo+📱)](https://youtu.be/VOTRE_VIDEO_ID)

## �🏗️ Architecture Technique

```
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│   Frontend      │    │   Backend API   │    │   Base de       │
│   Angular 13    │◄───┤   Symfony       │◄───┤   Données       │
│   Port: 4200    │    │   Port: 8081    │    │   MariaDB       │
└─────────────────┘    └─────────────────┘    └─────────────────┘
         ▲                       ▲                       
         │                       │                       
┌─────────────────┐    ┌─────────────────┐              
│   Tests E2E     │    │   Documentation │              
│   Cypress       │    │   Swagger UI    │              
│   + Mochawesome │    │   Port: 8081    │              
└─────────────────┘    └─────────────────┘              
```

## 🛠️ Prérequis Système

Avant de commencer, assurez-vous d'avoir installé les outils suivants :

### Prérequis Obligatoires
- **Docker Desktop** (version 4.0+)
- **Node.js** (version 16 ou 18 - **évitez la v21**)
- **npm** (version 8+)
- **Git** (version 2.0+)

### Prérequis Optionnels
- **Angular CLI** global : `npm install -g @angular/cli`
- **Cypress** (sera installé automatiquement)

### ⚠️ Notes de Compatibilité
- **Node.js v21** n'est pas officiellement supportée par Angular 13
- Utilisez de préférence **Node.js v16 ou v18 LTS**

## 📦 Installation et Configuration

### 1. Clonage du Projet

```bash
git clone https://github.com/Natm777/Eco-Bliss-Bath-V2-main
cd Eco-Bliss-Bath-V2-main
```

### 2. Démarrage de l'Infrastructure Backend

#### 2.1 Lancement des Services Docker

```bash
# Depuis la racine du projet
docker compose up -d
```

Cette commande lance :
- **Base de données MariaDB** : Conteneur `bliss-bath-bdd`
- **API Backend Symfony** : Conteneur `bliss-bath-symfony`

#### 2.2 Vérification du Démarrage

```bash
# Vérifier l'état des conteneurs
docker ps

# Vérifier les logs en cas de problème
docker logs bliss-bath-bdd
docker logs bliss-bath-symfony
```

**Services disponibles :**
- API Backend : `http://localhost:8081`
- Documentation Swagger : `http://localhost:8081/api/doc`
- Health Check API : `http://localhost:8081/api/health`

### 3. Configuration du Frontend Angular

#### 3.1 Installation des Dépendances

```bash
cd frontend
npm install
```

#### 3.2 Démarrage du Serveur de Développement

```bash
npm start
# ou
npm run start
```

Le frontend sera accessible sur : `http://localhost:4200`

**Note :** Si le port 4200 est occupé, Angular proposera automatiquement un port alternatif.

### 4. Installation et Configuration de Cypress

#### 4.1 Installation depuis la Racine

```bash
# Retourner à la racine du projet
cd ..

# Installer Cypress et les dépendances de test
npm install --save-dev cypress
npm install --save-dev mochawesome
```

#### 4.2 Configuration des Scripts de Test

Le fichier `package.json` contient les scripts suivants :

```json
{
  "scripts": {
    "test:mochawesome": "cypress run --reporter mochawesome --reporter-options \"reportDir=cypress/reports/mochawesome,overwrite=false,html=true,json=true\"",
    "test:headless": "cypress run",
    "test:open": "cypress open"
  }
}
```

## 🧪 Exécution des Tests

### Prérequis pour les Tests
**⚠️ Important :** Assurez-vous que tous les services sont démarrés avant d'exécuter les tests :
- ✅ Docker containers (API + BDD)
- ✅ Frontend Angular
- ✅ Port 4200 accessible

### 1. Tests en Mode Graphique (Recommandé pour le Développement)

```bash
npx cypress open
```

Interface graphique permettant de :
- Sélectionner et exécuter des tests individuels
- Observer l'exécution en temps réel
- Déboguer les tests interactivement

### 2. Tests en Mode Ligne de Commande

#### 2.1 Exécution Standard

```bash
npx cypress run
```

#### 2.2 Exécution avec Rapport Mochawesome

```bash
# Méthode recommandée
npm run test:mochawesome

# Ou directement avec npx
npx cypress run --reporter mochawesome --reporter-options "reportDir=cypress/reports/mochawesome,overwrite=false,html=true,json=true"
```

## 📊 Suites de Tests Disponibles

### Tests Fonctionnels Frontend
- **`1-login.cy.js`** : Tests de connexion utilisateur
- **`2-pannier.cy.js`** : Tests du panier d'achat
- **`3-smokeBoutonPannier.cy.js`** : Tests smoke du bouton panier
- **`4-smokeConnexion.cy.js`** : Tests smoke de connexion

### Tests de Sécurité
- **`5-testXss.cy.js`** : Tests de vulnérabilités XSS

### Tests API Backend
- **`apiHealth.cy.js`** : Tests de santé de l'API
- **`apiLogin.cy.js`** : Tests d'authentification API
- **`apiGetProducts.cy.js`** : Tests de récupération des produits
- **`apiGetOrders.cy.js`** : Tests de récupération des commandes
- **`apiGetReviews.cy.js`** : Tests de récupération des avis
- **`apiPostOrders.cy.js`** : Tests de création de commandes
- **`apiPutOrders.cy.js`** : Tests de modification de commandes
- **`apiDeleteOrders.cy.js`** : Tests de suppression de commandes
- **`apiChangeQuantity.cy.js`** : Tests de modification des quantités
- **`apiPostRegister.cy.js`** : Tests d'inscription
- **`apiGetInformation.cy.js`** : Tests de récupération d'informations

## 📈 Génération et Consultation des Rapports

### 1. Rapports Mochawesome

Après exécution des tests avec Mochawesome :

**Localisation des rapports :**
```
cypress/
└── reports/
    └── mochawesome/
        ├── mochawesome.html          # Rapport principal
        ├── mochawesome_*.html         # Rapports individuels
        ├── mochawesome_*.json         # Données JSON
        └── assets/                    # Ressources CSS/JS
```

**Ouverture du rapport :**
```bash
# Windows
start cypress/reports/mochawesome/mochawesome.html

# MacOS
open cypress/reports/mochawesome/mochawesome.html

# Linux
xdg-open cypress/reports/mochawesome/mochawesome.html
```

### 2. Captures d'Écran et Vidéos

Les captures d'écran des échecs sont automatiquement sauvegardées dans :
```
cypress/
├── screenshots/           # Captures d'écran des échecs
└── videos/               # Enregistrements vidéo (mode headless)
```

### 3. Métriques des Rapports

Les rapports Mochawesome incluent :
- **Statistiques globales** : Nombre de tests, succès, échecs
- **Durée d'exécution** : Temps total et par test
- **Taux de réussite** : Pourcentage de succès
- **Détails des échecs** : Messages d'erreur et stack traces
- **Captures d'écran** : Images des échecs

## 🔧 Résolution des Problèmes Courants

### Problème : Conteneurs Docker qui ne démarrent pas

```bash
# Arrêter tous les conteneurs
docker compose down

# Nettoyer les volumes (⚠️ supprime les données)
docker compose down -v

# Redémarrer
docker compose up -d
```

### Problème : Port 4200 déjà utilisé

Angular proposera automatiquement un port alternatif. Acceptez la proposition ou libérez le port :

```bash
# Windows - Trouver le processus sur le port 4200
netstat -ano | findstr :4200

# Tuer le processus (remplacer PID par l'ID du processus)
taskkill /PID <PID> /F
```

### Problème : Tests Cypress qui échouent

1. **Vérifiez que tous les services sont démarrés**
2. **Vérifiez les URLs dans cypress.config.js**
3. **Consultez les logs des conteneurs Docker**
4. **Vérifiez la connectivité réseau**

### Problème : Rapports Mochawesome non générés

```bash
# Vérifiez l'installation de Mochawesome
npm list mochawesome

# Réinstallez si nécessaire
npm install --save-dev mochawesome

# Vérifiez les permissions d'écriture sur le dossier cypress/reports
```

## 🌐 URLs de Référence

| Service | URL | Description |
|---------|-----|-------------|
| Frontend Angular | `http://localhost:4200` | Interface utilisateur |
| API Backend | `http://localhost:8081` | API REST Symfony |
| Documentation Swagger | `http://localhost:8081/api/doc` | Documentation interactive API |
| Health Check | `http://localhost:8081/api/health` | Statut de l'API |

## 📚 Documentation Complémentaire

### Configuration Cypress

Le fichier `cypress.config.js` contient la configuration principale :

```javascript
module.exports = defineConfig({
  env: {
    apiUrl: "http://localhost:8081"
  },
  e2e: {
    baseUrl: "http://localhost:4200/",
  }
});
```

### Structure des Fixtures

```
cypress/fixtures/
├── example.json          # Données d'exemple
├── profile.json          # Profils utilisateur test
└── users.json            # Données utilisateurs
```

### Commandes Personnalisées

Le fichier `cypress/support/commands.js` contient des commandes réutilisables comme `checkAddToCartButtonFromProductIndex()`.

## 🚀 Workflow de Développement Recommandé

1. **Démarrage de l'environnement**
   ```bash
   docker compose up -d
   cd frontend && npm start
   ```

2. **Développement de tests**
   ```bash
   npx cypress open
   ```

3. **Validation complète**
   ```bash
   npm run test:mochawesome
   ```

4. **Analyse des résultats**
   - Consulter les rapports Mochawesome
   - Examiner les captures d'écran
   - Corriger les échecs identifiés

## 📋 Checklist de Validation

Avant de considérer l'environnement comme opérationnel :

- [ ] Conteneurs Docker démarrés et healthy
- [ ] Frontend Angular accessible sur port 4200 (ou alternatif)
- [ ] API Backend répond sur `/api/health`
- [ ] Documentation Swagger accessible
- [ ] Tests Cypress s'exécutent sans erreur de configuration
- [ ] Rapports Mochawesome générés correctement

## 🤝 Contribution et Support

Ce projet suit les bonnes pratiques de test et de documentation. Pour toute question ou amélioration :

1. Consultez d'abord cette documentation
2. Vérifiez les logs des services
3. Examinez les rapports de tests existants
4. Proposez des améliorations via les issues GitHub

---

**Dernière mise à jour :** Juillet 2025  
**Version du projet :** 2.0  
**Compatibilité testée :** Windows 10/11, Node.js 16-18, Docker Desktop 4.0+
