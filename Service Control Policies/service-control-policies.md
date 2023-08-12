
# Service control policies
- Service control policies (SCPs) are one type of policy that can be used to manage your organization
- SCPs offer central control over the maximum available permissions for all accounts in your organization, allowing you 
  to ensure your accounts stay within your organization’s access control guidelines 
- In SCPs, you can restrict which AWS services, resources, and individual API actions the users and roles in each member 
  account can access
- You can also define conditions for when to restrict access to AWS services, resources, and API actions
- These restrictions even override the administrators of member accounts in the organization 
- If a user or role has an IAM permission policy that grants access to an action that is either not allowed or explicitly 
  denied by the applicable SCPs, the user or role can't perform that action 
- SCPs affect all users and roles in the attached accounts, including the root user 
- SCPs do not affect any service-linked role