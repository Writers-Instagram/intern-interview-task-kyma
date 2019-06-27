ClusterRoleBinding
---

To create a `ClusterRoleBinding`: 

1. Log in to the Kyma interface 
2. In the sidebar on the left, go to **Settings** > **Global Permissions**
3. Click on **+ Create Binding**  
4. Select the **Group/User** and **Role** you wish to bind
5. Click on **Save** 

You can view the binding in the list under Permissions. 

To **delete** a `ClusterRoleBinding`, select it from the list and click on Delete: 

![Screenshot](https://i.imgur.com/ThiA7J4.png)


Namespaces
---

Namespaces in Kubernetes or Kyma provide a wider scope for names (similarly to namespaces in C# or C++).

>**Note:** Namespaces are **virtual clusters** that exist within the **same** physical cluster.

Namespaces are useful for large organizations when naming conflicts begin to arise. They can also help with security and performance, for example: 

**Problem:** Several users share a cluster, but you don't want them to have access to the same cluster resources.

**Solution:** Create separate Namespaces and assign each user different permissions within different Namespaces.
