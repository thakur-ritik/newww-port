for aws static website.........

s3 bucket bnao---
check box not click

upload files

properties-> static web site hosting -> enable

permissions -> bucket policy



policy added
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicReadGetObject",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::new-static-ritik/*"
    }
  ]
}
