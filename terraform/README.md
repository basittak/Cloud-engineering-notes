# Terraform

Terraform helps you declare infrastructure in code. These notes include best practices and a few patterns I use daily.

How to use this folder
- Read `terraform-basics.md` for the core workflow (init, plan, apply).
- Follow `terraform-aws-pattern.md` to learn safer remote-state patterns and CI integration.

Practical tip: Commit your `.tf` files but never commit the `terraform.tfstate` file — use a remote backend instead.
