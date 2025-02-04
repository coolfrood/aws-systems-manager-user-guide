# How Systems Manager works<a name="how-it-works"></a>

Diagram 1 below shows a general example of the different processes that AWS Systems Manager performs when performing an action such as sending a command to your fleet of servers or performing an inventory of the applications running on your on\-premises servers\. Each Systems Manager capability, uses a similar process of set up, launching, processing, and reporting\. For example, Run Command and Maintenance Windows are each capabilities of Systems Manager\.

1. **Configure Systems Manager** – Use the Systems Manager console, SDK, AWS Command Line Interface \(AWS CLI\), or AWS Tools for Windows PowerShell to configure, schedule, automate, and run actions that you want to perform on your AWS resources\. 

1. **Verification and processing** – Systems Manager verifies the configurations, including permissions, and sends requests to the AWS Systems Manager SSM Agent running on your instances or servers in your hybrid environment\. SSM Agent performs the specified configuration changes\.

1. **Reporting** – SSM Agent reports the status of the configuration changes and actions to Systems Manager in the AWS Cloud\. Systems Manager then sends the status to the user and various AWS services, if configured\.

**Diagram 1: General example of Systems Manager process flow**

![\[Diagram showing how Systems Manager capabilities, for example Run Command or Maintenance Windows, use a similar process of set up, launching, processing, and reporting.\]](http://docs.aws.amazon.com/systems-manager/latest/userguide/images/how-it-works.png)