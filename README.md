Heroku buildpack: impart-inspector
=======================

Usage
-----

Add buildpack
```
heroku create --buildpack https://github.com/sbzimpart/heroku-buildpack-proxy
```

Create impart-inspector access token and set config value
```
heroku config:set INSPECTOR_API_ACCESS_TOKEN=<access_token_value>
```

Run command:
```
bin/inspector-app --http_listen_addr=:$PORT --http_listener_disable_tls &
```


