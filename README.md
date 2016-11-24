# AWS

Create S3 bucket public access policy

Policy JSON

`{"Version": "2008-10-17",`

`"Statement": [{"Sid": "AllowPublicRead",`

`"Effect": "Allow",`

`"Principal": {`

`"AWS": "*"`

`},`

`"Action": "s3:GetObject",`

`"Resource": "arn:aws:s3:::YOUR-BUCKET-NAME/*"`

`}]}`

Access S3 bucket by Domain Name:

`1: Deside your Domain Like: abc.xyz.com`

`2: Create S3 bucket as same name like your domain name is if your doamin name is abc.xyz.com then choose abc.xyz.com as bucket name.`

`3: Then please click in Properties tab after this click in Static Website Hosting link and choose  Enable website hosting write your first 2 page link like index.html and error.html and uplode same page in bucket. `

`4: After this go to Route 53 and set your new Set Record for abc.xyz.com and choose cname and enter complete S3 URL Path .`

`5: Thanks and now you can enjoy your new staic web site`
