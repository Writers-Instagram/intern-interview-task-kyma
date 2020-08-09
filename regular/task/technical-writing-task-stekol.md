## Create a ClusterRoleBinding
ClusterRoleBinding grants a user or a group of users the permissions defined in a role.
It holds a list of subjects (users, groups etc.), and a reference to the role being granted.
A ClusterRoleBinding grants permissions to all the namespaces of a cluster. 

To bind a ClusterRole to all the namespaces in your cluster, you use a ClusterRoleBinding.  

### To create a new ClusterRoleBinding  

1. Enter your credentials and log into the Kyma cluster.  
2. Select a namespace.
3. Click the _**Permissions**_ tab in the side bar.
4. Click on _**Create Binding**_ in the right corner of the _**Role Bindings**_ tab.
5. Select the option _**User Group**_, then enter "recruitment" in the _**User Group**_ box.  
 | _**Tip**_: The name must consist of lower case alphanumeric characters, dashes or dots, and must start and end with an alphanumeric character (e.g. 'my-name'). 
6. In the _**Kind**_ drop down menu, select "ClusterRole".
7. Select "kyma-edit" in the _**Role**_ drop down menu.
8. Click on _**Save**_ to create a ClusterRoleBinding.


## Namespace


