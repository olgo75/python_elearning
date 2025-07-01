# Jour 16 : Les requêtes HTTP avec requests

## Objectifs
- Comprendre ce qu'est une requête HTTP
- Savoir utiliser la bibliothèque requests pour récupérer une page web

## 1. Qu'est-ce qu'une requête HTTP ?
C'est une demande envoyée à un serveur web pour obtenir une ressource (page, image, etc.).

## 2. Installer requests
Si ce n'est pas déjà fait :
```bash
pip install requests
```

## 3. Faire une requête GET
Exemple pour récupérer la page d'accueil de Wikipédia :
```python
import requests

url = "https://fr.wikipedia.org/wiki/Accueil"
reponse = requests.get(url)
print(reponse.text)  # Affiche le code HTML de la page
```

## 4. Lire le contenu d'une réponse
- `reponse.text` : contenu en texte (HTML)
- `reponse.status_code` : code de retour (200 = OK)

## Exercice du jour
- Récupérer le code HTML de la page d'accueil de Wikipédia et l'afficher. 