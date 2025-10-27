

# Filtrage particulaire – Suivi d’objet simple

### English version below

## Description du projet

Ce projet présente une implémentation complète d’un **filtrage particulaire (Particle Filter)** appliqué au **suivi d’un objet en mouvement**.
L’objectif est de comprendre et d’illustrer comment une approche probabiliste permet d’estimer la position d’un objet incertaine dans le temps, à partir de mesures bruitées.

Le notebook combine **modélisation du mouvement**, **simulation des mesures**, **rééchantillonnage** et **visualisation dynamique** des particules et de la trajectoire estimée.

---

## Objectifs pédagogiques

* Comprendre les principes du **filtrage particulaire**.
* Mettre en œuvre un algorithme de suivi à base de **particules pondérées**.
* Visualiser l’évolution de la **distribution de probabilité** dans le temps.
* Comparer le filtrage particulaire à d’autres approches (Kalman, moyenne glissante, etc.).

---

## Structure du projet

1. **Introduction théorique**

   * Rappel sur les méthodes bayésiennes et la notion de probabilité conditionnelle.
   * Présentation du filtrage particulaire et des étapes clés : prédiction, mise à jour, rééchantillonnage.

2. **Modélisation du problème**

   * Définition du modèle d’état (position, vitesse).
   * Modélisation du bruit de mesure et du bruit de mouvement.
   * Génération de trajectoires simulées.

3. **Implémentation du filtre particulaire**

   * Initialisation des particules.
   * Étape de prédiction (propagation).
   * Calcul des poids selon les observations.
   * Rééchantillonnage des particules.

4. **Visualisation des résultats**

   * Affichage de la position réelle, estimée et des particules.
   * Animation de la convergence du filtre dans le temps.

5. **Analyse et discussion**

   * Étude des effets du nombre de particules, du bruit ou du modèle de mouvement.
   * Comparaison des performances avec un filtre de Kalman simple.

---

## Contenu du dépôt

* `particle_filter.ipynb` — Notebook principal contenant l’implémentation complète.
* `escrime-4-3.avi` 
* `README.md` — Présentation du projet.

---

## Résultats attendus

Le filtre particulaire doit :

* suivre correctement l’objet malgré le bruit,
* maintenir une estimation stable et cohérente,
* converger vers la vraie position au fil du temps.

---

## Auteur

Projet réalisé dans le cadre d’un **travail pratique sur les filtres bayésiens**.
Auteur : **Kadidiatou Diallo** – ENSEA

---

# English version

## Project Description

This project presents a full implementation of a **Particle Filter** applied to **simple object tracking**.
The main goal is to illustrate how probabilistic reasoning can estimate an object’s position over time under uncertainty and noisy measurements.

The notebook integrates **motion modeling**, **measurement simulation**, **resampling**, and **dynamic visualization** of particles and estimated trajectories.

---

## Learning Objectives

* Understand the principles of **particle filtering**.
* Implement an algorithm based on **weighted particles** for object tracking.
* Visualize the evolution of the **probability distribution** over time.
* Compare particle filtering with other approaches (Kalman filter, moving average, etc.).

---

## Project Structure

1. **Theoretical Introduction**

   * Overview of Bayesian filtering and conditional probability.
   * Presentation of the particle filter algorithm: prediction, update, and resampling.

2. **Problem Modeling**

   * Definition of the state-space model (position, velocity).
   * Modeling of process and measurement noise.
   * Generation of simulated trajectories.

3. **Implementation of the Particle Filter**

   * Particle initialization.
   * Prediction step (motion propagation).
   * Weight computation based on observations.
   * Particle resampling procedure.

4. **Results Visualization**

   * Plot of true vs estimated positions and particle clouds.
   * Animation showing convergence over time.

5. **Analysis and Discussion**

   * Effect of the number of particles, noise, and motion model.
   * Comparison with a simple Kalman filter baseline.

---

## Repository Content

* `particle_filter.ipynb` — Main notebook containing the full implementation.
* `escrime-4-3.avi` 
* `README.md` — Project overview and documentation.

---


## Expected Results

The particle filter should:

* accurately track the object despite noise,
* maintain a stable estimation,
* and converge toward the true position over time.

---

## Author

Project completed as part of a **Bayesian filtering lab**.
Author: **Kadidiatou Diallo** – ENSEA 

