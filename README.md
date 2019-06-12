# Heroku Logs on AWS CloudWatch using AWS Lambda 

![python](https://img.shields.io/badge/-python-555555.svg) ![serverless](http://public.serverless.com/badges/v3.svg)

Stream and store heroku logs in AWS Cloudwatch using AWS Lambda and Heroku Log Drains.

More info: https://coderecipe.ai/architectures/59609314

### Download the code locally

```
git clone git@github.com:CodeRecipe-dev/Heroku-log-AWS-cloudwatch.git
```

### Deploy to the cloud  

```
cd Heroku-log-AWS-cloudwatch

npm install

serverless deploy --stage <your-stage-name>

```

### Add endpoint as Log Drain on heroku

```
heroku drains:add <api endpoint from serverless deploy> -a <heroku app name>
```