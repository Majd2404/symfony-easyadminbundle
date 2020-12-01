# Symfony 5
# Configure easyadminbundle
1. Create a traditional web application
+ composer create-project symfony/website-skeleton symfony5-easyadminbundle
2. Databases and the Doctrine ORM
Installing Doctrine:
+ composer require symfony/orm-pack
+ composer require --dev symfony/maker-bundle
Configuring the Database:
    The database connection information is stored as an environment variable called DATABASE_URL. For development, you can find and customize this inside .env:
    DATABASE_URL=mysql://root:'root'@127.0.0.1:3300/easyAdminBundle

+ php bin/console doctrine:database:create

Creating an Entity Class:
+ php bin/console make:entity
+ php bin/console make:migration
+ php bin/console doctrine:migrations:migrate    


3. Run the following command to install EasyAdmin in your application:
+  composer require symfony/maker-bundle --dev
+  composer require easycorp/easyadmin-bundle
4. Run the following command to quickly generate a dashboard controller:
+  php bin/console make:admin:dashboard
5. Run the following command to generate the basic structure of a CRUD controller:
+  php bin/console make:admin:crud

6. You will get this message 
"You have successfully installed EasyAdmin 3 in your application!", but you must customize the dashboard start page.

********Good luck*******

