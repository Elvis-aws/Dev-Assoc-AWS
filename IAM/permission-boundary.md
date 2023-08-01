
# Types policies
1. Identity-based policies with boundaries – Inline or managed policies that are attached to a user, group of users, 
   or role. Identity-based policies grant permission to the entity, and permissions boundaries limit those permissions.
   The effective permissions are the intersection of both policy types.
2. Resource-based policies – Resource-based policies control how the specified principal can access the resource to 
   which the policy is attached
3. Permission Boundary - AWS supports permissions boundaries for IAM entities (users or roles). A permissions boundary is 
   an advanced feature for using a managed policy to set the maximum permissions that an identity-based policy can grant 
   to an IAM entity. An entity's permissions boundary allows it to perform only the actions that are allowed by both its 
   identity-based policies and its permissions boundaries. IAM permission boundary can only be applied to roles or users, 
   not IAM groups