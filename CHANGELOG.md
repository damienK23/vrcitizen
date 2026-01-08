# Changelog - VRCitizen X Elite S2

Toutes les modifications notables de ce projet seront documentées dans ce fichier.

Le format est basé sur [Keep a Changelog](https://keepachangelog.com/fr/1.0.0/),
et ce projet adhère au [Semantic Versioning](https://semver.org/lang/fr/).

## [0.01] - 2025-01-07

### Ajouté
- Configuration initiale basée sur CouchCitizen 3.22 WIP44
- Testée et validée sur Star Citizen 4.5
- Profil reWASD complet pour Xbox Elite Series 2
- Profil Star Citizen XML avec tous les keybinds
- Documentation complète (README, INSTALLATION, CONTROLS)

### Fonctionnalités FPS
- Sélection d'armes avec D-pad (Up/Down/Left/Right)
- Crouch/Prone avec paddle gauche bas (simple tap / double tap)
- Saut avec paddle droite bas
- Arme de mêlée avec LB + D-pad Right
- Mode interaction avec Y (hold) et Back (hold)

### Fonctionnalités Vol spatial
- Contrôles de vol complets (pitch, roll, yaw, strafe)
- Landing gear avec D-pad Down (double tap)
- Demande d'atterrissage avec LB + Y
- Sortie de siège avec LB + hold B
- Auto-land avec D-pad Down (long press)

### Autres fonctionnalités
- Wheel menu (roue de pensée) avec LB + Y
- Auto-run avec RB (long) + X (long)
- Mode souris pour navigation hangar
- Mode interaction cockpit optimisé

### Technique
- Émulation clavier via reWASD (DIK_5, DIK_3, etc.)
- Unmap D-pad au niveau de base pour éviter conflits mouvement
- Utilisation de `gp1_back multiTap="2"` pour corriger bug Star Citizen
- Shift layers optimisés (shiftId 1, 2, 4)
- Layer switching pour mode interaction (layer 1, 2)

### Documentation
- README.md avec vue d'ensemble du projet
- INSTALLATION.md avec guide d'installation détaillé
- CONTROLS.md avec documentation complète des contrôles
- CHANGELOG.md pour suivre les versions

---

## Historique (basé sur CouchCitizen 3.22)

### WIP29 (Version fonctionnelle de base)
- Configuration fonctionnelle complète
- CROUCH, PRONE, JUMP opérationnels
- D-pad armes fonctionnel
- Mode interaction Back et Y

### WIP30-WIP44 (Évolutions)
- Correction D-pad : gamepad → touches clavier
- Unmap D-pad au niveau de base
- Mode interaction Y : activation layer 2
- Interaction cockpit : clic souris au lieu de F
- Wheel menu : LB + Y
- LB + B : EXIT SEAT (hold) + DECLINE PROMPTS (tap)
- Optimisations diverses

---

**Note** : Pour plus de détails sur les versions précédentes (WIP29-WIP44), voir les changelogs individuels dans le dossier `CouchCitizen3.22/REWASD PROFILES/`.

