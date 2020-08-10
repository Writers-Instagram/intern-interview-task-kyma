## Create a ClusterRoleBinding
ClusterRoleBinding grants a user or a group of users the permissions defined in a role.  
It holds a list of subjects (users, groups, etc.), and a reference to the role being granted.  
A ClusterRoleBinding grants permissions to all namespaces of a cluster.  

### To create a new ClusterRoleBinding  

1. Enter your credentials and log into your Kyma account.  
2. Select a namespace.
3. Click the _**Permissions**_ tab in the side bar.
4. Click on _**Create Binding**_.
5. In the _**Create Binding**_ window, select the option _**User Group**_.
6. Enter the name "recruitment" in the _**User Group**_ box.  
 | _**Tip**_: The name must consist of lower case alphanumeric characters, dashes or dots, and must start and end with an alphanumeric character (e.g. 'my-name').
7. As _**Kind**_, select "ClusterRole" in the drop down menu.
8. As _**Role**_, select "kyma-edit".
9. Click on _**Save**_ to create a new ClusterRoleBinding.  
  
    
    
## Namespace

A namespace is a cluster of names. It ensures that all the objects of a cluster have unique names so that they can be clearly identified. 
Namespaces are a way of sharing cluster resources among multiple users. This way, users across multiple teams can access these resources and work on the same projects.