terraform-provider-terraform
============================

This repository contains a separated version of [the `terraform` provider](https://www.terraform.io/docs/providers/terraform/index.html) that can be used with 0.10.x releases of Terraform Core.

Prior to 0.10, and from 0.11 onwards, this provider is [an integrated part of Terraform Core](https://github.com/hashicorp/terraform/tree/master/builtin/providers/terraform) and no longer packaged as a provider plugin.

No further development of this provider will occur in this repository, with future changes instead being made in the Terraform Core repository. Please do not open new issues or pull requests against this repository: instead, open them in [the Terraform Core repository](https://github.com/hashicorp/terraform).

Requirements
------------

-	[Terraform](https://www.terraform.io/downloads.html) 0.10.x
-	[Go](https://golang.org/doc/install) 1.8 (to build the provider plugin)

Building The Provider
---------------------

Clone repository to: `$GOPATH/src/github.com/hashicorp/terraform-provider-$PROVIDER_NAME`

```sh
$ mkdir -p $GOPATH/src/github.com/hashicorp; cd $GOPATH/src/github.com/hashicorp
$ git clone git@github.com:hashicorp/terraform-provider-$PROVIDER_NAME
```

Enter the provider directory and build the provider

```sh
$ cd $GOPATH/src/github.com/hashicorp/terraform-provider-$PROVIDER_NAME
$ make build
```
