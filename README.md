# lab-week4-terraform

## Generate a new SSH key
1. Use command `ssh-keygen` and create a new key-pair
1. In `scripts/cloud-config.yaml`, set the value of the public key under the `users.ssh-authorized-keys` section

## Terraform setup and deployment
1. In your project directory, use command `terraform init` to initialize a Terraform project
1. After filling in the resource block parameters, verify with `terraform plan`
1. Use `terraform apply` to create your resources
1. Once finished, use `terraform destroy` to take down your resources

## Connecting to EC2 instance via SSH
1. Use command `ssh -i <keyname> web@<dns-or-pub-ip>` where
    - keyname is the name of your private key file
    - dns-or-pub-ip is the DNS or public IP of the EC2 instance