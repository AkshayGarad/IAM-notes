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