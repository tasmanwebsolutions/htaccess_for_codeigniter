<h3>Codeigniter 3 And Up</h3>

<h4>Read First:</h4>
<b>Disclaimer:</b> Please note these .htaccess files some may not work and some may work, it all depends on your <b>Codeigniter Version and Server and Operating System</b>

<p>Note: If you find one that is not on list please create a pull request and add the htaccess that you would like. And also add what OS for ie. linux windows etc.</p>

User Guide For Codeigniter 3 + <a href="http://www.codeigniter.com/user_guide/" target="_blank">Codeigniter 3 + Userguide</a>

<h3>Removing index.php from url</h3>

<b>Setup</b>

1: Choose your .htaccess file, And then place in the main directory but outside of the application folder.

2: Go to application/config/config.php

3: Set your base url as it is now recommended  $config['base_url'] = "http://localhost/yourprojectname/";

4: Find $config['index_page'] = 'index.php'; 
	
5: And replace $config['index_page'] = '';

6: Do not touch the htaccess file in application folder.

7: You may need to configure your routes in application/config/routes.php

<b>Example Routes application/config/routes.php</b>

Note: Some times you do not need to configure your routes.

$route['default_controller'] = 'welcome';
	
$route['dashboard'] = 'dashboard';

$route['dashboard/(:any)'] = 'dashboard/$1';

<b>Pull Request</b>
	
<p>You are more than welcome to create a pull request <a href="https://github.com/wolfgang1983/htaccess_for_codeigniter/pulls" target="_blank">Pull Request</a> If you come across any more htacces examples that might be a good idea to have. If you feel the read me file needs to be updated or improved you can make a pull request also.</p>
