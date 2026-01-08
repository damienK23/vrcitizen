# Guide de migration vers GitHub

Ce guide vous explique comment migrer ce projet vers un nouveau dépôt GitHub.

## 📋 Préparation

### Fichiers essentiels à inclure

1. **Documentation** :
   - `README.md` - Vue d'ensemble du projet
   - `INSTALLATION.md` - Guide d'installation
   - `CONTROLS.md` - Documentation des contrôles
   - `CHANGELOG.md` - Historique des versions
   - `MIGRATION.md` - Ce fichier

2. **Fichiers de configuration** :
   - `reWASD/VRCitizenXEliteS2-0.01.rewasd` - Profil reWASD
   - `StarCitizen/VRCitizenXEliteS2-0.01.xml` - Profil Star Citizen

3. **Fichiers de configuration Git** :
   - `.gitignore` - Fichiers à ignorer

### Structure recommandée pour GitHub

```
VRCitizenXEliteS2/
├── README.md
├── INSTALLATION.md
├── CONTROLS.md
├── CHANGELOG.md
├── MIGRATION.md
├── .gitignore
│
├── reWASD/
│   └── VRCitizenXEliteS2-0.01.rewasd
│
└── StarCitizen/
    └── VRCitizenXEliteS2-0.01.xml
```

## 🚀 Étapes de migration

### 1. Créer le nouveau dépôt GitHub

1. Aller sur GitHub.com
2. Cliquer sur "New repository"
3. Nommer le dépôt (ex: `VRCitizenXEliteS2`)
4. Choisir Public ou Private
5. **Ne pas** initialiser avec README, .gitignore, ou licence (on les ajoutera manuellement)
6. Cliquer sur "Create repository"

### 2. Préparer le dossier local

1. Créer un nouveau dossier pour le projet :
   ```bash
   mkdir VRCitizenXEliteS2
   cd VRCitizenXEliteS2
   ```

2. Copier les fichiers essentiels :
   ```bash
   # Copier la documentation
   cp README.md INSTALLATION.md CONTROLS.md CHANGELOG.md MIGRATION.md .gitignore .
   
   # Créer les dossiers
   mkdir -p reWASD StarCitizen
   
   # Copier les fichiers de configuration
   cp "CouchCitizen3.22/REWASD PROFILES/VRCitizenXEliteS2-0.01.rewasd" reWASD/
   cp "CouchCitizen3.22/SC PROFILES/VRCitizenXEliteS2-0.01.xml" StarCitizen/
   ```

### 3. Initialiser Git

1. Initialiser le dépôt Git :
   ```bash
   git init
   ```

2. Ajouter les fichiers :
   ```bash
   git add .
   ```

3. Faire le premier commit :
   ```bash
   git commit -m "Initial commit: Version 0.01"
   ```

### 4. Connecter au dépôt GitHub

1. Ajouter le remote :
   ```bash
   git remote add origin https://github.com/[VOTRE_USERNAME]/VRCitizenXEliteS2.git
   ```

2. Renommer la branche principale (si nécessaire) :
   ```bash
   git branch -M main
   ```

3. Pousser vers GitHub :
   ```bash
   git push -u origin main
   ```

## 📝 Fichiers optionnels à inclure

### Si vous voulez garder l'historique

Vous pouvez inclure les changelogs précédents dans un dossier `docs/` :

```
docs/
├── CHANGELOG_WIP29.txt
├── CHANGELOG_WIP30.txt
├── ...
└── CHANGELOG_WIP44.txt
```

### Si vous voulez inclure des exemples

Créer un dossier `examples/` avec des configurations alternatives :

```
examples/
├── alternative-keybinds.xml
└── custom-mappings.rewasd
```

## 🔧 Configuration post-migration

### Ajouter une licence

1. Créer un fichier `LICENSE` (MIT, GPL, etc.)
2. Ajouter la référence dans le README.md

### Configurer les GitHub Pages (optionnel)

Si vous voulez héberger la documentation :

1. Aller dans Settings → Pages
2. Choisir la branche `main` et le dossier `/docs`
3. La documentation sera accessible sur `https://[USERNAME].github.io/VRCitizenXEliteS2/`

### Ajouter des badges (optionnel)

Ajouter des badges dans le README.md :

```markdown
![Version](https://img.shields.io/badge/version-0.01-blue)
![Star Citizen](https://img.shields.io/badge/Star%20Citizen-3.22+-green)
![reWASD](https://img.shields.io/badge/reWASD-6.x+-orange)
```

## ✅ Checklist de migration

- [ ] Dépôt GitHub créé
- [ ] Dossier local préparé avec tous les fichiers
- [ ] Structure de dossiers créée (reWASD/, StarCitizen/)
- [ ] Documentation copiée (README, INSTALLATION, CONTROLS, CHANGELOG)
- [ ] Fichiers de configuration copiés (.rewasd, .xml)
- [ ] .gitignore configuré
- [ ] Git initialisé et premier commit fait
- [ ] Dépôt connecté à GitHub
- [ ] Code poussé vers GitHub
- [ ] README vérifié et mis à jour si nécessaire
- [ ] Licence ajoutée (optionnel)
- [ ] Badges ajoutés (optionnel)

## 🎯 Prochaines étapes

Après la migration :

1. **Tester** que tout fonctionne correctement
2. **Créer des releases** pour les versions futures
3. **Ajouter des tags** pour marquer les versions importantes
4. **Configurer les issues** et les templates de pull request
5. **Ajouter des contributeurs** si nécessaire

## 📞 Support

Si vous rencontrez des problèmes lors de la migration :

1. Vérifier que tous les fichiers sont bien copiés
2. Vérifier que le .gitignore est correct
3. Vérifier les permissions du dépôt GitHub
4. Consulter la documentation Git/GitHub

---

**Note** : Ce guide suppose que vous partez de zéro. Si vous voulez migrer un dépôt Git existant, les étapes seront différentes.

