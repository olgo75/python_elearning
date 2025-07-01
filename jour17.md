# Jour 17 : Introduction au parsing HTML avec BeautifulSoup

## Objectifs
- Savoir installer et importer BeautifulSoup
- Extraire des éléments HTML d'une page

## 1. Installer BeautifulSoup
```bash
pip install beautifulsoup4
```

## 2. Importer BeautifulSoup
```python
from bs4 import BeautifulSoup
```

## 3. Extraire des éléments HTML
Exemple : extraire le titre d'une page Wikipédia
```python
import requests
from bs4 import BeautifulSoup

url = "https://fr.wikipedia.org/wiki/Accueil"
reponse = requests.get(url)
soup = BeautifulSoup(reponse.text, "html.parser")
titre = soup.title.string
print(titre)
```

## Exercice du jour
- Extraire et afficher le titre de la page Wikipédia d'accueil. 