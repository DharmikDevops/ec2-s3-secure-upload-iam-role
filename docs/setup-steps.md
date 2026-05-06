## Setup Steps

1. Create an S3 bucket
2. Create an IAM Role with S3 permissions
3. Attach the IAM Role to an EC2 instance
4. Connect to the EC2 instance using EC2 Instance Connect
5. Create a file:
   echo "Hello from EC2" > test.txt
6. Upload file to S3:
   aws s3 cp test.txt s3://your-bucket-name/
7. Verify file in S3 bucket
