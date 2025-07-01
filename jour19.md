# Jour 19 : Gérer les erreurs et les cas particuliers

## Objectifs
- Savoir gérer les erreurs réseau et HTTP
- Vérifier la présence d'éléments dans la page

## 1. Gérer les erreurs réseau
```python
import requests
try:
    reponse = requests.get(url)
    reponse.raise_for_status()  # Lève une exception si erreur HTTP
except requests.exceptions.RequestException as e:
    print("Erreur réseau ou HTTP :", e)
```

## 2. Vérifier le code de retour HTTP
```python
if reponse.status_code == 200:
    print("Succès !")
else:
    print("Erreur :", reponse.status_code)
```

## 3. Gérer l'absence d'éléments
```python
titre = soup.title.string if soup.title else "Pas de titre trouvé"
```

## Exercice du jour
- Écrire un script qui récupère le titre d'une page Wikipédia, et affiche un message d'erreur si la page n'existe pas. 