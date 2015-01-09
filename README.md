Gravatar Library for Codeigniter
================================

Usage
-----

Before usage simply load the library as usual in your controller or other context.

```php
$this->load->library('gravatar');
```

After that you can call its public methods:

```php
echo '<br />';
echo '<br />';

$email = 'ivantcholakov@gmail.com';

$gravatar_url = $this->gravatar->get($email);

var_dump($gravatar_url);

echo '<br />';
echo '<br />';

echo '<img src="'.$gravatar_url.'" />';

echo '<br />';
echo '<br />';

$gravatar_profile = $this->gravatar->get_profile_data($email);

echo '<pre>';
echo print_r($gravatar_profile, true);
echo '</pre>';

echo '<br />';
echo '<br />';

$last_error = $this->gravatar->last_error();

echo '<pre>';
echo print_r($last_error, true);
echo '</pre>';

echo '<br />';
echo '<br />';
```

This library has been documented inside its source. For overall information about accessing gravatars see https://en.gravatar.com/site/implement/

Requirements
------------

CodeIgniter 2.x or CodeIgniter 3.x

Live Demo
---------

http://iridadesign.com/starter-public-edition-4/www/playground/gravatar-test

License Information
-------------------

Copyright (c) 2015 Ivan Tcholakov, ivantcholakov@gmail.com  
Copyright (c) 2011 - 2015 Ryan Marshall, http://irealms.co.uk  
License: The MIT License (MIT), http://opensource.org/licenses/MIT
