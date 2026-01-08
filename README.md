# VRCitizen X Elite S2

Configuration complète pour jouer à **Star Citizen** avec une manette Xbox Elite S2 via **reWASD**.

## 📋 Description

Cette configuration permet de jouer à Star Citizen avec une manette Xbox Elite S2 en utilisant reWASD pour mapper les boutons de la manette vers des touches clavier/souris. La configuration est optimisée pour offrir une expérience de jeu complète en mode FPS et en vol spatial.

## 🎮 Matériel requis

- **Manette** : Xbox Elite Series 2 Controller
- **Logiciel** : reWASD (version 6.x ou supérieure)
- **Jeu** : Star Citizen (version 4.5+)

## 📁 Structure du projet

```
VRCitizenXEliteS2/
├── README.md                          # Ce fichier
├── INSTALLATION.md                    # Guide d'installation détaillé
├── CONTROLS.md                        # Documentation complète des contrôles
├── CHANGELOG.md                       # Historique des versions
├── .gitignore                         # Fichiers à ignorer par Git
│
├── reWASD/
│   └── VRCitizenXEliteS2-0.01.rewasd  # Profil reWASD principal
│
└── StarCitizen/
    └── VRCitizenXEliteS2-0.01.xml     # Profil de keybinds Star Citizen
```

## 🚀 Installation rapide

1. **Installer reWASD** (si ce n'est pas déjà fait)
2. **Importer le profil reWASD** :
   - Ouvrir reWASD
   - Aller dans "Configs" → "Import"
   - Sélectionner `VRCitizenXEliteS2-0.01.rewasd`
3. **Importer le profil Star Citizen** :
   - Copier `VRCitizenXEliteS2-0.01.xml` dans le dossier Star Citizen
   - Chemin : `StarCitizen\USER\Controls\Mappings\`
   - Dans le jeu : Options → Keybindings → Load Profile → Sélectionner `VRCitizenXEliteS2-0.01`

Pour plus de détails, voir [INSTALLATION.md](INSTALLATION.md)

## 🎯 Fonctionnalités principales

### Mode FPS
- ✅ Sélection d'armes avec D-pad (Up/Down/Left/Right)
- ✅ Crouch/Prone avec paddle gauche bas
- ✅ Saut avec paddle droite bas
- ✅ Arme de mêlée avec LB + D-pad Right
- ✅ Mode interaction avec Y (hold) et Back (hold)

### Mode Vol spatial
- ✅ Contrôles de vol complets
- ✅ Landing gear avec D-pad Down (double tap)
- ✅ Demande d'atterrissage avec LB + Y
- ✅ Sortie de siège avec LB + hold B

### Autres fonctionnalités
- ✅ Wheel menu (roue de pensée) avec LB + Y
- ✅ Auto-run avec RB (long) + X (long)
- ✅ Mode souris pour navigation hangar

## 📖 Documentation

- **[INSTALLATION.md](INSTALLATION.md)** : Guide d'installation détaillé
- **[CONTROLS.md](CONTROLS.md)** : Documentation complète de tous les contrôles
- **[CHANGELOG.md](CHANGELOG.md)** : Historique des modifications

## 🔧 Configuration

### reWASD
- **Émulation clavier** : Utilise autant que possible l'émulation de touches clavier
- **D-pad** : Émule des touches clavier (DIK_5, DIK_3, etc.) pour éviter les conflits
- **Modificateurs** : LB active shiftId 1 sans délai

### Star Citizen
- **Unmap gamepad** : Utilise `gp1_back multiTap="2"` pour corriger un bug Star Citizen
- **Touches clavier** : Les actions utilisent les touches clavier émulées par reWASD

## 🐛 Dépannage

### Le D-pad bouge le personnage
- Vérifier que les "unmap" sont bien configurés dans reWASD
- Vérifier que le XML utilise `gp1_back multiTap="2"` pour les actions d'armes

### La sortie de siège ne fonctionne pas
- Maintenir LB + B (hold), pas juste un tap
- Vérifier que le profil reWASD est bien chargé

### Les armes ne se chargent pas
- Vérifier que reWASD envoie bien les touches clavier (DIK_5, DIK_3, etc.)
- Vérifier que le XML a les bonnes mappings avec `gp1_back multiTap="2"`

## 📝 Versions

- **0.01** : Version initiale basée sur CouchCitizen 3.22 WIP44, testée sur Star Citizen 4.5

## 🤝 Contribution

Les contributions sont les bienvenues ! N'hésitez pas à ouvrir une issue ou une pull request.

## 📄 Licence

[À définir]

## 🙏 Remerciements

- Basé sur la configuration **CouchCitizen 3.22**
Vous pouvez utilisez les videos de Couc citizen pour voir la ocnfig : https://www.youtube.com/watch?v=9gPdLI2DewE&list=PL0hxs6q3ACPYAgRk447fqnGkYp4D6v-Sp

---

**Note** : Cette configuration est testée sur Star Citizen 4.5. Des ajustements peuvent être nécessaires pour les versions futures du jeu.

