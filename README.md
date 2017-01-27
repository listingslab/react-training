# Healthy Lunch Box

## Developer
You'll need to be invited to collaborate on this private GitHub repo. Ask Petch or Hooch

cd to your working directory (ours is ~/node)
https://github.com/ustwo/healthy-lunch-box.git

## Bootstrap
https://github.com/ustwo/healthy-lunch-box/tree/feature/phase2/src/bootstrap-sass

## rsync for uploading to the AWS

```rsync -avz /Users/listingslab/node/healthy-lunch-box/build/ ec2-user@beta.healthylunchbox.com.au:/var/www/html/healthylunchbox.com.au/```

```rsync -avz /Users/listingslab/node/healthy-lunch-box/api/wordpress/ ec2-user@beta.healthylunchbox.com.au:/var/www/html/api.healthylunchbox.com.au/```

```rsync -avz /Users/listingslab/node/healthy-lunch-box/api/wordpress/wp-content/themes/ ec2-user@beta.healthylunchbox.com.au:/var/www/html/api.healthylunchbox.com.au/wp-content/themes/```



## Tech Stack Overview

A React frontend designed to consume a WordPress REST-API backend service found here:
[healthylunchbox.com.au](http://api.healthylunchbox.com.au/).

This is a complete Webpack build development environment which enables fast in-editor pre-testing of our React app against lint rules for both JavaScript and SCSS and enables multi-device testing while we develop and compile the app.

### NPM Scripts

#### npm start
Runs webpack-dev-server with hot reload

#### npm run build
Creates production ready application into /build folder

#### npm run elint
Run & Summarise the linting process

#### npm run slint
Run the style lint process

#### More Info
Using Atom editor?
Install IDE linting. It's proper helpful

```apm install linter-eslint```
&
```apm install linter-stylelint```
