# AWS Cloud Security Engineering Lab

## Project Overview
Built a hands-on AWS cloud security lab focused on
identity management, network security, auditing,
and security monitoring.

## Technologies Used
- AWS IAM
- IAM Policy Simulator
- Amazon VPC Security Groups
- AWS CloudTrail Event History
- Amazon CloudWatch Logs
- CloudWatch Metric Filters
- CloudWatch Alarms
- AWS CLI
- Linux

## Security Controls Implemented

### 1. IAM Least Privilege
Created an S3 bucket-listing policy and tested
allowed and implicitly denied permissions.

### 2. Network Security
Created a dedicated security group.
Removed unrestricted outbound access.
Configured outbound HTTPS access on TCP port 443.

### 3. CloudTrail Auditing
Investigated AWS API activity associated with
security group configuration changes.

### 4. CloudWatch Monitoring
Created a security log group with 7-day retention.
Configured a metric filter for security group changes.
Tested matching and nonmatching log events.

### 5. CloudWatch Alarm
Created a metric alarm and simulated an ALARM state.

## Important Limitations
CloudTrail was not connected to the CloudWatch log group.
The monitoring pipeline was not tested end-to-end.
The alarm did not have notification actions configured.

## Security Concepts Demonstrated
- Principle of least privilege
- Network access control
- Security configuration validation
- Audit logging
- Event filtering
- Security monitoring
- Incident response fundamentals
