<<<<<<< HEAD
<h2>Codeigniter HTACCESS Examples</h2>

<b>Setup</b>

	1: Go to application/config/config.php

	2: Find <b>$config['index_page'] = 'index.php';</b> and make <b>$config['index_page'] = '';</b>

	3: Add your base url <b>$config['base_url'] = http://localhost/project/;</b>

	4: In the htaccess files select the right one for you. And then place in the main directory.

	5: Do not touch the htaccess in application folder.

	6: You may need to configure your routes in application/config/routes.php

<b>Example Routes</b>

Note: Some times you do not need to configure your routes.

controllers >
	Welcome.php
	Dashboard.php

application/config/routes.php

	$route['default_controller'] = 'welcome';
	
	$route['dashboard'] = "dashboard";

Add any if have example user id http://localhost/dashboard/25/ 25 would be user id. You do not have to have
the controller named dashboard you can name it to what you want just examples.

	$route['dashboard/(:any)'] = "dashboard/$1"
=======
Codeigniter HTACCESS Files.

How to use: 

  1: First Make Sure You Have Removed The index.php from application/config/config.php so looks like this $config['index_page'] = '';
  2: Enter you base_url 
  3: Choose one of the 5 htaccess files in the zip.
  4: Note some may not work depending on your operating system and server. With linux may have to do some more tweaking with apache

You also may need to configure your routes in application/config/routes.php

controllers >
  Welcome.php
  Dashboard.php
   
   
Example

  $route['default_controller'] = 'welcome';
  $route['dashboard'] = "dashboard";
  
Then try http://localhost/project-name/dashboard

I have use the first htaccess on xampp and in windows 7 and works fine. I think the second htaccess is for wamp.

Disclaimer: Please note these are just examples some may not work and some may work, it all depends on your codeigniter and server setup.
>>>>>>> origin/master
