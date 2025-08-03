# Important
There is a conflicts with resources that only need to be created once:
- "aws_iam_openid_connect_provider" "github"
- The fix is to use "data", but we need to previously create that resource just once

They need to be created first and then never again.

## Todo list

- In order to make this universal, we should make the VITR organisation a variable
- In order to make this universal, we need to use a public EC2 AMI
- We need to see how to do it with the key-pair
