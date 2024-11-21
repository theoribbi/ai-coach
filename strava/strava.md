# Strava API Connection

## For M241 of CFPT

## Authentication

###  Link account

Open this in browser
```http://www.strava.com/oauth/authorize?client_id=YOUR_CLIENT_ID&response_type=code&redirect_uri=http://localhost/exchange_token&approval_prompt=force&scope=activity:read_all```

After authorize, take the code in return url

### Auth & Access token

```
POST https://www.strava.com/oauth/token?client_id=CLIENT_ID&client_secret=SECRET&code=CODE&grant_type=authorization_code
```

## Activites

### Get activities

```
GET https://www.strava.com/api/v3/athlete/activities?access_token=YOUR_TOKEN
```