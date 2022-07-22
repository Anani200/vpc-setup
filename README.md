# terraform-aws-vpc-configuration-setup

This is a exercise used to assess your approach to development and use of infrastructure as code.

In this example we have a simple VPC network. To run this configuration you can use the commands below:

terraform init
terraform apply -var-file=default.tfvars
This configuration needs to be adapted to become a more robust network architecture.

The AWS us-east-1 region has more than 2 availability zones, and we'd like to make use of one more for our network configuration. Modify the configuration to span 3 AZs.

To improve security and network separation we'd like to have private subnets that are not accessible to the internet. Modify the configuration for subnet b to make it private. Note that private subnets should still be able to egress to the internet.

To further improve security we'd like to have a database subnet that is not addressable from the internet, and also has no access to egress to the internet. Modify the configuration for the subnet you created in step 1 to make it only accessible from the local internal network.

By design, this is a fairly simple exercise, so we're hoping for solutions that reflect what you consider well-factored production-quality code. The best solutions will be elegant, as well as correct. Feel free to reformat the code to make use of terraform best practices in any way you see fit.

When you're finished, submit your solution to us as via Github, Gitlab, Bitbucket, etc. link and our team will review it.
