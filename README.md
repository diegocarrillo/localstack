# localstack
Sample project to test aws locally

#Pre-requisites
1. docker & docker-compose
2. aws cli v2i (https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2-linux.html)
3. We need to create a profile for the 'fake' aws access
´aws configure --profile localstack´

---
# How to create a bucket
´docker-compose up -d´

´aws s3api --endpoint-url http://localshot:4566 create-bucket --bucket my-first-bucket´

Then we can list that bucket
´aws s3api --endpoint-url http://localhost:4566 list-buckets´


