# Knative Camel Operator v0.7.1

This guide walks cluster administrators through installing the Knative Camel Operator in an OpenShift Container Platform cluster. As a cluster administrator, you can install the Knative Camel add-on from the OperatorHub using the OpenShift Container Platform web console. 

The Knative Camel add-on allows you to to install Camel Sources from the Developer Catalog.

## Prerequisites

The following must be installed and running on your cluster:
* [Knative Eventing](/versions/v071/knative-serving-v071-OCP-41.md)
* [Knative Serving](/versions/v071/knative-serving-v071-OCP-41.md)
* [Camel K](https://camel.apache.org/staging/camel-k/latest/index.html)


------
## Installing the Knative Camel Operator

1. Go to **Catalog > OperatorHub**. A list of operators for OpenShift, provided by Red Hat as well as a community of partners and open-source projects is available. Use the **Filter by Keyword** box to facilitate the search of the Knative Camel Operator in the catalog.  

2. Click on the **Knative Camel** tile.

![KACO Tile](/images/camel-tile-highlighted.png)

3. Click **Continue** in the `Show Community Operator` dialog box to proceed. 

4. The **Knative Camel Operator** descriptor screen will appear. Click **Install**.

![KACO Install](/images/camel-install.png)

5. On the **Create the Operator Subscription** screen
    - Go to the **Installation Mode** section and choose the default selection. 
    - Click  **Subscribe**.

![KACO Default](/images/kafka-default.png)

6. Confirm the subscription for the installation operator, by viewing the **Subscription Overview**. Observe as the **UPGRADE STATUS** goes for `0 Installing` to `1 Installed`.

![KACO Subscribe](/images/camel-subscription-installed.png)

7. Confirm the operators are installed by navigating to **Catalog > Operator Management** viewing the **Operator Subscriptions** tab.

![KACO Subscriptions](/images/camel-operator-subscriptions.png)



------
## Uninstalling the Knative Camel Operator 

1. Go to **Catalog > OperatorHub** 

2. Click on the **Knative Camel Operator** tile.

> **NOTE:** The operator tile will indicate it is installed.
 
3. Click **Uninstall** on the **Knative Camel Operator** descriptor screen.

4. In the **Remove Operator Subscription** dialog box
    - Select **Also completely remove the Operator from the selected namespace**
    - Click **Remove**. The Knative Camel Operator subscription is now removed.

