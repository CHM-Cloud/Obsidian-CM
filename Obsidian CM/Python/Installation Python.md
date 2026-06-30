
Telecharger le program

dans windows taper la commande CMD

Visual studio code : https://code.visualstudio.com/

puis : pip install yfinance

https://www.geeksforgeeks.org/how-to-install-yfinance-with-python-pip/

- Matplotlib releases are available as wheel packages for macOS, Windows and Linux on [PyPI](https://pypi.org/project/matplotlib/). Install it using `pip`:

python -m pip install -U pip
python -m pip install -U matplotlib

- sklearn
python -m pip install scikit-learn
python -m venv sklearn-env
sklearn-env\Scripts\activate  # activate
pip install -U scikit-learn

python -m pip install openpyxl


***************
import yfinance as yf

# Exemple : Télécharger les données pour Tesla (TSLA)
data = yf.download("TSLA", start="2023-01-01", end="2023-12-31", interval="1d")

# Enregistrer dans un fichier CSV
data.to_csv("Tesla_data.csv")
print("Données téléchargées avec succès !")

****************************

import yfinance as yf

# Exemple : télécharger les données historiques de l'action Apple (AAPL)
stock = yf.Ticker("AAPL")
data = stock.history(period="1y")  # Par exemple, pour obtenir 1 an de données

# Sauvegarder les données dans un fichier CSV
data.to_csv("AAPL_historical_data.csv")
