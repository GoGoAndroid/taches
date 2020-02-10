## Status actuel 
Current usage (voir keys)
  POST <url>/api/notes
    POST_DATA
  
 Ex post data title bla description blu

** Actuellement ici
/Users/<user>/Documents/workspace_aws/taches

Acces base : appli Mongo DB Compass
Stats base: https://cloud.mongodb.com/

# Boilerplate for Creating Restful API using Express.js, Node.js, Mongodb and Setting up on AWS Lambda

- Prerequisites

  - `AWS IAM Role`
  - `Mongodb Atlas Cloud`
  - `Serverless Framework`
  - `Node.js`
  - `Express.js`
  - `Mongodb`
  - `body-parser`
  - `Serverless-offline`
  - `loadtest`

**Installation Steps**

In the root directory run the following command:
- `npm install`
It will save all the dependencies and dev-dependencies present in package.json

**Setup the IAM Role and configure the serverless(sls) commandline.**
commande :   credentials --provider aws --key <key> --secret <secret> (credential.csv)
**Create an account on Mongodb Atlass Cloud and Whitelist the IP Address 0.0.0.0/0. Also create a user in database and setup it in secrets.json**

**Create Restful API using Express and Node**

**Deploy the codebase using ``` sls deploy ``` for the development stage**
For production switch over to ``` production ``` in secrets.json

After ``` sls deploy ```. Code will be deployed on AWS Lambda. Head over to AWS Lambda and test it using Postman or Insomnia. After that for scaling test, use ``` loadtest ``` and send 100 GET concurrent requests for 10 simulatenous users and watch the latency that comes around to be ~5 seconds.

Current usage (voir keys)
  POST <url>/api/notes
    POST_DATA
  
 Ex post data title bla description blu

** Actuellement ici
/Users/<user>/Documents/workspace_aws/taches

