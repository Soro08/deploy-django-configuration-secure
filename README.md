# deploy-django-configuration
Configuration du fichier stting avant deployement

## Check deploie

`python manage.py check --deploy`

## Configure
````
# SECURITY WARNING: don't run with debug turned on in production!
DEBUG = False

ALLOWED_HOSTS = ['localhost', '127.0.0.1', 'your_domain_name', 'your_ip_add']

# deployement   
SECURE_BROWSER_XSS_FILTER = True
SECURE_SSL_REDIRECT = False
SESSION_COOKIE_SECURE = True
CSRF_COOKIE_SECURE = True
SECURE_HSTS_SECONDS = 1
SECURE_HSTS_INCLUDE_SUBDOMAINS = True
SECURE_HSTS_PRELOAD = True


SECURE_CONTENT_TYPE_NOSNIFF = True
```
