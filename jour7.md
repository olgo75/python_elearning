# Jour 7 : Les dictionnaires

## Objectifs
- Comprendre la structure d'un dictionnaire
- Savoir manipuler les clés et valeurs

## 1. Créer un dictionnaire
```python
livre = {
    "titre": "Le Petit Prince",
    "auteur": "Antoine de Saint-Exupéry",
    "année": 1943
}
```

## 2. Accéder aux valeurs
```python
print(livre["titre"])
```

## 3. Parcourir un dictionnaire
```python
for cle, valeur in livre.items():
    print(cle, ":", valeur)
```

## Exercice du jour
- Créer un dictionnaire avec des informations sur un livre (titre, auteur, année), puis afficher chaque valeur. 