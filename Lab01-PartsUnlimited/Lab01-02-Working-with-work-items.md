## Overview 

* In this lab, you will learn about the agile planning and portfolio management tools and processes provided by Azure Boards and how they can help you quickly plan, manage, and track work across your entire team. 
* You will explore the product backlog, sprint backlog, and task boards which can be used to track the flow of work during the course of an iteration. 
* We will also take a look at how the tools have been enhanced in this release to scale for larger teams and organizations.

Lab requirements
----------------

- This lab requires you to create the project from 
https://azuredevopsdemogenerator.azurewebsites.net/ 

* **Completion of previous labs**

---

### Task: Working with work items

* Work items play a prominent role in Azure DevOps. 
* Whether describing work to be done, impediments to release, test definitions, or other key items, work items are the workhorse of modern projects. 
* In this task you'll focus on using various work items to set up the plan to extend the Parts Unlimited site with a product training section. 
* While it can be daunting to build out such a substantial part of a company's offering, Azure DevOps and the Scrum process make it very manageable.

![](images/010.png)

This task is designed to illustrate a variety of ways you can create different kinds of work items, as well as to demonstrate the breadth of features available on the platform. As a result, these steps should not be viewed as prescriptive guidance for project management. The features are intended to be flexible enough to fit your process needs, so explore and experiment as you go.

1. Navigate to **Overview \| Dashboards**.

    ![](images/011.png)

1. Select the **Overview** dashboard for **Parts Unlimited Team**.

    ![](images/012.png)

1. There are many ways to create work items in Azure DevOps, and we'll explore a few of them. Sometimes it's as simple as firing one off from a dashboard. In the **New Work Item** form, type **"Product training"** and select the **Epic** type. Click **Create**.

    ![](images/new-wit.png)
    ![](images/013.png)

1. Assign the new work item to yourself and set the **Area** to **Parts Unlimited\PUL-Web**. Set the **Iteration** to **Parts Unlimited\Sprint 2** and click **Save & Close**. Ordinarily you would want to fill out as much information as possible, but you can run lean here for the purposes of this lab.

    ![](images/014.png)

1. Navigate to **Boards \| Work Items**.

    ![](images/015.png)

1. Locate the newly created epic for **Product training** and open it.

    ![](images/016.png)

1. The work item form includes everything you could ever want to know about a work item. This includes details about who it's assigned to, its status across many parameters, and all the associated information and history for how it has been handled since creation. One of the key areas to focus on is the **Related Work**. One of the ways to add a feature to this epic is to select **Add link \| New item**.

    ![](images/017.png)

1. Set the **Link Type** to **Child**, **Work item type** to **Feature** and set the **Title** to **"Training dashboard"**. Click **OK**.

    ![](images/018.png)

1. That **Assignment**, **Area**, and **Iteration** should already set to the same as the epic, and it's even linked to the parent item it was created from. Click **Save & Close**.

    ![](images/019.png)

1. Navigate to the **Boards** view.

    ![](images/020.png)

1. Select **PUL-Web Boards**. This will open the board for that particular team.

    ![](images/021.png)

1. Switch the board from showing **Backlog items** to showing **Features**. This will make it easy to add tasks and other work items to the features.

    ![](images/022.png)

1. From the **Training dashboard** dropdown, select **Add Product Backlog Item**.

    ![](images/023.png)

1. Name the first backlog item **"As a customer, I want to view new tutorials"** and press **Enter** to save. This creates a new **Product Backlog Item** (PBI) work item that is a child of the feature and shares its area and iteration.

    ![](images/024.png)

1. Add two more PBIs designed to enable the customer to see their recently viewed tutorials and to request new tutorials.

    ![](images/025.png)

1. Switch the task board view back to **Backlog items**.

    ![](images/026.png)

1. Backlog items have a state that defines where they are relative to being completed. While you could open and edit the work item using the form, it's easier to just drag cards on the board. Drag the first work item to **Approved**.

    ![](images/027.png)

1. You can also expand work item cards to get to conveniently editable details.

    ![](images/028.png)

1. Assign the moved PBI to yourself.

    ![](images/029.png)

1. Drag the second work item to the **Committed** stage.

    ![](images/030.png)

1. Drag the final PBI to the **Done** stage.

    ![](images/031.png)

1. The task board is one view into the backlog. View the tabular form by clicking **View as Backlog**.

    ![](images/032.png)

1. Click the **Expand** button, which allows you to view nested tasks under these work items. Another easy way to create work items is using the **Add** button on the backlog. Click it to add a new task to the first backlog item.

    ![](images/033.png)

1. Set the **Title** to **"Add page for most recent tutorials"**. Set the **Remaining Work** to **"5"** and the **Activity** to **"Development"**. Click **Save & Close**.

    ![](images/034.png)

1. Add another task to **"Optimize data query for most recent tutorials"**. Set its **Remaining Work** to **"3"** and its **Activity** to **"Design"**. Click **Save & Close**.

    ![](images/035.png)

