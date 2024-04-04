# Two-Tier Architecture Deployment using AWS CloudFormation 🚀

Deploying a Highly available and fault-tolerant two-tier architecture using AWS CloudFormation.

## Architecture Explanation 📚

The architecture will consists of a web server and a database server. The web server will be hosted on an EC2 instance and the database server will be hosted on an RDS instance. We are going to create a Separate VPC for this architecture. The VPC will have 2 public subnets and 2 private subnets. The web server will be hosted on the public subnet and the database server will be hosted on the private subnet. The EC2 instance will be launched in an AutoScaling Group. The AutoScaling Group will have a minimum of 2 instances and a maximum of 4 instances. The AutoScaling Group will be behind an Application Load Balancer. The RDS instance will be a Multi-AZ deployment.

## Architecture Diagram 📊

![Two-Tier-Architecture-aws-cfn](https://github.com/mathesh-me/two-tier-architecture-aws-cf/assets/144098846/fb7b2a94-241a-47ad-8a41-11c95d263a7a)


## Prerequisites 📋

1. AWS Account
3. IAM User with necessary permissions

## Steps to Deploy Architecture 📝

| Step No | Document Link |
| ------ | ------ |
| 1 | [Create a IAM role for CloudFormation to Deploy Resources][Step-1] |
| 2 | [Create a YAML template for deploying our Architecture][Step-2] |
| 3 | [Create a CloudFormation Stack to Deploy Resources][Step-3] |
| 4 | [Validate our Architecture and it's Working][Step-4] |
| 5 | [Delete the CloudFormation Stack to Delete Resources][Step-5] |

   [Step-1]: <./Steps/step1.md>
   [Step-2]: <./Steps/step2.md>   
   [Step-3]: <./Steps/step3.md>
   [Step-4]: <./Steps/step4.md>
   [Step-5]: <./Steps/step5.md>

## Usage 🛠️

1. Download the `two-tier-architecture.yml` file from the repository.
2. Go to the CloudFormation service in the AWS Management Console.
3. Click on `Create Stack`.
4. Select `Upload a template file` and upload the `two-tier-architecture.yml` file.
5. Click on `Next`.
6. Enter the Stack name and other parameters as per your requirement.
7. Click on `Next`.
8. Click on `Create Stack`.

## Contributing 🤝

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License 📄

This project is licensed under the Apache License - see the [LICENSE](LICENSE) file for details.

## Author

- [Mathesh M](https://www.linkedin.com/in/mathesh-me/) on LinkedIn.
- You Can also check out my [Medium](https://medium.com/@mathesh-me) for articles on DevOps Tools and Technologies.
