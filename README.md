# MVC-Development
Sample MVC Development Projects

Steps to configure the Application
1. Download and Install Xampp Version 3.2.2 running PHP 7.0+ in your C Drive
2. Download and Install composer.json
3. Download and install Visual Studio code and the GIT bash terminal (or any other IDE and
Terminal of choice)
4. Setup your laravel environment and download all relevant dependencies as per Laravel
documentations guideline
5. Within your xampp directory navigate to “C:\xampp\apache\conf\extra” and open file httpdvhosts.conf
6. Add these two statements within your file and click save
<VirtualHost *:80>
DocumentRoot "C:/xampp/htdocs"
ServerName localhost
</VirtualHost>
<VirtualHost *:80>
DocumentRoot "C:/xampp/htdocs/japp/public"
ServerName japp.dev
</VirtualHost>
7. Within your C Drive navigate to “C:\Windows\System32\drivers\etc” and open file hosts using
notepad in administrator mode
8. Paste the following lines within your document and click save
127.0.0.1 localhost
127.0.0.1 japp.dev
9. Paste the Japp folder within your Xampp, htdocs directory
10. Open your brower environment and navigate to localhost/phpmyadmin and create database
japp
11. Set your database connection string within the env file in your japp root directory folder
12. Migrate your database environment within your terminal artisan command line using relavant
migrate files located within the japp directory
13. open your browser and type http://japp.dev to access your JSON Manager Application
14. The root directory where the JSON file resides is “C:\xampp\htdocs\Japp\storage\app”
15. Your application is ready to run
