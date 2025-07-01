# Jour 11 : Les fichiers (lecture/écriture)

## Objectifs
- Savoir lire et écrire dans un fichier texte

## 1. Écrire dans un fichier
```python
with open("exemple.txt", "w") as fichier:
    fichier.write("Ceci est une phrase.")
```

## 2. Lire un fichier
```python
with open("exemple.txt", "r") as fichier:
    contenu = fichier.read()
    print(contenu)
```

## Exercice du jour
- Écrire une phrase dans un fichier texte, puis la relire et l'afficher. 