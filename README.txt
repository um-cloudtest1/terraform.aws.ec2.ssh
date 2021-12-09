Based on https://jhooq.com/terraform-ssh-into-aws-ec2/
Ran again on 12/9/21 # succeeded
ssh -i aws4.pem ubuntu@54.149.33.214  
# Look in terraform.tfstate to find the public IP address.
# Note the aws4.pem is an AWS generated private key that I enabled.
# To use a different key, change the line '"key_name": "aws4"' in main.tf accordingly.
# Then I did "tf destroy" to kill the instance.  ("tf" is my alias for terraform.)

