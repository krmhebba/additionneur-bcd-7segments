# Additionneur BCD & Afficheur 7 Segments (FPGA)

## Description
Ce projet est une conception matérielle réalisée sur Quartus II pour un FPGA Altera Cyclone III. Il s'agit d'un circuit logique capable de réaliser l'addition de nombres et d'afficher le résultat décimal sur un afficheur 7 segments.

Le projet combine deux méthodes de conception numérique :
1.  **Conception Schématique (.bdf) :** Pour l'architecture globale et l'interconnexion des blocs logiques (Additionneurs, Logique combinatoire).
2.  **Langage AHDL (.tdf) :** Pour la programmation comportementale du décodeur 7 segments (Table de vérité convertissant le binaire en signaux d'affichage a-g).

## Fonctionnalités
* **Addition BCD :** Calcul de la somme de deux entrées binaires.
* **Décodage 7 Segments :** Conversion du résultat binaire en format lisible pour l'afficheur (Segments a, b, c, d, e, f, g).
* **Simulation Temporelle :** Validation du fonctionnement logique via des chronogrammes (Waveforms) pour vérifier les états des sorties en fonction des entrées.

## Architecture Technique
* **Matériel Cible :** FPGA Altera Cyclone III (EP3C16F484C6).
* **Environnement de Développement :** Quartus II 9.1.
* **Top-Level Entity :** `Blockdecodeur`.
* **Composants Clés :**
    * `Ahdl1.tdf` : Logique de table de vérité pour le pilotage des segments.
    * `Block1` & `Block2` : Blocs logiques intermédiaires pour le traitement des signaux.

## Fichiers du Dépôt
* **Sources :** Fichiers schématiques (.bdf) et code AHDL (.tdf).
* **Simulation :** Fichiers Vector Waveform (.vwf) montrant les tests unitaires.
* **Configuration :** Fichier Pinout (.pin) détaillant l'assignation des broches physiques du FPGA.

## Installation et Ouverture
1. Cloner le dépôt.
2. Ouvrir le fichier `exo1.qpf` avec le logiciel Quartus II.
3. Lancer la compilation pour vérifier la synthèse logique.
4. Ouvrir les fichiers `.vwf` pour visualiser les simulations.

## Auteurs
Projet réalisé Hiba Karam en collaboration avec Tarek Souibri - Élèves Ingénieurs @ EMSI.
