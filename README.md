# opsdroid skill aws

A skill for [opsdroid](https://github.com/opsdroid/opsdroid) to interact with AWS.

## Requirements

You need an AWS account and the apiai parser configured.

## Configuration

```yaml
skills:
  - name: aws
    aws_access_key_id: ABCDEF123456789
    aws_secret_access_key: ZYX987654321abc678910
```

## Usage

#### `how many servers are running?`

Checks how many ec2 instances are running.

> user: how many servers are running?
>
> opsdroid: There are 26 servers running

#### `what instances are running?`

Lists ec2 instances.

> user: what instances are running?
>
> opsdroid:
  
```
+-------------------+-------------------+---------+----------------+--------+
| Name              | ID                | State   | IP             | Uptime |
+-------------------+-------------------+---------+----------------+--------+
| instancename      | i-23456789        | running | 12.34.56.78    | 3d     |
+-------------------+-------------------+---------+----------------+--------+
```

## License

GNU General Public License Version 3 (GPLv3)
