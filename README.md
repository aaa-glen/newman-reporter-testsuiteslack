Custom [Postman](https://www.postman.com/) /[Newman](https://github.com/postmanlabs/newman) api test suite reporter for [Slack](https://slack.com/)

## Setup
- Install [Newman](https://github.com/postmanlabs/newman) ``` $ npm run i -g newman ```
- Create slack app with a [Slack webhook](https://api.slack.com/messaging/webhooks)
- Install this custom Newman reporter ``` npm i -g newman-reporter-testsuiteslack ```

## Running the test collection
```CLI
 newman run <thisCollectionFile> -e <thisEnvironmentFile> --suppress-exit-code -r testsuiteslack --reporter-testsuiteslack-webhookurl '<thisWebhookUrl>'
```
