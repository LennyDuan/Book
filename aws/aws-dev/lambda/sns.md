## Example send SNS from lambda

```
const AWS = require('aws-sdk');
const SNS = new AWS.SNS();
const arm = 'full_name_arm';
const subject = 'full_name_subject';

exports.handler = (payloads, context, callback) => {
  try {
    const upcs = payloads.upcs;
    console.log(`Start check duplicated properties for upcs ${upcs.toString()}`);
    upcs.forEach(upc => {
      const msgBody = {
        default: {
          upc,
        },
        sqs: {
          upc,
        }
      };
      const params = {
        Message: msgBody,
        Subject: subject,
        TopicArn: arm,
      };
      SNS.publish(params, context.done);
      console.log(`Send SNS for property ${JSON.stringify(params)}`);
    });

    callback(null, "Check duplicated properties completed");
  }
  catch (error) {
    console.log(`Error found: ${error}`);
    callback(error);
  }
};
```