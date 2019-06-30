## Role Based Access Control (RBAC) in Kyma

RBAC is the process of granting access to a user or group of users to a Kubernetes cluster or a particular namespace within the cluster. 
In order to provide different levels of access a particular role specific to a namespace must be defined.

Roles are actionable verbs for each user or group of users e.g. edit, admin, dex-role etc. Access can be granted within a namespace 
using RoleBinding, or a cluster-wide access is possible through ClusterRoleBinding. 
See [this](https://kyma-project.io/docs/components/security/#overview-overview) document to learn more about CluterRoleBinding.

To create a ClusterRoleBinding following these steps:

![ClusterRoleBinding](https://github.com/SaraZahid/intern-interview-task-kyma/blob/master/task/assets/screenshot-clusterrolebinding.png)

1. Open your Kyma cluster, Click > **Global Permissions**
2. Click > **Create Binding**
3. Click > **User Group**
4. Type **recruitment** in User Group name
5. Select **edit** role 
6. Click > **Save**

## Namespaces in Kyma and Kubernetes

Kyma namespaces provide a mechanism to scope the resources in a cluster. Namespaces are like virtual clusters inside your Kubernetes cluster. Namespaces are objects which partition a single Kubernetes cluster into multiple virtual clusters.  Multiple namespaces can be created within a single cluster while keeping them logically isolated from each other.

Users can create a namespace from the Kyma Dashboard. Namespaces can be limited or expanded through resource constraints e.g. memory allocation and limits per container. See [this](https://kubernetes.io/docs/concepts/overview/working-with-objects/namespaces/) document to learn more about namespaces.

Common use cases of namespaces are as follows:

### Use Case 1

Users can separate/isolate a development test system from a production environment in a Kubernetes cluster by creating two namespaces **test** and **production**. The **test** namespace can contain a pod, role binding user group **developers** with minimal resource allocation to test the deployment. Whereas, the **production** namespace could contain a role binding **admins**, enabling admins to manage pods and containers inside this environment.

### Use Case 2

For instance, ```component-a``` and ```component-b``` need to be scaled differently inside the cluster due to resource requirements and traffic, but occasionly ```component-a``` needs to rely on ```component-b```. In this case, separate namespaces ```component-a``` and ```component-b``` can be created while scaling them separately as required. Services in Kubernetes expose their endpoint using a common DNS pattern, such as:
```
<Service name>.<Namespace Name>.svc.cluster.local
```
So, ```component-a``` can request services of ```component-b``` using the address:
```
servicename.component-a
```
Similarly, ```component-b``` can also request services of ```component-a```. Thus, by using namespaces different components of a service can scale separately and also call each other if and when required. 
