# Grant Permission to the Amazon WorkDocs API for a Developer on the AWS Account<a name="wd-iam-sameacct"></a>

As an IAM administrator if you want to grant Amazon WorkDocs API access to an IAM user from the same AWS account, you will need to create a Amazon WorkDocs API permission policy and attach it to the IAM user\. The following is a sample Amazon WorkDocs API policy that grants permission to read\-only APIs \(List and Describe APIs\)\.

```
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "WorkDocsAPIReadOnly",
            "Effect": "Allow",
            "Action": [
                "workdocs:Get*",
		    "workdocs:Describe*"
            ],
            "Resource": [
                "*"
            ]
        }
    ]
}
```