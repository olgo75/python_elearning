# Jour 3 : Opérations et conversions

## Objectifs
- Savoir faire des opérations arithmétiques
- Comprendre la concaténation de chaînes
- Savoir convertir des types

## 1. Opérations arithmétiques
- Addition : `+`
- Soustraction : `-`
- Multiplication : `*`
- Division : `/`

Exemple :
```python
a = 5
b = 2
print(a + b)  # 7
print(a * b)  # 10
```

## 2. Concaténation de chaînes
Assembler des textes :
```python
prenom = "Alice"
print("Bonjour, " + prenom)
```

## 3. Conversion de types
Pour convertir une chaîne en nombre :
```python
texte = "42"
nombre = int(texte)  # 42
```
Pour convertir un nombre en chaîne :
```python
age = 30
texte = str(age)  # "30"
```

## 4. Saisir des valeurs avec input()
```python
x = input("Entrez un nombre : ")
```
Attention : `input()` retourne toujours une chaîne !

## Exercice du jour
- Demander à l'utilisateur deux nombres et afficher leur somme. 