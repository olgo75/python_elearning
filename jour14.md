# Jour 14 : Mini-projet

## Objectifs
- Réutiliser toutes les notions vues
- Structurer un petit programme

## 1. Récapitulatif
- Variables, types, conditions, boucles, fonctions, fichiers, exceptions, listes, dictionnaires, modules

## 2. Exemple de structure
```python
nom = input("Nom : ")
age = input("Âge : ")
ville = input("Ville : ")

with open("utilisateur.txt", "w") as fichier:
    fichier.write(f"Nom : {nom}\nÂge : {age}\nVille : {ville}\n")
```

## Exercice du jour
- Créer un programme qui demande le nom, l'âge, et la ville de l'utilisateur, puis sauvegarde ces infos dans un fichier texte. 