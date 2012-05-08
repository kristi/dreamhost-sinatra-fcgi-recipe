dreamhost-sinatra-recipe
========================

Simple hello world sinatra app to deploy on dreamhost

## Instructions

- Setup your domain to run fastcgi
- Install gems

```
gem install sinatra
```

- Unpack files

Make sure you put your files in the following locations:

```
~/example.com/public/.htaccess
~/example.com/public/dispatch.fcgi
~/example.com/public/appdir
```

Note that for a real app, you wouldn't put your app files 
in the public directory. You just have to adjust the paths
in dispatch.fcgi

- Set permissions

```
chmod 644 .htaccess
chmod +x dispatch.fcgi
```

- View website

You should get a "Hello world" message if you browse your site

