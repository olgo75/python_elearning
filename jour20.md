# Jour 20 : Scraper une page Wikipédia au choix

## Objectifs
- Savoir récupérer une page à partir d'une URL dynamique
- Extraire le premier paragraphe d'un article

## 1. Demander un sujet à l'utilisateur
```python
sujet = input("Sujet à rechercher sur Wikipédia : ")
```

## 2. Construire l'URL Wikipédia
```python
url = f"https://fr.wikipedia.org/wiki/{sujet.replace(' ', '_')}"
```

## 3. Extraire le premier paragraphe
```python
import requests
from bs4 import BeautifulSoup

reponse = requests.get(url)
soup = BeautifulSoup(reponse.text, "html.parser")
paragraphe = soup.find('p')
if paragraphe:
    print(paragraphe.text)
else:
    print("Aucun paragraphe trouvé.")
```

## Exercice du jour
- Demander à l'utilisateur un sujet, récupérer la page Wikipédia correspondante, et afficher le premier paragraphe. 