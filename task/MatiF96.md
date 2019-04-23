# Recruitment task

## Create ClusterRoleBinding
Follow these steps to create a ClusterRoleBinding and bind the group to the selected role:
1. Access the [Kyma cluster](https://console.recruitment.kyma.pro/) using your credentials.
  >**NOTE:** The password and email are encoded with base64. [Decode](https://www.base64decode.org/) the credentials before use.

2. Go to the **Settings** menu, select **Global Permissions**.

3. Select **Cluster Role Bindings** tab and click **Create Binding**.

4. Enter *User Group* and select *Role* from the list. Then click **Save**.



## Namespaces

Grouping and security units which allows you to divide the cluster into smaller units are called Namespaces. They help to organize objects. You can use them for different purposes, such as development and testing.

This example shows you how to easily create Namespace in Kyma:
```
cat <<EOF | kubectl create -f -
apiVersion: v1
kind: Namespace
metadata:
  name: my-namespace
  labels:
    env: "true"
EOF
```

>**NOTE:** Marking Namespace with ```env: "true"``` label makes it available for users
