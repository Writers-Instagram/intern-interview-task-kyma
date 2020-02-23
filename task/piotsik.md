## Create ClusterRoleBinding

This tutorial is intended for people who want to learn how to create ClusterRoleBinding.  
Follow this instruction to bind **edit** role with **recruitment** group:

1. Sign into [Kyma cluster](https://console.kyma-1-10.kyma-goat.ga/) using your login credentials.
2. Navigate the sidebar panel on the left side of the console.
3. Click **Settings > Global Permissions** and make sure you're on **Cluster Role Binds** tab.
4. Press **Create Binding** button.
5. In the pop-up window choose **User group**.
6. Fill in the fields with the following values:

|User Group |Role |
|:---------:|:---:|
|recruitment|edit |

>**TIP**: You may also choose a role from a drop-down list.

7. Save your binding using **Save** button.


## Namespaces

Namespace, also called _name scope_, is an abstract space which consists of names, symbols and words. They are used to distinguish same names or objects but in different context. Within a name scope every element must be unique to avoid naming collisions.  
In **Kyma** users can choose different functionalities for their services and lambda functions using namespaces.

Example below can help you understand that better:

```go
package main

import "fmt"

func main() {
	var a int = 7
    
	fmt.Println("Hello!")  // 'Println' is in "fmt" package namespace

	write()
}

func write() {
	var b int = 3
   	
    fmt.Println(b)  // This alone will work
	fmt.Println(a)  // It will return an error because 'a' is defined only in 'main' function scope
}

```

- Calling variables outside their namespace _(such as function)_ results in an error.
- Using `Println` without `fmt` prefix fails because it calls a function which does not exist in a global scope. Although it is defined in **fmt** package, therefore by adding prefix it will work.

