# HyperFlow fargate worker

Usage:
- Set AWS credentials using `TF_VAR_aws_access_key` and `TF_VAR_aws_secret_key`
- run `terraform init`
- run `terraform apply` to create a HyperFlow Fargate worker with generic executor 
- set `SERVICE_URL` to the output of Terraform (load balancer URL)
- run the test workflow (not yet working):
```
BUCKET="<S3_Bucket_name>" PATH="<bucket path>" S3_FILE=<S3 file name>" hflow run . 
```

