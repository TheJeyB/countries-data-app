# Countries Data App

Application Django permettant d’explorer des données de pays à partir de l’API REST Countries, avec affichage web et statistiques.

---

## Stack

- Python
- Django
- PostgreSQL
- REST Countries API

---

## Fonctionnalités

- Liste des pays avec recherche et filtre par région : `/countries/`
- Détails d’un pays : `/countries/<cca3>/`
- Statistiques : `/countries/stats/`
- Import des données via commande personnalisée

---

## Installation

Cloner le projet :

```bash
git clone https://github.com/TheJeyB/world-countries-django.git
cd countries-data-app
```

Créer et activer un environnement virtuel :

```bash
# Windows
python -m venv venv
venv\Scripts\activate

# Mac / Linux
python3 -m venv venv
source venv/bin/activate
```

Installer les dépendances :

```bash
pip install -r requirements.txt
```

Configurer la base de données dans le fichier `.env`.

Appliquer les migrations :

```bash
python manage.py migrate
```

Importer les données :

```bash
python manage.py import_countries
```

Lancer le serveur :

```bash
python manage.py runserver
```

Ouvrir dans le navigateur :

```
http://127.0.0.1:8000/countries/
```

---

## Auteur

TheJeyB
