### Step 1: Install package

```
$ yarn install
```

When package installed, postinstall script will be tiggered, and the `./cmd/rarity_analyze.js` will run for the first install. This will take some time for the rarity score calculation. (generally in minues)

### Final Step: Run

```
$ DEBUG=rarity-analyser:* yarn start-dev
```

Then open: http://localhost:3000/ on your web browser. Yes! Now you see the rarity website of your NFT collection!

### Extra

You can generate `collection-rarities.json` file by using this command:

```
yarn rarity-output-json
```

The `collection-rarities.json` file will store in `config` folder.

## Deploy to Heroku

### Step 1: Prerequisites

- Register Heroku account
- Install [Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli)

### Step 2: Login and Create App

In your Rarity folder:

```
$ heroku login
```

```
$ heroku create your_app_name
```

### Final Step: Deploy

```
$ git push heroku main
```

If you have any update want to deploy to Heroku, just use this final step to deploy to Heroku.

### Use One Click Heroku Deploy

Here you can deploy this rarity tool to Heroku in one click, just be sure you have the Heroku account.



