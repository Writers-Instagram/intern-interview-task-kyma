## Create a ClusterRoleBinding
ClusterRoleBinding grants the permissions defined in a role 
to a user or set of users. 
holds a list of subjects (users, groups, or service accounts), 
and a reference to the role being granted. 
A ClusterRoleBinding grants that access cluster-wide.

Alternatively, A RoleBinding can reference a ClusterRole and bind that ClusterRole to the namespace of the RoleBinding.

If you want to bind a ClusterRole to all the namespaces in your cluster, you use a ClusterRoleBinding. 

The name of ClusterRoleBinding object must be a valid path segment name.  

### To create a ClusterRoleBinding  

1. Enter your credentials and log into the Kyma cluster.  
2. Select the desired namesspace.
3. Click the _**Permissions**_ tab in the side bar.
4. Click on _**Create Binding**_ in the right corner of the _**Role Bindings**_ tab.
5. Select the option _**User Group**_ and enter "recruitment" in the _**User Group**_ box.  
 | **Tip**: The name must consist of lower case alphanumeric characters, dashes or dots, and must start and end with an alphanumeric character (e.g. 'my-name'). 
6. In the _**Kind**_ drop down menu, select "ClusterRole".
7. Select "kyma-edit" in the _**Role**_ drop down menu .
8. Click on **Save**_ to create a ClusterRoleBinding.


Namespace


