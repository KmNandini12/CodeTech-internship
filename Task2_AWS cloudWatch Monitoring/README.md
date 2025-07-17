# Task 2 – AWS Cloud Monitoring with CloudWatch

## Objective

To configure basic monitoring on an EC2 instance using AWS CloudWatch and demonstrate the triggering of an alarm under simulated load conditions.

## What Was Implemented

- Launched an EC2 instance (Ubuntu) in the AWS Free Tier
- Created a custom CloudWatch dashboard
- Added widgets for metrics like CPUUtilization, NetworkPacketsIn/Out, and CPUCreditUsage
- Created a CloudWatch alarm for CPUUtilization > 15%
- Installed and used the `stress` utility on the EC2 instance to simulate high CPU usage
- Alarm was triggered and a notification was received via email (SNS)

## Tools Used

- AWS CloudWatch
- AWS EC2 (Ubuntu)
- CloudWatch Alarm
- SNS (Simple Notification Service)
- Ubuntu terminal (stress utility)

## Screenshots

Dashboard.png –
Displays the CloudWatch dashboard with real-time metrics for the EC2 instance, including CPUUtilization, CPUCreditUsage, and NetworkOut.

dashboard2.png –
Shows the dashboard when the CPUUtilization alarm is in triggered state, confirming that the alarm activated successfully under load.

Alarm_details.png –
Contains the full alarm configuration including metric name, threshold value (15%), evaluation period, and SNS topic for alert delivery.

Alarm_mail.png –
Screenshot of the email notification received from Amazon SNS when the alarm is triggered, proving that the alert mechanism is working.

CLI1.png –
Initial terminal output after connecting to the EC2 instance, used to verify access and prepare the environment for stress testing.

CLI2.png –
Shows successful installation of the stress utility using apt, required to simulate high CPU usage on the instance.

CLI4.png –
Output of the command stress --cpu 2 --timeout 60, used to artificially raise CPU utilization and trigger the CloudWatch alarm.

## Outcome

This task demonstrated real-time monitoring of AWS EC2 resources using CloudWatch. Alarms were configured, triggered, and verified through both the dashboard and email notifications. The experience helped build confidence in infrastructure monitoring and alerting mechanisms in cloud environments.

## Deliverables

- CloudWatch dashboard screenshots
- Alarm configuration and triggered state
- Email alert proof
- EC2 setup and stress testing screenshots


