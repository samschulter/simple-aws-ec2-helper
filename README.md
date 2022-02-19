# simple-aws-ec2-helper

## Assumptions

- Each instance has the tag `Name` and a unique value! This tag is used to identify instances
- All instances are running Ubuntu with user name `ubuntu`
- You have a `.pem` file to connect to EC2 instances
- You know your `Access key ID`, `Secret access key` and your `region` to configure `aws` cli


## Install

Requirements:
- `brew install jq`

Configure:
- `export AWS_PEM_FILE_PATH=absolute/path/to/your/.pem/file`
- Run `aws configure` and enter `Access key ID`, `Secret access key` and `region`


## Usage

- List instance names: `ec2list`
- Start/stop instances: `ec2{start/stop} <instance-name>`
- SSH to instance: `ec2ssh <instance-name>`
