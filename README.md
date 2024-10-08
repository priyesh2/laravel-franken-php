# Setup Laravel with FrankenPHP

### Step 1: Clone the Repository

Navigate to the root of your Laravel project and clone the repository:
```sh
git clone https://github.com/priyesh2/laravel-franken-php.git
```


### Step 2: Move the Cloned Repository
Move the cloned repository to root directory:
```sh
mv laravel-franken-php/{Caddyfile,download.sh} ./ && rm -rf laravel-franken-php
```


### Step 3: Make Download Script Executable
Make the download script executable:
```sh
chmod +x download.sh
```

### Step 4: Download Composer and FrankenPHP
Run the download script:
```sh
./download.sh 
```


This script will download `composer.phar` for Composer and FrankenPHP for `php-cli`, `php`, and `Caddy server`.

### Step 5: Install Composer dependency
To install all the dependency, use the following command:
```sh
 ./frankenphp php-cli ./composer.phar install
```

### Step 6: Run FrankenPHP Server
To run the FrankenPHP server, use the following command:
```sh
./frankenphp run
```

### Step 7: Open Localhost
After running the server, open your web browser and navigate to https://localhost

### Step 8: gitignore 
Add this in `.gitignore`
```sh
frankenphp
composer.phar
```

### Useful command 

```sh
./frankenphp php-cli ./composer.phar (install | update | dump-autoload | require | remove)
```

```sh
./frankenphp php-cli artisan about
```

---

> *NOTE:* It installs PHP 8.3. If you need another version of PHP, you can compile and use FrankenPHP and change the Composer version.

---

