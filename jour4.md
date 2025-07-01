# Jour 4 : Les conditions (if, else, elif)

## Objectifs
- Comprendre les structures conditionnelles
- Utiliser les opérateurs de comparaison

## 1. Les conditions
Permettent d'exécuter du code seulement si une condition est vraie.

Exemple :
```python
age = 18
if age >= 18:
    print("Majeur")
else:
    print("Mineur")
```

## 2. Opérateurs de comparaison
- `==` égal à
- `!=` différent de
- `<` inférieur à
- `>` supérieur à
- `<=` inférieur ou égal à
- `>=` supérieur ou égal à

## 3. elif
Pour tester plusieurs cas :
```python
note = 15
if note >= 16:
    print("Très bien")
elif note >= 10:
    print("Moyen")
else:
    print("Insuffisant")
```

## Exercice du jour
- Demander l'âge de l'utilisateur et afficher s'il est majeur ou mineur. 