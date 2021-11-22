


# WHAT IS EC2 AUTOSCALING ?

Auto Scaling helps you maintain application availability and allows you to dynamically scale your Amazon EC2 capacity up or down automatically, according to conditions you define.

Amazon Web service provides Amazon EC2 Auto Scaling services to overcome this failure. Auto Scaling ensures that Amazon EC2 instances are sufficient to run your application. You can create an auto-scaling group which contains a collection of EC2 instances. You can specify a minimum number of EC2 instance in that group and auto-scaling will maintain and ensure the minimum number of EC2 instances. You can also specify a maximum number of EC2 instances in each auto scaling group so that auto-scaling will ensure instances never go beyond that maximum limit.

![autoscaling](https://user-images.githubusercontent.com/54776422/142845510-6c82d7e8-51d4-4dd0-8c6f-b63aa0fa7890.jpeg)

You can also specify desired capacity and auto-scaling policies for the Amazon EC2 auto-scaling. By using the scaling policy, auto-scaling can launch or terminate the EC2 instances depending on the demand.

# AUTOSCALING COMPONENTS

# 1.Launch Configuration 2. Auto scaling Group 3. Auto scaling Policy

1. Launch Configuration (WHAT) : AMI, INSTANCE TYPE, SCURITY GROUPS AND ROLES

2. Auto Scaling Group (WHERE)  : VPC AND SUBNETS, LOAD BALANCERS, MINIMUM INSTANCES, MAXIMUM INSTANCES AND DESIRED CAPACITY

3. Auto Scaling Policy (WHEN)  : SCHEDULED, ON-DEMAND, SCALE-OUT POLICY AND SCALE-IN POLICY

# DYNAMIC AUTO SCALING :

A dynamic scaling policy instructs Amazon EC2 Auto Scaling to track a specific CloudWatch metric, and it defines what action to take when the associated CloudWatch alarm is in ALARM. The metrics that are used to trigger an alarm are an aggregation of metrics coming from all of the instances in the Auto Scaling group. (For example, let's say you have an Auto Scaling group with two instances where one instance is at 60 percent CPU and the other is at 40 percent CPU. On average, they are at 50 percent CPU.) When the policy is in effect, Amazon EC2 Auto Scaling adjusts the group's desired capacity up or down when the alarm is triggered.


![DYNAMIC](https://user-images.githubusercontent.com/54776422/142850616-26750bd2-15f6-43a9-9e3f-0b205d8d58d5.jpg)
