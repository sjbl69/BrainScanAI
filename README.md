# BrainScanAI

Projet de Computer Vision appliqué à l’analyse d’IRM cérébrales pour la détection de tumeurs, utilisant des méthodes de deep learning et d’apprentissage semi-supervisé.

---

## Objectif

L’objectif du projet est d’explorer un dataset d’images médicales et de :

* analyser et comprendre les données (EDA)
* extraire des caractéristiques visuelles avec un modèle pré-entraîné
* appliquer des méthodes de clustering
* exploiter des données partiellement labellisées (semi-supervisé)

---

## Dataset

Le dataset contient **1506 images de cerveau**, réparties comme suit :

### Images labellisées :

* 50 images cancer
* 50 images normal

### Images non labellisées :

* 1406 images

---

## Structure des données

```
data/raw/mri_dataset_brain_cancer_oc/
├── avec_labels/
│   ├── cancer/
│   └── normal/
└── sans_label/
```

 Les données ne sont pas incluses dans ce dépôt (taille trop importante).

---

## Installation

### 1. Cloner le projet

```
git clone https://github.com/sjbl69/BrainScanAI.git
cd BrainScanAI
```

### 2. Créer un environnement virtuel

```
python -m venv venv
venv\Scripts\activate
```

### 3. Installer les dépendances

```
pip install -r requirements.txt
```

---

## Utilisation

### 1. Télécharger le dataset

Placer les données dans :

```
data/raw/mri_dataset_brain_cancer_oc/
```

---

### 2. Lancer les notebooks dans l’ordre :

```
notebooks/01_EDA.ipynb  
notebooks/02_Feature_Extraction.ipynb  
notebooks/04_SemiSupervised.ipynb
```

 Le clustering est directement intégré dans le notebook **04_SemiSupervised.ipynb**.

---

## Étape 1 - Analyse exploratoire (EDA)

* Exploration du dataset
* Visualisation des images
* Analyse des dimensions et du format
* Étude de la structure des données (labellisé / non labellisé)

---

## Technologies utilisées

* Python
* PyTorch
* torchvision
* NumPy
* pandas
* matplotlib
* scikit-learn

---

## Méthodes utilisées

* Feature extraction avec ResNet
* Clustering (K-Means)
* Apprentissage semi-supervisé

---

## Auteur

Selma JBILOU

