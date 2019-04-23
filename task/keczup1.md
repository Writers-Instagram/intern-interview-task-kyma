## Create a ClusterRoleBinding

To create a ClusterRoleBinding search for **Global Permissions** in the navigation bar on the left. In Permissions, go to **Cluster Role Bindings** section and click **Create Binding** button on the right. Insert Group Name and Select Role. Then click **Save**.

If Error occurs, check whether the binding already exists. To do that, click **Search** button and enter the Role or the Group Name. If the row containing the data occurs, the binding already exists.

## Namespaces

A Namespace is a unit which grants you work in smaller units of the cluster to use for development.

To create a Namespace available for Kyma users, mark it with the `env: "true"` label.

Kyma offers some Namespaces ready for you to use:
- production
- qa
- stage
