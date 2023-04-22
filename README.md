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