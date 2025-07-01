# Jour 21 : Mini-projet scraping Wikipédia

## Objectifs
- Structurer un script de scraping complet
- Sauvegarder les résultats dans un fichier texte

## 1. Demander un sujet à l'utilisateur
```python
sujet = input("Sujet à rechercher sur Wikipédia : ")
```

## 2. Récupérer la page et extraire les infos
```python
import requests
from bs4 import BeautifulSoup

url = f"https://fr.wikipedia.org/wiki/{sujet.replace(' ', '_')}"
try:
    reponse = requests.get(url)
    reponse.raise_for_status()
    soup = BeautifulSoup(reponse.text, "html.parser")
    titre = soup.title.string if soup.title else "Pas de titre"
    paragraphe = soup.find('p')
    texte = paragraphe.text if paragraphe else "Pas de paragraphe trouvé."
except Exception as e:
    titre = "Erreur"
    texte = str(e)
```

## 3. Sauvegarder dans un fichier
```python
with open("resultat_wikipedia.txt", "w", encoding="utf-8") as f:
    f.write(f"Titre : {titre}\n\n{texte}")
```

## Exercice du jour
- Écrire un programme qui demande un sujet, récupère le titre et le premier paragraphe de la page Wikipédia, et les enregistre dans un fichier. 