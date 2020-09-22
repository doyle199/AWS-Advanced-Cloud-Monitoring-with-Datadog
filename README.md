# AWS-Monitoring-with-Datadog
AWS Monitoring with Datadog

Go to the following link and click on free trial: https://www.datadoghq.com

![alt text](https://github.com/doyle199/AWS-Advanced-Cloud-Monitoring-with-Datadog/blob/master/datadog1.png)

Enter your information and click sign up. On step two, choose AWS and click next. Navigate to AWS EC2 and select a Linux instance. On the choose instance type page, choose a size and click configure instance.

![alt text](https://github.com/doyle199/AWS-Advanced-Cloud-Monitoring-with-Datadog/blob/master/AMI.png)

On the configure instance page, choose the correct subnet and enable auto-assign Public IP, and click next add storage.

![alt text](https://github.com/doyle199/AWS-Advanced-Cloud-Monitoring-with-Datadog/blob/master/configure1.png)

Click next: add tags. Click next: configure security group.	Select or make a security groups with the correct access and click review and launch.

![alt text](https://github.com/doyle199/AWS-Advanced-Cloud-Monitoring-with-Datadog/blob/master/SG.png)

Click launch, choose a key pair, check the acknowledgment box and click launch instances.

![alt text](https://github.com/doyle199/AWS-Advanced-Cloud-Monitoring-with-Datadog/blob/master/keypair.png)

Connect to the instance via CLI. Update instance.

![alt text](https://github.com/doyle199/AWS-Advanced-Cloud-Monitoring-with-Datadog/blob/master/AMI2.png)

Run the following command to install the Datadog instance on the AMI "DD_AGENT_MAJOR_VERSION=7 DD_API_KEY=KEY-HERE DD_SITE="datadoghq.com" bash -c "$(curl -L https://s3.amazonaws.com/dd-agent/scripts/install_script.sh)"

![alt text](https://github.com/doyle199/AWS-Advanced-Cloud-Monitoring-with-Datadog/blob/master/connect.png)

Navigate back to the Datadog setup and click next.

![alt text](https://github.com/doyle199/AWS-Advanced-Cloud-Monitoring-with-Datadog/blob/master/congrats.png)

Click install integration.

![alt text](https://github.com/doyle199/AWS-Advanced-Cloud-Monitoring-with-Datadog/blob/master/integration.png)

Click the configuration tab and then the automatically using CloudFormation button.

![alt text](https://github.com/doyle199/AWS-Advanced-Cloud-Monitoring-with-Datadog/blob/master/config1.png)

This sends one to CloudFormation. Go to the following link: https://app.datadoghq.com/account/settings#api. Click the dropdown for API Keys and copy the key.

![alt text](https://github.com/doyle199/AWS-Advanced-Cloud-Monitoring-with-Datadog/blob/master/API%20KEY.png)

Navigate back to CloudFormation and past the key into the DbApiKey box. Leave the defaults, click the acknowledgements, and click create stack.

![alt text](https://github.com/doyle199/AWS-Advanced-Cloud-Monitoring-with-Datadog/blob/master/DdApiKey.png)

![alt text](https://github.com/doyle199/AWS-Advanced-Cloud-Monitoring-with-Datadog/blob/master/stack_1.png)

![alt text](https://github.com/doyle199/AWS-Advanced-Cloud-Monitoring-with-Datadog/blob/master/stacks.png)

For step 4 of the Datadog setup, click finish.

![alt text](https://github.com/doyle199/AWS-Advanced-Cloud-Monitoring-with-Datadog/blob/master/finish.png)

Now one can run advanced AWS metrics in DataDog.

![alt text](https://github.com/doyle199/AWS-Advanced-Cloud-Monitoring-with-Datadog/blob/master/1.png)

![alt text](https://github.com/doyle199/AWS-Advanced-Cloud-Monitoring-with-Datadog/blob/master/2.png)

![alt text](https://github.com/doyle199/AWS-Advanced-Cloud-Monitoring-with-Datadog/blob/master/3.png)


