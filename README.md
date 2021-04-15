# TEST SHOPINVEST

## Liste des technos
- PHP 7.3.5
- Laravel 8
- MySQL 5.7.26
- Boostrap / jQuery / Ajax


## Installation

1. Clone du répertoire
   ```sh
   git clone https://github.com/kmvwsve/Test-shopinvest.git
   ```
2. Installer des packages
   ```sh
   composer install
   ```
3. Entrer le fichier `.env`, et modifer les paramètres pour la connection de la base de données.
4. Modifer le 'RewriteBase' dans le fichier `public/.htaccess`.
5. Utiliser le fichier  `projectapp.sql` pour créer la base de données de test.

## Structure des fichiers
    ├── app                    
    │   ├── Http             
    │   │   ├── Controllers              
    │   │   │   ├── admin              
    │   │   │   │   ├── category              
    │   │   │   │   │   ├── ProductController.php     # page admin index, page liste des produits, CRUD
    │   │   │   │   ├── common              
    │   │   │   │   │   ├── HeaderController.php      # page admin header
    │   │   │   │   │   ├── FooterController.php      # page admin footer
    │   │   │   ├── catalog              
    │   │   │   │   ├── category              
    │   │   │   │   │   ├── ProductController.php     # récupérer un produit par ID, actions Ajouter/Supprimer au panier
    │   │   │   │   ├── common     
    │   │   │   │   │   ├── CartController.php        # Action de session du panier
    │   │   │   │   │   ├── HeaderController.php      # page front header
    │   │   │   │   │   ├── FooterController.php      # page front footer
    |   |   |   |   └── ... 
    |   |   |   └── ...
    |   |   └── ...
    │   ├── Model              
    │   │   ├── Product.php    # Opérations CRUD de la base de donnée 
    |   |   └── ...
    ├── resources
    │   ├── views              
    │   │   ├── 404.blade.php
    │   │   ├── admin.blade.php
    │   │   ├── cart.blade.php
    │   │   ├── footer.blade.php
    │   │   ├── header.blade.php
    │   │   ├── header_admin.blade.php
    │   │   ├── product.blade.php
    │   │   ├── product_edit.blade.php
    │   │   └── ...
    |   └── ...
    └── ...
