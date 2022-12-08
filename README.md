# AWS switch role

If you have multile roles in multiple AWS accounts,
it's tedius to switch between roles in AWS CLI.

This script makes it easier to select a role.

## Usage
```
Usage:
$ assume-role 
```

![select-a-role](https://user-images.githubusercontent.com/193891/183918204-d94de389-09cd-4ee2-aeb0-86f779ffcb78.png)

## Configuration file: ~/.aws/assume-role.conf
```
account1 arn:aws:iam::012345678901:role/xxxxxx-role
account1 arn:aws:iam::012345678901:role/yyyyyy-role
account1 arn:aws:iam::012345678901:role/zzzzzz-role
account2 arn:aws:iam::123456789012:role/abcdef-role
account3 arn:aws:iam::987654321098:role/opqrst-role
```

## Funding
This work is partially funded by [Linkbal Inc.](https://linkbal.co.jp/)
