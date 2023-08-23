# Infrastructure as Code (IAC)

Today we are starting to work with Terraform!

The first step is to get setup with Terraform and their AWS Getting Started guide is a great place to start.

Before you get started, here are a couple of guidance points:

**Ignore the section Quick start tutorial**

There is a heading on the Terraform tutorial called **"Quick start tutorial"** that is within the **Install Terraform** section. You can IGNORE the entirety of the **Quick start tutorial** and move straight on to **Build infrastructure** stage.

**Remote state stage**

Ignore the final stage which is the remote state stage. We are going to cover that in more detail later.

**Authenticating terraform for your AWS account**

In the guide it tells you to set the `AWS_ACCESS_KEY_ID` and the `AWS_SECRET_ACCESS_KEY` - this approach would be used if you are using long live credentials (and is a bit insecure as we have already discussed) so instead we can continue to leverage the refresh token and AWS SSO login approach.

Instead of setting the variables as indicated in the terraform guide you should perform the `aws sso login` command approach to authenticate your AWS command line.

Validate that your AWS CLI is authenticated using the usual `aws sts get-caller-identity` approach

Once your AWS CLI is authenticated then we just need to inform terraform of what your AWS profile is called. To do this run the following (replacing the REPLACE_ME section with whatever you called your AWS profile):

```
export AWS_PROFILE="REPLACE_ME"
```

Then you can run the `terraform` commands as indicated through the guide and they should authenticate fine.

**Directories and files**

Make sure to create any directories or files within this repository so that they will be included in your submission

**Screenshots**

Once you have a successful `terraform apply` outcome, take a screenshot showing the output from the command line and a second screenshot showing your EC2 instance running in the console. The screenshots should be placed within this directory.

===

Ok now that you've got a few guidance points here's the link to get started:

[Terraform AWS Getting Started](https://developer.hashicorp.com/terraform/tutorials/aws-get-started)

Once finished, make sure to commit and push your code at this point

**Run `terraform destroy` to remove any resources when you are done!**