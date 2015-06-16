<h3>Codeigniter 2 & 3 htaccess examples</h3>

=======================================

<h4>Read First:</h4>
<b>Disclaimer:</b> Please note these .htaccess files some may not work and some may work, it all depends on your <b>Codeigniter Version and Server and Operating System</b>

<p>Note: If you find one that is not on list please create a pull request and add the htaccess that you would like. And also add what OS for ie. linux windows etc.</p>

<b>Comment:</b><p>I have used the first .htaccess with xampp and windows 7 and 8.1 works fine.</p>

<h3>Removing index.php from url</h3>

<b>Setup</b>

	1: Go to application/config/config.php
	
	2: Add your base url $config['base_url'] = "http://localhost/project/";

	3: Find $config['index_page'] = 'index.php'; 
	
	4: And replace $config['index_page'] = '';

	5: Select the right one for you. And then place in the main directory. Don't touch the application folder .htaccess

	6: Do not touch the htaccess in application folder.

	7: You may need to configure your routes in application/config/routes.php

<b>Example Routes application/config/routes.php</b>

Note: Some times you do not need to configure your routes.

	$route['default_controller'] = 'welcome';
	
	$route['dashboard'] = "dashboard"; Example 1

	$route['dashboard/(:any)'] = "dashboard/$1" Example 2

<b>Pull Request</b>
	
<p>You are more than welcome to create a pull request <a href="https://github.com/riwakawebsitedesigns/htaccess_for_codeigniter/pulls" target="_blank">Pull Request</a> If you come across any more htacces examples that might be a good idea to have. If you feel the read me file needs to be updated or improved you can make a pull request also.</p>
