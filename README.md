# Prédiction des cas confirmés d'Ebola en RDC

##  Description
Application de prédiction des cas confirmés d'une epidemie basée sur un modèle de régression linéaire multiple utilisant des données épidémiologiques et environnementales.

##  Fonctionnalités
- Prédiction en temps réel des cas confirmés
- Interface utilisateur intuitive avec Streamlit
- Visualisation des données d'entrée
- Interprétation des résultats

## Variables utilisées
| Variable | Description |
|----------|-------------|
| Cas suspects | Nombre de cas suspects signalés |
| Pluviométrie | Précipitations en mm |
| Température | Température moyenne en °C |
| Déforestation | Surface déforestée en ha |
| NDVI | Indice de végétation |

## Installation

### Prérequis
- Python 3.8 ou supérieur
- Git

### Étapes d'installation
```bash
# 1. Cloner le dépôt
git clone https://github.com/SylvieMpwek/Projet_final.git  
cd Epi_regression

# 2. Créer un environnement virtuel
python -m venv venv
source venv/bin/activate  # Sur Windows: venv\Scripts\activate

# 3. Installer les dépendances
pip install -r requirements.txt

# 4. Entraîner le modèle
python train_model.py

# 5. Lancer l'application
streamlit run app.py