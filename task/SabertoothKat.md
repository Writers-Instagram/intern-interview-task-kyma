## Create ClusterRoleBindings
Follow these steps to bind clusters with roles:
1. Access the Console UI of your Kyma cluster.
2. Navigate to the **Settings** section. 
3. Click **Global Permissions**.
4. Click **+ Create Binding**.
5. Define the **UserGroup** name and then select the **Role** from the pull-down menu in the dialog box.  
For example, name the group **recruitment** and bind it to the **edit** role.
6. Click the **Save** button.
## Namespaces

Namespaces are virtual units in Kubernetes that exist within a physical cluster, logically independent from each other. They can help teams with organization, security and performance.

Think of them as the target consumers of the power output provided by an electricity power plant. 
The power plant is a "physical cluster with limited output", and can produce power for different consumer purposes: households, schools, factories etc. The consumers can be seen as the "virtual units" or Namespaces. They use the same energy resources, but for a different purpose.

Similarly, users can create Namespaces (for example, **production**, **development** or **qa** environments) based on their network policies and resource quotas.
