# 🐉 Projet Donjons & Dragons

Une application Java en console pour simuler un jeu de rôle inspiré de **Donjons & Dragons**, mettant en scène des personnages combattant des monstres à travers plusieurs donjons.

## 🔥 Présentation
Le Projet **Donjons & Dragon** modélise un jeu de rôle de **Medieval Fantasy** simplifié, se jouant au tour par tour. L'objectif pour l'équipe de joueurs est d'éliminer tous les monstres de tous les donjons successifs afin d'en terminer le plus possible.

**Règles Clés :**
* **Victoire/Défaite :** L'équipe gagne si tous les monstres sont vaincus. L'équipe perd si un seul personnage est éliminé.
* **Tour par Tour :** L'ordre des tours est déterminé par un jet d'**Initiative** au début de chaque donjon.
* **Actions :** Les personnages et les monstres peuvent effectuer jusqu'à 3 actions par tour (attaquer, se déplacer, s'équiper, ramasser un équipement).
* **Jets de Dés :** Toutes les actions de combat (attaque et dégâts) se basent sur des jets de dés.

## 🧑‍🤝‍🧑 Les Personnages
Chaque personnage est défini par sa **Race** (Humain, Nain, Elfe, Halfelin) et sa **Classe** (Guerrier, Clerc, Magicien, Roublard), qui influencent ses caractéristiques de base.

| Caractéristique | Description | Utilisation |
| :---: | :---: | :---: |
| **Points de Vie** | Dégâts max avant de mourir. | Déterminés par la classe. |
| **Force** | Bonus pour les attaques au corps-à-corps. | Jet d'attaque (corps-à-corps). |
| **Dextérité** | Bonus pour les attaques à distance. | Jet d'attaque (à distance). |
| **Vitesse** | Distance de déplacement max par action. | Déplacement (distance $/ 3$). |
| **Initiative** | Bonus pour l'ordre de jeu. | Ordre des tours (jet de $1\text{d}20$ + Initiative). |

## 🛡️ Les Équipements
Les personnages gèrent un inventaire d'armes et d'armures, et peuvent équiper une seule arme et une seule armure.
* Les **Armures** (légères ou lourdes) définissent la **Classe d'Armure** (CA) de la cible.
* Les **Armes** définissent les dés de dégâts et la portée. Certaines armes et armures imposent des malus de **Vitesse** ou des bonus de **Force**.

## 👾 Les Monstres
Les monstres sont définis par leur espèce, leurs caractéristiques (PV, Vitesse, Force/Dextérité, CA, Initiative) et une attaque unique (portée et dégâts).

---

## 🧠 Fonctionnalités
* **Simulation de Combat :** Gestion des jets d'attaque ($1\text{d}20$ + caractéristique vs. Classe d'Armure) et des dégâts.
* **Gestion de Donjon :** Création et affichage d'une carte rectangulaire avec des obstacles et des équipements à ramasser.
* **Gestion de Personnages :** Création de personnages avec les règles de race et de classe. Gestion de l'inventaire et des équipements portés.
* **Séquencement des Tours :** Ordre des tours basé sur l'initiative.
* **Role Play :** Possibilité pour les joueurs et le Maître du Jeu de commenter les actions.
* **Interface Console :** Affichage clair et structuré des statistiques et de la carte du donjon.

---

## 🏗️ Architecture & technologies
* **Langage :** Java
* **Environnement :** Application console
* **IDE recommandé :** IntelliJ IDEA

---

## ⚙️ Installation & configuration
### 1. Prérequis
 * Java Development Kit (**JDK**) installé (version 17 ou supérieure recommandée).
 * Un IDE ou un environnement capable de compiler et d'exécuter du code Java.

### 2. Cloner le dépôt
 ```git
 git clone https://github.com/PanDox42/textgame-donjons-et-dragons
 ```

### 3. Lancer l'application
 * Compilez les sources situées dans le dossier `src/`.
 * Exécutez la classe principale `Main.java`.
