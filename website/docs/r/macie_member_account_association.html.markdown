---
subcategory: "Macie Classic"
layout: "aws"
page_title: "AWS: aws_macie_member_account_association"
description: |-
  Associates an AWS account with Amazon Macie as a member account.
---

# Resource: aws_macie_member_account_association

~> **NOTE:** This resource interacts with [Amazon Macie Classic](https://docs.aws.amazon.com/macie/latest/userguide/what-is-macie.html). Macie Classic cannot be activated in new accounts. See the [FAQ](https://aws.amazon.com/macie/classic-faqs/) for more details.

Associates an AWS account with Amazon Macie as a member account.

~> **NOTE:** Before using Amazon Macie for the first time it must be enabled manually. Instructions are [here](https://docs.aws.amazon.com/macie/latest/userguide/macie-setting-up.html#macie-setting-up-enable).

## Example Usage

```hcl
resource "aws_macie_member_account_association" "example" {
  member_account_id = "123456789012"
}
```

## Argument Reference

The following arguments are supported:

* `member_account_id` - (Required) The ID of the AWS account that you want to associate with Amazon Macie as a member account.

## Attributes Reference

In addition to all arguments above, the following attributes are exported:

* `id` - The ID of the association.
