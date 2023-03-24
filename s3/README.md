# ACL S3 Publicly
https://havecamerawilltravel.com/how-allow-public-access-amazon-bucket/


# Copy code below on: AWS > S3 > Permissions > Bucket policy
{
    "Version": "2008-10-17",
    "Statement": [
        {
            "Sid": "AllowPublicRead",
            "Effect": "Allow",
            "Principal": {
                "AWS": "*"
            },
            "Action": "s3:GetObject",
            "Resource": "arn:aws:s3:::YOUR-S3-BUCKET-NAME/*"
        }
    ]
}
