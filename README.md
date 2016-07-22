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
