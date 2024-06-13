# Facebook Login using PHP

## Setup

### 1. Go to Facebook for Developers
Create a new app and configure it.

### 2. Update Facebook App Details in Code
Edit the PHP files (`index.php`) and replace `your-app-id` and `your-app-secret` with your Facebook app credentials.

```php
$fb = new Facebook\Facebook([
    'app_id' => 'your-app-id', // your app id
    'app_secret' => 'your-app-secret', // your app secret
    'default_graph_version' => 'v2.5',
]);
```

**call back url**
    <p>replace website URL name as added in the developers.Facebook.com/apps</p>

```php
$loginUrl = $helper->getLoginUrl('http://localhost/facebook-login-using-php/', $permissions);
```

## Directory structure
```
    facebook-login-using-php
    |-- index.php
    |-- logout.php
    |-- profile.php
    |-- vendor
    |-- composer.json
    |-- composer.lock
```