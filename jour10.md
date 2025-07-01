# Jour 10 : Les chaînes de caractères (méthodes)

## Objectifs
- Découvrir les méthodes utiles sur les chaînes

## 1. Quelques méthodes utiles
- `lower()` : tout en minuscules
- `upper()` : tout en majuscules
- `split()` : découper en mots
- `replace()` : remplacer un mot

Exemple :
```python
phrase = "Bonjour le monde"
print(phrase.upper())
print(phrase.split())
```

## 2. Compter les mots d'une phrase
```python
texte = input("Écris une phrase : ")
nombre_de_mots = len(texte.split())
print("Nombre de mots :", nombre_de_mots)
```

## Exercice du jour
- Demander une phrase à l'utilisateur et afficher le nombre de mots. 