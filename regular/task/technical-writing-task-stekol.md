## Create a ClusterRoleBinding
ClusterRoleBinding grants a user or a group of users the permissions defined in a role.
It holds a list of subjects (users, groups etc.), and a reference to the role being granted.
A ClusterRoleBinding grants permissions to all namespaces of a cluster. 

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

A namespace is a set of names that are used to identify and refer to objects.  
A namespace ensures that all the objects of a specific set have unique names so that they can be clearly identified. 

Namespaces are commonly structured as hierarchies to allow reuse of names in different contexts. As an analogy, consider a system of naming of people where each person has a given name, as well as a family name shared with their relatives. If the first names of family members are unique only within each family, then each person can be uniquely identified by the combination of first name and family name; there is only one Jane Doe, though there may be many Janes. Within the namespace of the Doe family, just "Jane" suffices to unambiguously designate this person, while within the "global" namespace of all people, the full name must be used.

The namespace keyword is used to declare a scope that contains a set of related objects. You can use a namespace to organize code elements and to create globally unique types.
