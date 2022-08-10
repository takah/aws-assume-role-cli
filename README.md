# Easy role selector for AWS assume-role

If you have multile roles in multiple AWS accounts,
it's tedius to switch between roles in AWS CLI.

This script makes it easier to select a role.

```
Usage:
$ assume-role 

===== Choose a role in selector =====

Old identity
{
    "UserId": "XXXXXXXXXXXXXXXXXXXXX",
    "Account": "123456789012",
    "Arn": "arn:aws:iam::234567890123:user/xxxxx@example.com"
}
Copy and paste to Run the lines below in your shell

export AWS_ACCESS_KEY_ID=xxxxxxxxxxxxxxxxxxxx
export AWS_SECRET_ACCESS_KEY=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
export AWS_SESSION_TOKEN=xxxxxxxxxxxxx...(snip)...xxxxxxxxxxxxxxx

echo Current identity
aws sts get-caller-identity
```

## Configuration file: ~/.aws/assume-role.conf
```
account1 arn:aws:iam::012345678901:role/xxxxxx-role
account1 arn:aws:iam::012345678901:role/yyyyyy-role
account1 arn:aws:iam::012345678901:role/zzzzzz-role
account2 arn:aws:iam::123456789012:role/abcdef-role
account3 arn:aws:iam::987654321098:role/opqrst-role
```
