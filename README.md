USING TERRFORM TO DEPLOY LAMBDA AND CLOUDWATCH 

Instruction: 

Open Check_file_lambda.py to change s3 bucket name

Run The following commands: 

pip install virtualenv 

virtualenv venv

venv/bin/activate

pip install requirements.txt

terraform init

export AWS_ACCESS_KEY_ID=$(aws configure get terraform-test.aws_access_key_id)

export AWS_SECRET_ACCESS_KEY=$(aws configure get terraform-test.aws_secret_access_key)

export AWS_DEFAULT_REGION=us-east-1

./deploy.sh

