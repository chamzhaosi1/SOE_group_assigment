# se_web_design
September 2022 - BIBIS2123 Software Engineering Web Design Project (Laravel)
---
# Software Required to run
1. php 8.0 and above
2. Any SQL Server
3. composer
4. Node.js (Optional)
---
# Clone Repo Set Up
1. create ".env" file (Can copy from .env.example ) and set database to connect to.
2. run command: composer install
3. run command: php artisan key:generate
4. run command: npm install (use Node.js (optional))
5. run command: php artisan migrate:fresh --seed
6. Done! (run command to start server: php artisan serve)
> (Default Login account email is "superadmin@newera.edu.my" and password is "superadmin123")
---
# If MySQL / MariaDB Index Lengths key too long
1. In "App\Providers\AppServiceProvider", use "use Illuminate\Support\Facades\Schema;" from the top and add the line "Schema::defaultStringLength(191);" to boot() function
