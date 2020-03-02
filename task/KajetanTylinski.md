## Create a ClusterRoleBinding
**Follow these steps:**

1. Access and log into the ```Kyma``` cluster using the necessary credentials.

2. Click on the **Permissions** tab.

3. Click on **Create Binding** and select the **User Group** option.

4. Enter ```recruitment``` in the **User Group** box.

5. Select the ```ClusterRole``` Kind.

6. Select the ```Edit``` Role.

7. Press **save** to create the ClusterRoleBinding.

## What is a Namespace

Namespaces are objects which allow you to partition single Kubernetes clusters into smaller virtual clusters. Namespaces make sure that each resource has a unique name within a large cluster. The name of a resource needs to only be unique in a single Namespace. Namespaces can be used to, for example, share a cluster and its resources with other users working on the same project.