## Namespaces

# Definition

Namespaces are a concept used by Kubernetes to divide a cluster into several logical units. Namespaces are intended for use in environments with many users spread across multiple teams, or projects. For clusters with a few to tens of users, you should not need to create or think about namespaces at all. Start using namespaces when you need the features they provide.

Namespaces can be used to  By default, namespaces are not isolated from each other. However, there are ways to restrict users and applications to certain namespaces.

Kubernetes supports multiple virtual clusters that are supported by the same physical cluster. These virtual clusters are called namespaces.


# Use Namespaces in your implementations XX diese implementation soll in die definition



Namespaces provide a scope for names. Names of resources need to be unique within a namespace, but not across namespaces. Namespaces cannot be nested inside one another and each Kubernetes resource can only be in one namespace.

Namespaces are a way to divide cluster resources between multiple users (via resource quota).

In future versions of Kubernetes, objects in the same namespace will have the same access control policies by default.

It is not necessary to use multiple namespaces just to separate slightly different resources, such as different versions of the same software: use labels to distinguish resources within the same namespace




Kubernetes resources, such as pods and Deployments, are logically grouped into a namespace.





ddd
