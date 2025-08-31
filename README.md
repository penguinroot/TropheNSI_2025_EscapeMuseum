# 🎮 Projet Escape Game avec Ursina et SQLite

## 📌 Description

Ce projet est un jeu d'escape game interactif utilisant le moteur graphique **Ursina** et une base de données **SQLite** pour gérer les scores. Le jeu propose deux modes :

- **SpeedRun** : Terminer le jeu le plus rapidement possible.
- **Exploration** : Explorer librement sans limite de temps.

Un **leaderboard** est inclus pour afficher les meilleurs scores enregistrés.

## 🛠️ Installation

### 🔹 Prérequis

- **Python 3.12.9** spécifiquement

### 🔹 Installation des dépendances

Installe les dépendances nécessaires en exécutant la commande suivante dans le terminal :

```bash
pip install -r requirements.txt
```

## 🚀 Lancement du jeu

Pour démarrer le jeu, exécute la commande suivante dans le répertoire principal du projet(/EscapeMuseum et non pas /EscapeMuseum/sources) :

```bash
python sources/main.py
```

Assure-toi que tous les fichiers nécessaires (comme `musee.db` et les assets) sont présents dans leurs répertoires respectifs.

## 🏛️ Structure du projet

```plaintext
EscapeMuseum/
├── assets/  # Tous les assets graphiques et sonores
│   ├── image/  # Images diverses (interfaces, etc.)
│   │   ├── ascenseur.jpg
│   │   ├── commandes.png
│   │   ├── Escape.png
│   │   ├── ligne_droite.png
│   │   ├── ligne_haut.png
│   │   ├── menu.png
│   │   ├── regles.png
│   ├── minimap/  # Cartes miniatures
│   │   ├── grid.png
│   │   ├── grid_etage2.png
│   ├── models/  # Modèles 3D et textures
│   │   ├── banc.blend/.glb/.obj
│   │   ├── etage1.blend/.glb/.obj
│   │   ├── etage2.blend/.glb/.obj
│   │   ├── marble.jpg
│   │   ├── mur(bon).jpg
│   │   ├── pasmal.blend
│   │   ├── plafond.jpg
│   │   ├── woodfloor.png
│   ├── musique/  # Fichiers audio
│   │   ├── bruit_pas.mp3
│   │   ├── clique.mp3
│   │   ├── exploration.mp3
│   │   ├── menu.mp3
│   │   ├── saut.mp3
│   │   ├── speedrun.mp3
│   ├── oeuvre/  # Œuvres d'art (images)
│   │   ├── allegoriedeloccasion.jpg
│   │   ├── americangothic.jpg
│   │   ├── guernica.jpg
│   │   ├── la_joconde.jpg
│   │   ├── le_baiser.jpg
│   │   ├── ... (toutes les autres œuvres)
├── polices/  # Polices d'écriture
│   ├── Poppins-Bold.ttf
├── data/  # Données du jeu
│   ├── musee.db  # Base de données SQLite
│   ├── oeuvres.json  # Données des œuvres
├── sources/  # Code source Python
│   ├── artwork.py  # Gestion des œuvres
│   ├── exploration.py  # Mode exploration
│   ├── main.py  # Point d'entrée principal
│   ├── speedrun.py  # Mode speedrun
├── EscapeMuseum.md  # Documentation
├── licence.txt  # Licence du projet
├── presentation.pdf  # Présentation du projet
├── requirements.txt  # Dépendances Python
````
## 🎮 Commandes du jeu

- **ZQSD / Flèches** : Se déplacer
- **Espace** : Interagir
- **Échap** : Retour au menu
- **Clic sur l'ascenseur** : Changer d'étage

## 📊 Fonctionnalités principales

- 🎮 Modes **SpeedRun** et **Exploration**
- 🏆 Gestion d’un **leaderboard** (meilleurs scores enregistrés en SQLite)
- 🎵 **Musique dynamique** dans le menu et les niveaux
- 🎨 Interface utilisateur optimisée avec Ursina

## 📜 Licence

Ce projet est sous licence GPL v3+.
