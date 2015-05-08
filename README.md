# Kirby Project Hub Translations

This repository contains language files for the [Kirby Project Hub Theme](https://www.project-hub.net), a simple project management tool for web designers and developers.

Kirby Project Hub is an intuitive client area a freelancer can add to his website and it allows his clients to quickly and easily monitor the progress of an ongoing project.


## Usage

The user interface of the project page is translatable. Two files are included in the theme, one in English and one in French. If you want to use a different language, you can add a new language specification to the /site/config/config.php file and create a new language file in the /site/languages directory. Check out the Kirby documentation for more information about [multilingual Kirby websites](http://getkirby.com/docs/languages).

When using the Kirby Admin Panel, a dropdown menu in the top-right corner of the screen let's you switch language when you add content to the website.


**Examples** :


If you wish to add a new language to the project hub (i.e. Dutch), make the following changes to the language configuration in the /site/config/config.php file :

```php

c::set('languages', array(
  array(
    'code'    => 'en',
    'name'    => 'English',
    'default' => true,
    'locale'  => 'en_US',
    'url'     => '/',
  ),
  array(
    'code'    => 'fr',
    'name'    => 'Français',
    'locale'  => 'fr_FR',
    'url'     => '/fr',
  ),
  array(
    'code'    => 'nl',
    'name'    => 'Nederlands',
    'locale'  => 'nl_NL',
    'url'     => '/nl',
  )
));

```


If you wish to switch the default language from English to French, make the following changes to the language configuration in the /site/config/config.php file :

```php

c::set('languages', array(
  array(
    'code'    => 'fr',
    'name'    => 'Français',
    'default' => true,
    'locale'  => 'fr_FR',
    'url'     => '/',
  ),
  array(
    'code'    => 'en',
    'name'    => 'English',
    'locale'  => 'en_US',
    'url'     => '/en',
  ),
));

```



## Credits

Dutch language file by [Wietse Neven](https://gist.github.com/wietseneven/0e9c497e3819ebf06876)
