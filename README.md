<p align="center">
<a href="https://github.styleci.io/repos/167211927"><img src="https://github.styleci.io/repos/167211927/shield?branch=2.x" alt="StyleCI"></a>
<a href="https://travis-ci.org/itorgov/laravel-forge-bot"><img src="https://travis-ci.org/itorgov/laravel-forge-bot.svg?branch=2.x" alt="Build Status"></a>
<a href="https://packagist.org/packages/itorgov/laravel-forge-bot"><img src="https://poser.pugx.org/itorgov/laravel-forge-bot/v/stable" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/itorgov/laravel-forge-bot"><img src="https://poser.pugx.org/itorgov/laravel-forge-bot/license" alt="License"></a>
</p>

# Laravel Forge Telegram Bot

[@LaravelForgeBot](https://t.me/LaravelForgeBot) is unofficial Laravel Forge chat bot for Telegram messenger.

## Motivation

Several years ago I have started to use Laravel Forge for deploying my and my clients' projects.
I found that Laravel Forge couldn't send deployment notification to Telegram messager but for me, Telegram is the number one messenger.
That time I just wrote a simple bot with hardcoded chat id and webhook URL.
During my work, I realized that I need a more flexible solution and I designed and implemented the first version of this bot.
The first version could only send deployment notifications.
It just generated a webhook URL for you and then you had to add that URL manually to your Laravel Forge's site.
After release, I have started to work with a new client.
This client has had a project where I haven't could to enable "Quick deploy".
Because of that I had to go to the Laravel Forge website and hit the button "Deploy Now" whenever I needed to update the production.
So I decided to improve my bot and built the second version.

## Features

[@LaravelForgeBot](https://t.me/LaravelForgeBot) helps you manage your servers in such operations as:

* Reboot a server.
* Reboot MySQL.
* Reboot PostgreSQL.
* Reboot PHP.
* Reboot NGINX. 

It also have a feature to run deploy of your site right from Telegram.
It's really helpful when you don't want to enable "Quick deploy" feature for your site.

Other awesome feature is sending deployment notifications from Laravel Forge to you or any other chat.
Using this abilyty only one member of your team will manage servers in his private chat with the bot, but all members will recieve deployment notifications in your team chat.

## Screenshots

There will be screenshots.

## How to use?

List of available commands:

* /addtoken
* /deletetoken
* /menu
* /showchatid

You always can get an actual list of commands by using /help command.

### /addtoken

Use this command to add your [Laravel Forge API token](https://forge.laravel.com/user/profile#/api).
Note that you can add multiple tokens, so you can manage different Laravel Forge accounts from one place.
This command will trigger automaticaly after /start command.

### /deletetoken

If you want you can delete added token from the bot by using this command.

### /menu

This command creates a new menu for managing servers.

### /showchatid

Use this command to get an ID of any chat.
It will be helpful when you'll configure receiving deployment notifications to other chat.
Please note that if you have more than one bots in your target chat then you have to write bot's username after the command without space (/showchatid@LaravelForgeBot).

## Versioning

We use [SemVer](http://semver.org) for versioning. For the versions available, see the [releases on this repository](https://github.com/itorgov/laravel-forge-bot/releases). 

## Authors

* [**Ivan Torgov**](https://github.com/itorgov) - *initial work*

## License

[@LaravelForgeBot](https://t.me/LaravelForgeBot) is licensed under the [ISC](https://github.com/itorgov/laravel-forge-bot/blob/2.x/LICENSE) license.  
Copyright &copy; 2020, Ivan Torgov
