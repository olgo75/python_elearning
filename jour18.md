# Jour 18 : Manipuler et parcourir le DOM avec BeautifulSoup

## Objectifs
- Savoir utiliser les sélecteurs pour trouver des éléments HTML
- Parcourir et filtrer les éléments d'une page

## 1. Sélection par balise, classe, id
Exemples :
```python
# Trouver tous les liens
liens = soup.find_all('a')

# Trouver un élément par id
element = soup.find(id="mon-id")

# Trouver tous les éléments d'une classe
elements = soup.find_all(class_="ma-classe")
```

## 2. Parcourir les éléments
```python
for lien in liens:
    print(lien.get('href'))
```

## 3. Sélecteurs CSS
```python
elements = soup.select("div.titre")
```

## Exercice du jour
- Extraire tous les liens présents sur la page d'accueil de Wikipédia. 