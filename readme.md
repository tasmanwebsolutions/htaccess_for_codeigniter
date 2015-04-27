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
