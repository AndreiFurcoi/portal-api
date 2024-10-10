# Portal API

Welcome to the Shopping API repository! Follow the steps below to set up the project environment and start developing.

## Requirements

- **PHP:** Version 8.3 or higher
    - [Download PHP](https://www.php.net/downloads)
- **Composer:**
    - [Download Composer](https://getcomposer.org/download/)
- **Git Bash:**
    - [Download Git Bash](https://git-scm.com/downloads)
- **WSL for Windows:**
    1. Open PowerShell
    2. Run: `wsl --install`
- **Docker:**
    - [Download Docker](https://www.docker.com/products/docker-desktop/)

## Project Setup

1. Open `powershell`
2. Clone repository: [Portal API](https://github.com/AndreiFurcoi/portal-api)
3. Open the terminal in the project directory and run: `composer install`
4. Open the terminal with a Linux tab
5. Create an alias for the sail command by using `alias sail='sh $([ -f sail ] && echo sail || echo vendor/bin/sail)'`
6. Run: `sail up --build`
7. Run: `sail artisan migrate:fresh --seed`

## Artisan/Composer commands with sail

If you are using the Linux terminal for artisan or composer commands, always use the sail command like this:
sail composer install
sail artisan migrate

## Aliases TODO

You're all set! Happy coding!

## Laravel Pint

For [Pint](https://laravel.com/docs/11.x/pint) usage: `sail composer pint`

## Laravel Pulse

For [Pulse](https://laravel.com/docs/11.x/pint) usage:
1. Run `php/sail artisan vendor:publish --provider="Laravel\Pulse\PulseServiceProvider"`
2. Migrate using `php/sail artisan migrate`
3. Check the installation on `/pulse`

## Laravel Telescope

For [Telescope](https://laravel.com/docs/11.x/pint) usage:
1. Run `php/sail artisan telescope:install`
2. Migrate using `php/sail artisan migrate`
3. Check the installation on `/telescope`

## PHPStan

For [phpstan](https://phpstan.org/) usage: `sail composer stan`
