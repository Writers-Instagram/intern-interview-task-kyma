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
