# IAM Notes
## 9. What IAM permissions are needed to use CDK Deploy?
To use CDK Deploy, the following AWS Identity and Access Management (IAM) permissions are required:

1. `cloudformation:CreateStack` - Allows creating a new CloudFormation stack.

2. `cloudformation:DescribeStacks` - Allows retrieving information about an existing CloudFormation stack.

3. `cloudformation:DescribeStackEvents` - Allows retrieving events related to a CloudFormation stack.

4. `cloudformation:GetTemplate` - Allows retrieving the template for a CloudFormation stack.

5. `cloudformation:UpdateStack` - Allows updating an existing CloudFormation stack.

6. `cloudformation:DeleteStack` - Allows deleting a CloudFormation stack.

You can assign these permissions to a user or a group in IAM using policies. For example, you could create a policy with these permissions and attach it to a group that your user is a member of. It is recommended to grant the minimum set of permissions required to perform the required actions to minimize the potential for accidental changes or unauthorized access.

## 10. How to rename an AWS customer IAM policy?
To rename an AWS customer IAM policy, you can follow these steps:

1. Sign in to the AWS Management Console and open the IAM console.

2. In the navigation pane on the left, click on "Policies."

3. Select the policy you want to rename from the list.

4. Click on the "Policy actions" dropdown button and select "Edit policy."

5. In the policy editor, change the policy name in the "Policy name" field at the top of the page.

6. Click on the "Review policy" button to review your changes.

7. Review the policy and ensure that the policy is correct.

8. Click on the "Save changes" button to save the policy with the new name.

Once you've saved the policy with the new name, the policy's ARN (Amazon Resource Name) will remain the same. If you are referencing the policy by its ARN in other parts of your AWS infrastructure, you will need to update those references to reflect the new name.

## 11. Why is IAM important?
Here are some key reasons why Amazon Identity and Access Management (IAM) is
important:
1. IAM allows you to control access to your AWS resources. With IAM, you can create
and manage users and groups, and grant them permissions to access specific AWS
resources or actions. This allows you to control who has access to your resources, and
what they can do with them.
2. IAM helps you enforce the principle of least privilege. This means that you only grant
users and applications the minimum permissions they need to perform their tasks, and
no more. This helps to reduce the risk of unauthorized access to your resources, and to
minimize the potential impact of security breaches.
3. IAM integrates with other AWS services. Many AWS services, such as Amazon EC2
and Amazon S3, support IAM authentication, so you can use IAM to control access to
those services as well. This allows you to manage access to your entire AWS
environment using a single, centralized service.
4. IAM is flexible and scalable. IAM allows you to easily add or remove users and
groups, and to adjust their permissions as needed. This makes it easy to manage
access to your resources as your organization grows and changes.
5. IAM is secure. IAM uses industry-standard encryption and authentication
technologies to protect your resources, and provides a variety of security features,
such as multi-factor authentication and password policies, to help you secure your

## 12. Are root users and IAM users the same?
No, AWS root users and IAM users are not the same. AWS root users are the original users
of an AWS account, with full access to all AWS services and resources in the account. Root
users are created when an AWS account is first created, and the email address and password
for the root user are used to sign in to the AWS Management Console.
In contrast, IAM users are separate users that can be created and managed within an AWS
account. IAM users are typically used to give individuals or applications access to specific
AWS services and resources in the account. IAM users are managed through the IAM
service, and they can be granted different levels of access to the AWS resources in the
account through the use of IAM policies.
Root users have full access to all AWS services and resources by default, while IAM users
have no access to any services or resources until specific permissions are granted to them. It's
generally recommended to use IAM users for most tasks, rather than using the root user, to
help ensure the security and integrity of your AWS account.