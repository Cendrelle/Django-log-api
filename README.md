# Django Blog API

Une API de blog complète développée avec **Django REST Framework** et **JWT Authentication**, avec documentation Swagger.  

## 🚀 Fonctionnalités

- Authentification JWT (login / register)  
- Gestion des articles : création, lecture, mise à jour, suppression (CRUD)  
- Gestion des catégories d’articles  
- Filtrage par catégorie  
- Recherche par mot-clé dans le titre et le contenu  
- Pagination des résultats  
- Documentation interactive avec Swagger et ReDoc  

---

## 💻 Installation

1. Cloner le dépôt
```bash
git clone https://github.com/ton-username/django-blog-api.git
cd django-blog-api

2. Créer un environnement virtuel et l’activer
python -m venv venv
venv\Scripts\activate   # Windows

3. Installer les dépendances
pip install -r requirements.txt

4. Appliquer les migrations
python manage.py migrate


5. Créer un super utilisateur (optionnel)
python manage.py createsuperuser


6.Lancer le serveur
python manage.py runserver

## Endpoints principaux 
Endpoint	Méthode	Description
/api/register/	POST	Créer un nouvel utilisateur
/api/token/	POST	Obtenir le token JWT pour login
/api/token/refresh/	POST	Renouveler le token JWT
/api/articles/	GET, POST	Lister ou créer des articles
/api/articles/<id>/	GET, PUT, PATCH, DELETE	Détails, modification ou suppression d’un article
/api/categories/	GET, POST	Lister ou créer des catégories
/api/categories/<id>/	GET, PUT, PATCH, DELETE	Détails, modification ou suppression d’une catégorie

## 📄 Documentation API
Swagger UI : http://127.0.0.1:8000/swagger/
ReDoc : http://127.0.0.1:8000/redoc/
Ces pages montrent tous les endpoints, paramètres, modèles de données et permettent de tester l’API directement depuis le navigateur.
