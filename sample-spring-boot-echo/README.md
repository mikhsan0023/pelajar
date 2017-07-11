# sample-spring-boot-echo

sample-spring-boot-echo is a tiny sample bot application based on Spring Boot.

## Usage

Run this sample bot using Gradle.

    ../gradlew bootRun -Dline.bot.channelToken=62D2k2ey26C+l+Jt4d63XyKUnVpsoOhGI1/BFr2cZseyEi4GbRatHzssA82IR8Z6YpluORGch45k0Xk33e7Wi9ZzUqJn9lKBa3P2hyvQL/4RXUi6nkWI8bt1A0JEZ3h/1H0oNDuIDUOS881uIY0BXAdB04t89/1O/w1cDnyilFU= \
                       -Dline.bot.channelSecret=6f1fe387fa6c923659a4d5f3ed1ae508

or if you finished create `src/main/resources/application.yml` file based on `src/main/resources/application-template.yml`. You can start configured web server just hitting

    ../gradlew bootRun

You need to pass the following options.

  * line.bot.channelToken: Your Channel access token
  * line.bot.channelSecret: Your Channel secret

For more information about configuration way, refer [Spring Boot Reference - 24. Externalized Configuration](https://docs.spring.io/spring-boot/docs/current/reference/html/boot-features-external-config.html).

## Deploy on Heroku

Deploy this module on Heroku.

### Step 1

Get the Channel access token and Channel secret from the Channel Console.

<img src="https://github.com/line/line-bot-sdk-java/blob/master/sample-spring-boot-echo/_assets/line-bot-configuration.png?raw=true">

### Step 2

Tap the deploy button.

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/line/line-bot-sdk-java)

### Step 3

Fill in the form and run your instance.

<img src="https://github.com/line/line-bot-sdk-java/blob/master/sample-spring-boot-echo/_assets/heroku.png?raw=true">

### Step 4

Tap the **Manage App** button and copy the name of your Heroku instance.

<img src="https://github.com/line/line-bot-sdk-java/blob/master/sample-spring-boot-echo/_assets/heroku-app-name.png?raw=true">

### Step 5

Set the webhook URL for your Channel on the Channel Console using the following URL:
`https://${YOUR_HEROKU_APP_NAME}.herokuapp.com/callback`

<img src="https://github.com/line/line-bot-sdk-java/blob/master/sample-spring-boot-echo/_assets/put-webhook-url.png?raw=true">
