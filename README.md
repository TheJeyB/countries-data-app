# Countries Data App

Mini application Django pour explorer des données pays provenant de l’API REST Countries, avec interface web et statistiques.

---

## Technologies utilisées

- Python 3.14  
- Django 6.0  
- PostgreSQL ou SQLite  
- Tailwind CSS (via CDN)  
- API REST Countries (https://restcountries.com)  

---

## Fonctionnalités

- Liste des pays avec pagination et filtres (nom et région) : `/countries/`  
- Détails d’un pays : `/countries/<cca3>/`  
- Statistiques : `/countries/stats/`  
  - Nombre total de pays  
  - Top 10 pays par population  
  - Top 10 pays par superficie  
  - Répartition par région  

---

## Installation et configuration

### 1. Cloner le dépôt

```bash
git clone https://github.com/TheJeyB/countries-data-app.git
cd countries-data-app
# Windows
python -m venv venv
venv\Scripts\activate

# Linux / Mac
python3 -m venv venv
source venv/bin/activate



pip install -r requirements.txt



Configurer la base de données

Modifie le fichier .env avec les informations de ta base de données (SQLite ou PostgreSQL).

Exemple de variables dans .env :

DATABASE_ENGINE=django.db.backends.postgresql
DATABASE_NAME=nom_de_ta_base
DATABASE_USER=ton_user
DATABASE_PASSWORD=ton_mdp
DATABASE_HOST=localhost
DATABASE_PORT=5432


5. Faire les migrations
python manage.py migrate

6. Importer les données pays
python manage.py import_countries


7. Lancer le serveur Django
python manage.py runserver
