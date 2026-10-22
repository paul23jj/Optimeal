optimeal
├── data/
│   ├── raw/                  # Fichiers bruts (lecture seule)
│   └── processed/            # CSV nettoyé et fusionné (la table pivot)
│
├── notebooks/                # Pour tester et explorer
│   └── 01_eda_donnees.ipynb
│
├── src/                      # Code source réutilisable
│   ├── data_loader.py        # Téléchargement, nettoyage et jointures
│   ├── features.py           # Encodage, lags temporels, variables météo
│   └── train.py              # Entraînement du modèle et export (.joblib)
│
├── models/
│   └── model.joblib          # Le modèle entraîné sauvegardé
│
├── api/                      # Backend d'inférence
│   └── main.py               # Routes FastAPI (/health, /predict)
│
├── app/                      # Frontend / Dashboard
│   ├── dashboard.py          # Interface Streamlit
│   └── style.css             # (Optionnel) Quelques retouches CSS propres
│
├── .gitignore
├── requirements.txt
└── README.md