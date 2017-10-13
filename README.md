# DQ Terraform Demo

Simple proof of concept terraform scripts that will deploy the [UKHomeOffice/dq-packer-demo](UKHomeOffice/dq-packer-demo) built ami to an instance and setup a security group that allows http traffic

Requires the env vars `TF_VAR_aws_access_key` and `TF_VAR_aws_secret_key` to be set

Build is automated with drone, and will only `terraform deploy` on commits/merges to master but will always plan on pushes with output visible in drone.