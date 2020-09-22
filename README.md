# Receiptify

Web application inspired by https://www.instagram.com/albumreceipts/. Generates receipts that list out a user's top tracks in the past month, 6 months, and all time.

The application can be viewed at https://receiptify.herokuapp.com/.

## Using your own credentials

You will need to register your app and get your own credentials from the Spotify for Developers Dashboard.

To do so, go to [your Spotify for Developers Dashboard](https://beta.developer.spotify.com/dashboard) and create your application. In my own development process, I registered these Redirect URIs:

- http://localhost:3000 (needed for the implicit grant flow)
- http://localhost:3000/callback

## Running the App Locally

This app runs on Node.js. On [its website](http://www.nodejs.org/download/) you can find instructions on how to install it. You can also follow [this gist](https://gist.github.com/isaacs/579814) for a quick and easy way to install Node.js and npm.

Once installed, clone the repository and install its dependencies running:

    $ npm install

Once you have created your app, load the `client_id` and `client_secret` into a `.env` file.

In order to run the app, open the folder, and run its `app.js` file:

    $ npm start

Then, open `http://localhost:3000` in a browser.

## Deploying in Heroku

Change config vars in heroku

```
KEY             : VALUE
ClientID        : VALUE
ClientSecret    : VALUE
URL             : VALUE
url_callback    : VALUE
```
