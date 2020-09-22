# AWS-Advanced-Cloud-Monitoring-with-Datadog
AWS Advanced Cloud Monitoring with Datadog

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
