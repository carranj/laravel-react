#Steps to create a react app on laravel

# Tools used

to setup make sure you have Docker, NPM, Node, and Composer 2.0 installed on your machine.

# 1. Install Laravel

As of September 2021, Laravel 8 is the latest and I will be using that. Installation instructions can be found at https://laravel.com/docs/8.x
run `composer create-prject laravel/laravel example-app` inside your main directory that will host your application name. Keep in mind the example-app will be the name of the directory created with all the Laravel projects.

## After installation

run `npm i` / `npm install` also works i is just the shorthand to install
Run `php artisan serve` then go to http://127.0.0.1:8000/ to make sure Laravel is installed.

#Install React
npm install --save-dev react react-dom @babel/preset-react

#Integrate React in Laravel
webpack.mix.js compiles all of your files together. there you can edit your file to include the react and version methods, you can erase the css files there, we will be using reacts js and css. You can read more on laravels documention on webpack, but doing this will install all of the presets.
[Installing React](https://laravel.com/docs/8.x/mix#react)

```
mix.js('resources/js/app.js', 'public/js')
   .react();
```
