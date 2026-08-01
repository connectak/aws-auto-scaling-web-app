# aws-auto-scaling-web-app
Built a highly available Auto Scaling Web Application on AWS using EC2, Launch Templates, Auto Scaling Groups, CloudWatch Alarms, and Scheduled Scaling.

Overview

This project demonstrates how to build a highly available and scalable web application on AWS using Auto Scaling.

The infrastructure automatically launches additional EC2 instances when CPU utilization becomes high and terminates unnecessary instances when demand decreases.

The project also includes Scheduled Scaling for predictable traffic patterns.

                    Users
                       │
                EC2 Instance
                       │
          Launch Template (AMI)
                       │
            Auto Scaling Group
        Min:1    Desired:1    Max:3
                       │
              CloudWatch Alarm
               CPU >70% / <49%
                       │
        Launch / Terminate Instance

      
