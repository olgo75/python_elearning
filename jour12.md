# Jour 12 : Les exceptions (try/except)

## Objectifs
- Comprendre la gestion des erreurs

## 1. try/except
Permet d’éviter que le programme plante en cas d’erreur.

Exemple :
```python
try:
    nombre = int(input("Entrez un nombre : "))
    print("Le double est", nombre * 2)
except ValueError:
    print("Ce n’est pas un nombre valide.")
```

## Exercice du jour
- Demander un nombre à l’utilisateur et gérer l’erreur si ce n’est pas un nombre. 