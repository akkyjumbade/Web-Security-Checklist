# Web-Security-Checklist
Web Security Checklist - VAPT

### Host header injection 
Apache / httpd 
```htaccess
RewriteCond %{HTTP_HOST} !^((www\.|subdomain\.)?(example\.com|otherdomain\.in)).*$ [NC]
RewriteRule .* / [L,R=403]
```
