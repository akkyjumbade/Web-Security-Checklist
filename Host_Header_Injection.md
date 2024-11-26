# Host Header Injection

## Apache / httpd 
```htaccess
RewriteCond %{HTTP_HOST} !^((www\.|subdomain\.)?(example\.com|otherdomain\.in)).*$ [NC]
RewriteRule .* / [L,R=403]
```
