# Cloud-watch-metrics
This is a short project showing the Cloud watch metrics
# What is AWS CloudWatch?

AWS CloudWatch is a powerful monitoring and observability service provided by Amazon Web Services. It enables you to gain insights into the performance, health, and operational aspects of your AWS resources and applications. CloudWatch collects and tracks metrics, collects and monitors log files, and sets alarms to alert you on certain conditions on the AWS resources. 
It is like a Gatekeeper for AWS which helps in Monitoring, Alerting, Reporting and Logging foe the AWS resources. Using this we can keep track of activities happening on AWS account.

## Advantages of AWS CloudWatch:

**Comprehensive Monitoring:** CloudWatch allows you to monitor various AWS resources such as EC2 instances, RDS databases, Lambda functions, and more. You get a unified view of your entire AWS infrastructure. We can do monitoring for AWS Infra as well as for applications deployed on AWS.

**Real-Time Metrics:** It provides real-time monitoring of metrics, allowing you to respond quickly to any issues or anomalies that might arise. Metrics like CPU utilization, memory usage, API calls.

**Automated Actions:** With CloudWatch Alarms, you can set up automated actions like triggering an Auto Scaling group to scale in or out based on certain conditions.

**Log Insights:** CloudWatch Insights lets you analyze and search log data from various AWS services, making it easier to troubleshoot problems and identify trends.

**Dashboards and Visualization:** Create custom dashboards to visualize your application and infrastructure metrics in one place, making it easier to understand the overall health of your system.

## Issues solved by Cloud Watch:
CloudWatch helps address several critical challenges.
* **Resource Utilization:** Tracking resource utilization and performance metrics to optimize your AWS infrastructure efficiently.
* **Proactive Monitoring:** Identifying and resolving issues before they impact your applications or users.
* **Troubleshooting:** Analyzing logs and metrics to troubleshoot problems and reduce downtime.
* **Scalability:** Automatically scaling resources based on demand to ensure optimal performance and cost efficiency.


## Cloud Watch can perform these actions

**Auto Scaling:** CloudWatch can trigger Auto Scaling actions based on defined thresholds. For example, you can automatically scale in or out based on CPU utilization or request counts.

**Resource Monitoring:** Monitor EC2 instances, RDS databases, DynamoDB tables, and other AWS resources to gain insights into their performance and health.

**Application Insights:** Track application-specific metrics to monitor the performance of your applications and identify potential bottlenecks.

**Log Analysis:** Use CloudWatch Logs Insights to analyze log data, identify patterns, and troubleshoot issues in real-time.

**Billing and Cost Monitoring:** CloudWatch can help you monitor your AWS billing and usage patterns, enabling you to optimize costs.



There are 2 tasks I am performing on Cloud Watch

# Task 1 - Using Default metrics, How to send out alarms for CPU utilization
* How to configure a Alarm for CPU utilization. 
* If the CPU utilization reaches above the set limit/threshold, how to setup alarm, and send the notification depending on the Default metrics

# Task 2 - Custom metrics
* How to write application that can trigger custom metrics.

## Cloud watch features 
1. Monitoring
2. Real-time metrics
3. Alarms
4. Log Insights
5. Custom metrics
6. Cost Optimization - Integrate Cloud watch with Lambda functions, helps to identify un-used resources and delete them, helps in cost optimization
7. Scaling  - If CPU utilization is 80%, Cloud watch sends notification to Auto scaling group to scale the EC2 instance. 

Using Log groups - Cloud Watch creates a group for a every AWS every or every application that is deployed, so that it groups all the logs of that application


Task 1 : A python script to spike the EC2 CPU usage
* I have created a EC2 instance, written a python script to spike the CPU usage on that EC2 instance.
* I will use Cloud Watch to see the CPU utilization metrics for that instance.
* By default EC2 instance sends metrics  every 5 min. 
* In Cloud watch, using SNS - Simple Notification Service, we can send emails/notifications for the alarms















