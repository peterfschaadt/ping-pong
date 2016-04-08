# Ping Pong Dashboard

An automated ping pong scoreboard/leaderboard for the office.

Based on a project created by [sidgtl](https://github.com/sidgtl/Ping-Pong), with updates from [timelf123](https://github.com/timelf123/Ping-Pong). Check out sidgtl's [original blog post](http://sidigital.co/blog/lab-notes-hacking-our-ping-pong-table).

A demo version of the app is available on Heroku at [http://hobbyproj.herokuapp.com](http://hobbyproj.herokuapp.com)


## Required Components

**Scorekeeper:**

- [Particle Photon (used to be "Spark Core")](https://store.particle.io/collections/photon)

- 2x [Capacitive touch sensor](https://www.adafruit.com/product/1374)

**RFID reader:**

- [Arduino Pro Mini board](http://www.arduino.cc/en/Main/ArduinoBoardProMini)

- [Adafruit CC3000 WiFi breakout board](https://www.adafruit.com/products/1469)

- [ID-12LA RFID reader](https://www.coolcomponents.co.uk/rfid-reader-id-12la-125-khz.html)

- [RFID tags](http://www.amazon.com/100pcs-125khz-Wholesale-Proximity-Keyfobs/dp/B00H1HGPH2)


## Running in Development Mode

1. Modify config.js file.

2. Build front end with Gulp: ```$ gulp```

3. Start Node server: ```$ NODE_ENV=development npm start```


## Deploying

1. Create a new branch with Git: ```$ git checkout -B <branch> master```

2. Remove the following from the .gitignore: config.js, versions, and compiled CSS/JS.

3. Build front end with Gulp: ```$ gulp```

4. Deploy branch with Git: ```$ git push origin <branch>:master```
