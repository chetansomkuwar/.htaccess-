What is .htaccess file.

.htaccess is used by web servers that are powered by Apache.
They are used to configure each directory.
Also, if the web hosting doesn't let you edit the .htaccess file, then you can easily create a new one & overwrite the parameteres from your .htaccess file.



## USE CASES:- 



RewriteEngine On
RewriteBase /


## redirection html pages to the main root domain
RewriteRule ^index\.html$ / [NC,R,L]


## http to http://www redirection
RewriteEngine on
RewriteCond %{HTTPS} OFF [OR]
RewriteCond %{HTTP_HOST} |^www\. [NC]
RewriteCond %{HTTP_HOST} ^(.*)$ [NC]
RewriteRule (.*) https://www.%1/$1 [R=301,L]


## http to https redirection
RewriteEngine On
RewriteCond %{HTTP_HOST} |^www\.
RewriteCond %{HTTPS} s on (s) | offs()
RewriteRule ^http%1://www.%{HTTP_HOST}% {REQUEST_URI} [NC,R,L]
