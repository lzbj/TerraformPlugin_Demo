# Terraform Plugin_Demo
A sample app to demo how to implement Terraform Plugin. The purpose
is to try to integrate Terraform with [wskdeploy](https://github.com/apache/incubator-openwhisk-wskdeploy)
so in the sample main.tf, we added a sample yaml path. Change the path to your
local wskdeploy yaml file instead.


# How to
This section describe how to build and run this demo app.

## Install Go
For how to install go, please refer [golang web site](https://golang.org)

## Install terraform.
For how to install terraform, please refer [terraform website](https://www.terraform.io)

## Build and run
Run the below command to get all the dependencies:
`go get . `

Then run:
`go build -o terraform-provider-example` to generate a plugin which
will be invoked by terraform.

You can get it directly as the terraform-provider-example bin in this repo.

Then run:
`terraform plan` to see the config details.

Run command:
`terraform apply` to deploy the manifest yaml file.

# Next Steps:
We could add more config tags and implement the code logic to support such as update, delete etc, By
defining new terraform style tags or we could use yaml instead.


