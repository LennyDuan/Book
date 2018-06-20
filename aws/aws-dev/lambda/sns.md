## Example send SNS from lambda

```
const AWS = require('aws-sdk');
const SNS = new AWS.SNS();
const arm = 'full-name-arm';
const subject = 'full-name-subject';

exports.handler = (payloads, context, callback) => {
  try {
    const body = payloads.body;
    const msgBody = {
      key: body,
    };
    const params = {
      Message: msgBody,
      Subject: subject,
      TopicArn: arm,
    };
    SNS.publish(params, context.done);
    callback(null, "SNS have been sent ${JSON.stringify(params)}");
  }
  catch (error) {
    console.log(`Error found: ${error}`);
    callback(error);
  }
};
```