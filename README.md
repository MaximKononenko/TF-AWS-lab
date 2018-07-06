# terraform_lab
https://www.terraform.io/intro/getting-started/build.html

example.tf
provider "aws" {
  region     = "us-east-1"
}

resource "aws_instance" "example" {
  ami           = "ami-2757f631"
  instance_type = "t2.micro"
}

terraform init
terraform apply
terraform show
terraform destroy

https://www.terraform.io/docs/provisioners/connection.html