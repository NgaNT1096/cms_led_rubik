
# TailAdmin Inertia
Setup Directions
------

1. ```npm install```
2. ```composer install```
3. Please clone .env.example and copied file name change from .env.example to .env
4. Create a clean db table
5. Set database infos in the .env
6. ```php artisan migrate --seed```
7. ```php artisan storage:link```
8. ```php artisan key:generate```
9. ```npm run dev```
10. ```php artisan serve```
11. ```Goto: http://localhost:8000```

Setup Directions with Docker - Linux

1. Setup Docker with user permissions on pc
2. clone this repo to any directory ```git clone sinan-aydogan/tailadmin-laravel```
3. Enter project root directory by terminal for example ```cd tailadmin-laravel```
4. Install composer packages by docker, because your host machine doesn't have php, mysql, nginx etc. Everything is in the docker containers
   ```docker run --rm \ -u "$(id -u):$(id -g)" \ -v "$(pwd):/var/www/html" \ -w /var/www/html \ laravelsail/php83-composer:latest \composer install --ignore-platform-reqs```
5. You should add an alias to your .bashrc file for shorcut to sail. ```sudo nano ~/.bashrc```
6. Adds this lines end of the file ```alias sail='sh $([ -f sail ] && echo sail || echo vendor/bin/sail)'```
7. Apply changes ```source ~/.bashrc```
8. You can start the project with sail ```sail up -d```
9. Don't forget add to domain to your host file ```sudo nano /etc/hosts```
    - ```127.0.0.1 tailadmin-laravel.test```
10. Go to ```http://tailadmin-laravel.test``` or your custom domain 

Admin Login Infos / Demo Account
------

- **Demo:** *[https://tailadmin-demo.tailadmin.dev](https://tailadmin-demo.tailadmin.dev)*
- **Email:** *admin@tailadmin.dev*
- **Password:** *admin*


[![TailAdmin Demo](public/img/demo/youtube.jpg)](https://www.youtube.com/playlist?list=PLbdS49WKsrOXTo_X_Ja6P3zll1yyhoIYN)

## Help

If you need to help more than this documentation: 
 - You can join our [Discord Channel](https://discord.gg/TnjA2GqYmw) then ask your questions
 - Access to our [Tabbs page](https://tailadmin.tabbs.co/) for how to make links (Install in Linux, solution of the npm errors etc.)

## Featured :

- TailwindCSS
- Vue.js 3 Laravel 12 - JetStream Inertia
- Every component are well documented
- Easy usability
- Simple and short code blocks
- A lot of customization options for every component
- Responsive, you can use with all devices
- Custom Auth Pages: Login, Register, Profile, Lock
- Unique Form Inputs: Repeatable Fields, Select(Rich Content) and Date
- Completely UI Kit
- Statistic Widgets for Summary or Small Data Windows
- It works with FontAwesome
- ### Content Components :
    - Alert 
    - Avatar / Avatar Group for Team Lists 
    - Badge 
    - Breadcrumb 
    - Buttons 
    - Content Card
    - Collapsible Content
    - Dropdowns
    - Lists 
    - Modals 
    - Pagination
    - Popovers 
    - Progress 
    - Statistic Widgets
    - Tabs 
    - FrontEnd Table
    - BackEnd Table 
      - With Dynamic Query Builder
      - Auto generated advanced search fields
      - Sort 
      - Show-hide columns
    - Tooltips

- ### Form Components :
    - Form Content 
    - Form Section 
    - Input Group 
    - HTML Inputs 
    - Text Input
    - Selectable Text Input (Combo)
    - File Input
    - Checkbox
    - Radio
    - Text Area
    - Select
    - Multi Select
    - Repeatable Fields
    - Date/Calendar Input
    - Between Input

> :rocket:  We are going to make the big updates about app because this theme is using in our projects therefore the updates will be continuous

---
