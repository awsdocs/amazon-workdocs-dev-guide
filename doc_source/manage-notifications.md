# Managing Notifications for an IAM User or a Role<a name="manage-notifications"></a>

IAM Administrators can enable or disable notifications in Amazon WorkDocs through the IAM Console\. Note that even if there is an explicit allow policy attached to a user or role granting access to Notification APIs, for example by adding `workdocs:CreateNotificationSubscription` in the allowed action, Administrators still have to explicitly enable Notifications for this specific User or Role ARN through the IAM console\.

Unless Notifications are explicitly enabled for a user or a role ARN through the IAM console, the applications using the user or role credentials would not be able to make calls to `CreateNotificationSubscription` to subscribe and receive notifications\.

**To enable notifications**

1. Open the Amazon WorkDocs console at [https://console\.aws\.amazon\.com/zocalo/](https://console.aws.amazon.com/zocalo/)\.

1. On the **Manage Your WorkDocs Sites** page, select the desired directory and choose **Actions** and then **Manage Notifications**\.

1. On the **Manage Notifications** page, choose **Enable Notifications**\.

1. Enter the ARN for the user or role you want to allow to receive notifications from your Amazon WorkDocs site\.

**To disable notifications**

1. Open the Amazon WorkDocs console at [https://console\.aws\.amazon\.com/zocalo/](https://console.aws.amazon.com/zocalo/)\.

1. On the **Manage Your WorkDocs Sites** page, select the desired directory and choose **Actions** and then **Manage Notifications**\.

1. On the **Manage Notifications** page, select the ARN that you wish to disable notifications for and choose **Disable Notifications**\.