# Jour 15 : Les environnements virtuels et la gestion des paquets

## Objectifs
- Comprendre l'intérêt des environnements virtuels
- Savoir créer un environnement virtuel avec venv
- Installer des paquets avec pip

## 1. Pourquoi un environnement virtuel ?
Un environnement virtuel permet d'isoler les dépendances d'un projet Python. Cela évite les conflits entre différents projets.

## 2. Créer un environnement virtuel
Dans le terminal, placez-vous dans le dossier de votre projet puis tapez :

```bash
python -m venv env
```

Cela crée un dossier `env` contenant l'environnement virtuel.

## 3. Activer l'environnement virtuel
- **Windows :**
```bash
.\env\Scripts\activate
```
- **Mac/Linux :**
```bash
source env/bin/activate
```

Vous devriez voir `(env)` au début de la ligne de commande.

## 4. Installer un paquet avec pip
Exemple : installer la bibliothèque `requests` :
```bash
pip install requests
```

## 5. Désactiver l'environnement virtuel
```bash
deactivate
```

## Exercice du jour
- Créer un environnement virtuel et installer le paquet `requests`. 