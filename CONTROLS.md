# Documentation des contrôles - VRCitizen X Elite S2

Documentation complète de tous les contrôles disponibles dans cette configuration.

## 🎮 Légende

- **LB** : Left Bumper (Bumper gauche)
- **RB** : Right Bumper (Bumper droit)
- **LT** : Left Trigger (Gâchette gauche)
- **RT** : Right Trigger (Gâchette droite)
- **LS** : Left Stick (Joystick gauche)
- **RS** : Right Stick (Joystick droit)
- **Paddle** : Paddle arrière (gauche ou droite, haut ou bas)

## 🚶 Mode FPS (à pied)

### Mouvement

| Contrôle | Action |
|----------|--------|
| **LS** | Déplacement (avant/arrière/gauche/droite) |
| **RS** | Rotation de la caméra |
| **Paddle droite bas** | Saut (hold) |
| **Paddle gauche bas** (simple tap) | Crouch (toggle) |
| **Paddle gauche bas** (double tap) | Prone (toggle) |

### Sélection d'armes

| Contrôle | Action |
|----------|--------|
| **D-pad Up** | Armes de mêlée (poings) |
| **D-pad Down** | Gadget utilitaire |
| **D-pad Left** | Arme principale |
| **D-pad Right** | Arme secondaire (pistolet) |
| **LB + D-pad Right** | Arme de mêlée (couteau) |

### Interaction

| Contrôle | Action |
|----------|--------|
| **Y (hold)** | Mode interaction (maintenir) |
| **Back (hold)** | Mode interaction souris (maintenir) |
| **RT** (en mode interaction) | Clic gauche souris |
| **LT** (en mode interaction) | Clic gauche souris |
| **RB** (en mode interaction) | Scroll up |
| **LB** (en mode interaction) | Scroll down |
| **Back (double tap)** (en mode interaction) | Clic gauche souris |

### Autres actions FPS

| Contrôle | Action |
|----------|--------|
| **X** | Recharger / Ranger arme / Quantum Travel |
| **A** | Interagir / Utiliser |
| **B** | Annuler / Retour |
| **Y (long press)** | Toggle mode interaction |
| **RB (long) + X (long)** | Toggle auto-run |

## 🚀 Mode Vol spatial

### Contrôles de vol

| Contrôle | Action |
|----------|--------|
| **LS** | Pitch / Roll |
| **RS** | Yaw / Strafe |
| **LT** | Frein |
| **RT** | Accélération |
| **Paddle droite haut** | Strafe up |
| **Paddle droite bas** | Strafe down |
| **Paddle gauche haut** | Strafe left |
| **Paddle gauche bas** | Strafe right |

### Navigation et systèmes

| Contrôle | Action |
|----------|--------|
| **D-pad Down** (simple tap) | Toggle landing gear |
| **D-pad Down** (double tap) | Toggle landing gear |
| **D-pad Down** (long press) | Auto-land |
| **LB + Y** | Demande d'atterrissage / Wheel menu (F9) |
| **LB + B** (hold) | Sortir du siège |
| **LB + B** (tap) | Décliner les prompts (]) |
| **LB + X** | [Action spécifique] |
| **LB + A** | [Action spécifique] |

### Autres actions vol

| Contrôle | Action |
|----------|--------|
| **X** | Quantum Travel |
| **Y** | [Action spécifique] |
| **A** | [Action spécifique] |
| **B** | [Action spécifique] |

## 🎯 Modificateurs

### LB (Left Bumper) - Modificateur principal

Le LB active le **shiftId 1** dans reWASD. Il permet d'accéder à des actions secondaires :

- **LB + Y** : Wheel menu (F9) / Demande d'atterrissage
- **LB + B** : Sortir du siège (hold) / Décliner prompts (tap)
- **LB + D-pad Right** : Arme de mêlée
- **LB + [Autres boutons]** : Actions spécifiques

### RB (Right Bumper) - Modificateur secondaire

Le RB active le **shiftId 4** dans reWASD pour certaines actions :

- **RB (long) + X (long)** : Toggle auto-run

## 🖱️ Mode Interaction

### Back (hold) - Mode interaction souris

Quand **Back** est maintenu :
- Active le mode interaction (F)
- Active le layer 1 dans reWASD (mode souris)
- **RS** contrôle le curseur souris
- **RT** = Clic gauche souris
- **LT** = Clic gauche souris
- **RB** = Scroll up
- **LB** = Scroll down

### Y (hold) - Mode interaction cockpit

Quand **Y** est maintenu :
- Active le mode interaction (F)
- Active le layer 2 dans reWASD
- **RS** contrôle le curseur souris
- **RT** = Clic gauche souris (pour interaction cockpit)
- **LT** = Clic gauche souris
- **RB** = Scroll up
- **LB** = Scroll down
- **Back (double tap)** = Clic gauche souris

## 📋 Actions spéciales

### Wheel Menu (Roue de pensée)

- **LB + Y** : Ouvre le wheel menu (F9)

### Auto-run

- **RB (long) + X (long)** : Toggle auto-run/walk

### Sortie de siège

- **LB + B (hold)** : Sortir du siège
- **LB + B (tap)** : Décliner les prompts

## 🔧 Notes techniques

### D-pad et armes

- Le D-pad émet des touches clavier (DIK_5, DIK_3, etc.) via reWASD
- Les signaux gamepad sont "unmapped" au niveau de base pour éviter les conflits
- Le XML utilise `gp1_back multiTap="2"` pour corriger un bug Star Citizen

### Mode interaction

- Le mode interaction utilise F (DIK_F) maintenu
- Les clics souris sont utilisés pour `pc_interaction_select`
- Le mode reste actif tant que le bouton est maintenu

### Modificateurs

- LB active shiftId 1 sans délai
- Les modificateurs restent actifs tant que le bouton est maintenu
- Pas de délai d'activation pour éviter les problèmes de timing

## 📝 Raccourcis clavier émulés

| Touche | Action Star Citizen |
|--------|---------------------|
| **F** | Mode interaction |
| **F9** | Wheel menu (roue de pensée) |
| **5** | Sélectionner gadget |
| **3** | Sélectionner pistolet |
| **1** | Sélectionner arme principale |
| **6** | Sélectionner poings |
| **V** | Sélectionner arme de mêlée |
| **]** | Décliner prompts |
| **Space** | Saut |
| **Ctrl** | Crouch (toggle) |
| **M** | Prone (toggle) |

---

**Note** : Cette documentation est basée sur la version 0.01, testée sur Star Citizen 4.5. Certaines actions peuvent varier selon les versions futures du jeu.

