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

### 1. CloudWatch Dashboard
![Dashboard](Dashboard.png)

### 2. Alarm Details (Threshold breached)
![Alarm Details](Alarm_details.png)

### 3. Alarm Notification Email
![Alarm Mail](Alarm_mail.png)

### 4. EC2 Terminal - Before installing stress
![CLI1](CLI1.png)

### 5. EC2 Terminal - Installing stress
![CLI2](CLI2.png)

### 6. EC2 Terminal - stress command running
![CLI4](CLI4.png)

### 7. CloudWatch Dashboard (alarm in triggered state)
![Dashboard 2](dashboard2.png)

## Outcome

This task demonstrated real-time monitoring of AWS EC2 resources using CloudWatch. Alarms were configured, triggered, and verified through both the dashboard and email notifications. The experience helped build confidence in infrastructure monitoring and alerting mechanisms in cloud environments.

## Deliverables

- CloudWatch dashboard screenshots
- Alarm configuration and triggered state
- Email alert proof
- EC2 setup and stress testing screenshots


