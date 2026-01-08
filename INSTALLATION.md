# Guide d'installation - VRCitizen X Elite S2

Ce guide vous explique comment installer et configurer VRCitizen X Elite S2 pour jouer à Star Citizen avec une manette Xbox Elite Series 2.

## 📋 Prérequis

1. **reWASD** installé et activé (version 6.x ou supérieure)
   - Télécharger depuis : https://www.rewasd.com/
   - Une licence est requise pour utiliser les fonctionnalités avancées

2. **Star Citizen** installé (version 4.5 ou supérieure)

3. **Xbox Elite Series 2 Controller** connectée à votre PC

## 🔧 Installation étape par étape

### Étape 1 : Préparer reWASD

1. Ouvrir **reWASD**
2. S'assurer que la manette Xbox Elite S2 est détectée
3. Vérifier que reWASD est en mode "Advanced mapping" (nécessaire pour les shift layers)

### Étape 2 : Importer le profil reWASD

1. Dans reWASD, aller dans l'onglet **"Configs"**
2. Cliquer sur **"Import"** (ou utiliser le raccourci Ctrl+I)
3. Naviguer vers le fichier `VRCitizenXEliteS2-0.01.rewasd`
4. Sélectionner le fichier et cliquer sur **"Open"**
5. Le profil devrait apparaître dans la liste des configs
6. **Activer le profil** en cliquant dessus (il devrait être surligné)

### Étape 3 : Importer le profil Star Citizen

1. Localiser le dossier de configuration Star Citizen :
   ```
   StarCitizen\USER\Controls\Mappings\
   ```
   - Par défaut sur Windows : `C:\Users\[VotreNom]\AppData\Local\Star Citizen\USER\Controls\Mappings\`
   - Ou : `%LOCALAPPDATA%\Star Citizen\USER\Controls\Mappings\`

2. **Copier** le fichier `VRCitizenXEliteS2-0.01.xml` dans ce dossier

3. Ouvrir **Star Citizen**

4. Dans le jeu :
   - Aller dans **Options** → **Keybindings**
   - Cliquer sur **"Load Profile"** (ou "Charger un profil")
   - Sélectionner **"VRCitizenXEliteS2-0.01"**
   - Cliquer sur **"Load"** (ou "Charger")

5. **Sauvegarder** les keybinds :
   - Cliquer sur **"Save"** (ou "Enregistrer")
   - Confirmer que le profil est bien chargé

### Étape 4 : Vérifier la configuration

1. **Tester reWASD** :
   - Vérifier que le profil est bien actif (icône verte dans reWASD)
   - Tester quelques boutons pour confirmer que les mappings fonctionnent

2. **Tester dans Star Citizen** :
   - Tester les mouvements de base (joysticks)
   - Tester la sélection d'armes (D-pad)
   - Tester le mode interaction (Y hold)

## ⚠️ Variations par rapport à Couch Citizen

Cette configuration présente quelques différences importantes par rapport à Couch Citizen :

1. **Mobiglass et Vault inversés** :
   - La **Mobiglass** est mappée sur le **bouton Xbox** (bouton central de la manette)
   - Le **Vault** est mappé sur un autre bouton
   - Cette inversion est intentionnelle dans cette configuration

2. **Crouch et Prone en mode Toggle** :
   - Pour que le **Crouch** et le **Prone** fonctionnent correctement, il est **nécessaire** de les paramétrer en mode **Toggle** dans les paramètres du jeu
   - Dans Star Citizen : **Options** → **Keybindings** → Rechercher "Crouch" et "Prone"
   - Assurez-vous que ces actions sont configurées en **Toggle** (et non en Hold)

## ⚙️ Configuration avancée

### Ajuster la sensibilité

Si les contrôles sont trop sensibles ou pas assez :

1. Dans **reWASD** :
   - Aller dans les paramètres de la manette
   - Ajuster la sensibilité des joysticks
   - Ajuster la sensibilité de la souris (pour le mode interaction)

2. Dans **Star Citizen** :
   - Options → Keybindings → Advanced
   - Ajuster les sensibilités des axes

### Personnaliser les mappings

Si vous souhaitez modifier certains contrôles :

1. **Dans reWASD** :
   - Ouvrir le profil
   - Modifier les mappings selon vos préférences
   - Sauvegarder le profil

2. **Dans Star Citizen** :
   - Options → Keybindings
   - Modifier les keybinds directement dans le jeu
   - Sauvegarder le profil

⚠️ **Attention** : Modifier les keybinds dans Star Citizen peut créer des conflits avec reWASD. Il est recommandé de modifier uniquement dans reWASD.

## 🔄 Mise à jour

Pour mettre à jour vers une nouvelle version :

1. **Sauvegarder votre configuration actuelle** (si vous avez fait des modifications)
2. **Importer le nouveau profil reWASD** (remplacer l'ancien)
3. **Importer le nouveau profil XML** dans Star Citizen
4. **Charger le nouveau profil** dans Star Citizen

## 🐛 Dépannage

### reWASD ne détecte pas la manette

- Vérifier que la manette est bien connectée
- Redémarrer reWASD
- Vérifier les paramètres Windows (Paramètres → Périphériques → Périphériques Bluetooth et autres)

### Le profil reWASD ne se charge pas

- Vérifier que reWASD est à jour
- Vérifier que le fichier `.rewasd` n'est pas corrompu
- Essayer de réimporter le profil

### Les keybinds ne fonctionnent pas dans Star Citizen

- Vérifier que le profil XML est bien chargé dans Star Citizen
- Vérifier que reWASD est bien actif et que le profil est appliqué
- Redémarrer Star Citizen
- Vérifier qu'il n'y a pas de conflits avec d'autres logiciels (Steam, etc.)

### Le D-pad bouge le personnage au lieu de sélectionner les armes

- Vérifier que les "unmap" sont bien configurés dans reWASD
- Vérifier que le XML utilise `gp1_back multiTap="2"` pour les actions d'armes
- Voir la section "Dépannage" dans le README.md

## 📞 Support

Si vous rencontrez des problèmes :

1. Consulter la section "Dépannage" du README.md
2. Vérifier les issues existantes sur GitHub
3. Ouvrir une nouvelle issue avec :
   - Description du problème
   - Version de reWASD
   - Version de Star Citizen
   - Logs d'erreur (si disponibles)

---

**Note** : Cette configuration est testée avec Star Citizen 4.5. Des ajustements peuvent être nécessaires pour les versions futures.

