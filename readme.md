# laravel-social-login
Login users into app using social profiles like Facebook, Google, Github and Twitter.

Make apps for desired social feaure.
In callback/redirect url of the app put as following REDIRECT.

In .env file add
```
FB_CLIENT_ID = *****
FB_CLIENT_SECRET = *****
FB_REDIRECT = 'http://localhost:8000/login/callback/facebook'

G+_CLIENT_ID = *****
G+_CLIENT_SECRET = *****
G+_REDIRECT = 'http://localhost:8000/login/callback/google'

GITHUB_CLIENT_ID = *****
GITHUB_CLIENT_SECRET = *****
GITHUB_REDIRECT = 'http://localhost:8000/login/callback/github'

TWITTER_CLIENT_ID = *****
TWITTER_CLIENT_SECRET = *****
TWITTER_REDIRECT = 'http://localhost:8000/login/callback/twitter'
```

### Commands to Run
```bash
composer install
php artisan key:generate
php artisan make:auth
php artisan migrate
php artisan serve
```