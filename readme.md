<!-- DO NOT EDIT THIS FILE; it is auto-generated from readme.txt -->
# Strong Password Generator

![Banner](assets/banner-1544x500.png)
Encourage the use of strong passwords by helping users generate them easily.

**Contributors:** [fjarrett](https://profiles.wordpress.org/fjarrett)  
**Tags:** [admin](https://wordpress.org/plugins/tags/admin), [login](https://wordpress.org/plugins/tags/login), [membership](https://wordpress.org/plugins/tags/membership), [passwords](https://wordpress.org/plugins/tags/passwords), [profile](https://wordpress.org/plugins/tags/profile), [security](https://wordpress.org/plugins/tags/security), [users](https://wordpress.org/plugins/tags/users)  
**Requires at least:** 3.7  
**Tested up to:** 4.2  
**Stable tag:** 0.2.0  
**License:** [GPLv3](https://www.gnu.org/licenses/gpl-3.0.html)  

[![Build Status](https://travis-ci.org/fjarrett/strong-password-generator.png?branch=master)](https://travis-ci.org/fjarrett/strong-password-generator) 

## Description ##

**Did you find this plugin helpful? Please consider [leaving a 5-star review](https://wordpress.org/support/view/plugin-reviews/strong-password-generator).**

Strong passwords are one of the best defenses for maintaining a secure website.

The **Password Generator** button makes it easy for your users to choose a secure password.

This plugin utilizes the [password-generator](https://github.com/bermi/password-generator) JavaScript library under the MIT license.

**Development of this plugin is done [on GitHub](https://github.com/fjarrett/strong-password-generator). Pull requests welcome. Please see [issues reported](https://github.com/fjarrett/strong-password-generator/issues) there before going to the plugin forum.**

## Frequently Asked Questions ##

### How can I change the default generated password length? ###
The default password length is `20` and can be overridden with a filter. Simply add this hook to your theme's `functions.php` file or as an [MU plugin](http://codex.wordpress.org/Must_Use_Plugins):

```php
add_filter( 'spg_default_password_length', 12 );
```

### How can I change the minimum required generated password length? ###
The default minimum password length is `7` and can be overridden with a filter. Simply add this hook to your theme's `functions.php` file or as an [MU plugin](http://codex.wordpress.org/Must_Use_Plugins):

```php
add_filter( 'spg_min_password_length', 8 );
```

Note: This setting only affects the minimum length of _generated passwords_, not passwords manually created by users.

### How can I change the maximum generated password length allowed? ###
The default maximum password length is `32` and can be overridden with a filter. Simply add this hook to your theme's `functions.php` file or as an [MU plugin](http://codex.wordpress.org/Must_Use_Plugins):

```php
add_filter( 'spg_max_password_length', 50 );
```

Note: This setting only affects the maximum length of _generated passwords_, not passwords manually created by users.

### How can I generate passwords that are easier to memorize? ###
The default mode for password generation is non-memorable (alphanumeric + special characters), but this too can be overridden with a filter so that generated passwords are purely alphabetic, making them easier for users to memorize. Simply add this hook to your theme's `functions.php` file or as an [MU plugin](http://codex.wordpress.org/Must_Use_Plugins):

```php
add_filter( 'spg_allow_memorable_passwords', '__return_true' );
```


## Screenshots ##

### When choosing a password, users can optionally choose to have a strong password generated for them.

![When choosing a password, users can optionally choose to have a strong password generated for them.](assets/screenshot-1.png)

### The fields are filled in automatically and the user is prompted to save their new password.

![The fields are filled in automatically and the user is prompted to save their new password.](assets/screenshot-2.png)

### The strong password generator is also available when editing profiles.

![The strong password generator is also available when editing profiles.](assets/screenshot-3.png)

## Changelog ##

### 0.3.0 - May 5, 2015 ###
* Fix: JS bug preventing manual passwords from being set
* Tweak: Use hooks to insert generator markup instead of JS
* Tweak: Improved CSS styling in various views

Props [@fjarrett](https://github.com/fjarrett)

### 0.2.0 - May 4, 2015 ###
* New: Add slider for custom password length control, retire alert window

Props [@fjarrett](https://github.com/fjarrett)

### 0.1.0 - May 4, 2015 ###
* Initial release

Props [@fjarrett](https://github.com/fjarrett)


