## Create Docker with Laravel, Apache/PHP and Mysql

* Edit **.env** file with your settings

* Run **docker-compose up -d**

* It will create 2 containers (Apache Server and Mysql Server)

* **/www** folder will be created

* Put your application files in **/www** folder

* Install laravel with composer inside **/www** folder. Like this
    
    `composer create-project --prefer-dist laravel/laravel laravel-test 5.2.29`
    
    - You must have installed composer (need PHP) at your PC
        - https://getcomposer.org/download/
    

* Mysql data files will be in **/docker/mysql/data** folder

You can create your apache image instead of **apps4net/laraver-apache** with the command:

    docker build -t laravel-apache docker/apache