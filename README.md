# handle-htaccess
Hi there, this is small .htaccess docs, Thanks...

### Redirect to index.html

<pre>
<IfModule mod_rewrite.c>
RewriteEngine on
RewriteCond %{REQUEST_FILENAME} !-f
RewriteCond %{REQUEST_FILENAME} !-d
RewriteRule ^(.*)$ /index.html?path=$1 [NC,L,QSA]
</IfModule>
</pre>

### Redirect into another folder 
<pre>
<IfModule mod_rewrite.c>
RewriteEngine On
RewriteRule ^(.*)$ folder-name/$1 [L]
</IfModule>
</pre>

+ https://varvy.com/pagespeed/htaccess.html
