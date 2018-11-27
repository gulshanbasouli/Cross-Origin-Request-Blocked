# Cross-Origin-Request-Blocked
Cross-Origin Request Blocked:

Try this in the .htaccess of the external root folder :

<IfModule mod_headers.c>
    Header set Access-Control-Allow-Origin "*"
</IfModule>

if There only concerns .js scripts you can wrap the above code inside this:

<FilesMatch "\.(js)$">
...
</FilesMatch>


