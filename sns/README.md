# AWS-SNS
#### Send SMS with AWS Javascript SDK or node js sdk
````````````````````````````
var AWS = require('aws-sdk');
  // configure AWS
    AWS.config.update({
'region': 'us-west-2',
      'accessKeyId': '[accessKeyId]',
      'secretAccessKey': '[secretAccessKey]'
    });

    var sns = new AWS.SNS();
   // var sqs = new AWS.SQS();
//     sns.createTopic({
//     'Name': 'pikfoodsns'
//    }, function (err, result) {

//     if (err !== null) {
//         console.log(util.inspect(err));
//         return;
//     }

//     console.log(util.inspect(result));

// });
var params = {
  Message: 'this is a test message',
  MessageStructure: 'string',
  PhoneNumber: '+91[10 digit mobile no.]'
};

sns.publish(params, function(err, data) {
  if (err) console.log(err, err.stack); // an error occurred
  else     console.log(data);           // successful response
});
````````````````````````
