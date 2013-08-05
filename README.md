#Global-Artisan

This script provides access to the Laravel 4 Artisan command line tool from anywhere within a Laravel project directory structure.

###Installation

Place the artisan script anywhere within your `PATH`. `/usr/local/bin` is a good place.

    cp artisan /usr/local/bin/

Set the execute bit.

    chmod +x /usr/local/bin/artisan

###Usage

You can call artisan from inside any directory in your Laravel 4 project. Where before you would need to be in the project root to create a new migration

    php artisan migrate:make --create create_my_new_table

you can now call it from within any of the project subdirectories like this

    artisan migrate:make --create create_my_new_table
