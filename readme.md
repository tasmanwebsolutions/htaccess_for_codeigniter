<h2>Codeigniter HTACCESS Examples</h2>

=======================================

<b>Setup</b>

	1: Go to application/config/config.php

	2: Find $config['index_page'] = 'index.php'; and make $config['index_page'] = '';

	3: Add your base url $config['base_url'] = "http://localhost/project/";

	4: In the htaccess files select the right one for you. And then place in the main directory.

	5: Do not touch the htaccess in application folder.

	6: You may need to configure your routes in application/config/routes.php

<b>Example Routes</b>

Note: Some times you do not need to configure your routes.

controllers >

controllers >	Welcome.php
	
controllers >	Dashboard.php

application/config/routes.php

	$route['default_controller'] = 'welcome';
	
	$route['dashboard'] = "dashboard";

Add any if have example user id http://localhost/dashboard/25/ 25 would be user id. You do not have to have
the controller named dashboard you can name it to what you want just examples.

	$route['dashboard/(:any)'] = "dashboard/$1"

Disclaimer: Please note these are just examples some may not work and some may work, it all depends on your codeigniter and server setup.
