# AI Recipe Generator

Serverless web app that turns user-submitted ingredients into recipes using **AWS Amplify** and **Amazon Bedrock** (Claude 3 Sonnet).

## What it does
- HTML/Amplify frontend for ingredient input, with continuous deployment from GitHub
- **AWS Lambda** + **AppSync** (GraphQL) to process requests
- **Amazon Bedrock** for AI recipe generation
- **Amplify Auth / Cognito** for signed-in access

## Live demo
https://main.d3sjg76q9l66pz.amplifyapp.com

## Stack
`AWS Amplify` · `Cognito` · `Lambda` · `AppSync` · `Bedrock` · `Node.js`

## What I’d harden next
- Tighter authorization and input validation on the GraphQL path
- Structured logging / monitoring (CloudWatch) and cost controls on Bedrock calls
- Clearer IAM least-privilege for Amplify backend roles

Built as a focused AWS serverless + generative AI demo (Free Tier–friendly). Not a production certification platform — see [aws-productized-services](https://github.com/EvanInTech/aws-productized-services) and [my site](https://evanintech.carrd.co/) for broader DevSecOps / secure platform work.
