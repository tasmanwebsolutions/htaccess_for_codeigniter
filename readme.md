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