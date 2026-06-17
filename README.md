1. Create the S3 Bucket & DynamoDB Table
    bucket         = "vivek-234121221-rrn"
    key            = "envs/demo-state/terraform.tfstate"
    encrypt        = true

    dynamodb_table = "tfstate-lock"
    hash_key       = "LockID"   # also called partition key

2. In terminal:
    terraform init -migrate-state