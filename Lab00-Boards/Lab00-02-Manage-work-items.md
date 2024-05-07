
Agile planning and portfolio management with Azure Boards
=========================================================

Lab requirements
----------------

* **Completion of previous labs**

Objectives
----------

After you complete this lab, you will be able to:

*   Manage work items.
  
Instructions
------------

#### Task: Manage work items

* In this task, you will step through common work item management tasks.

* Work items play a prominent role in Azure DevOps. 
* Whether describing work to be done, impediments to release, test definitions, or other key items, work items are the workhorse of modern projects. 
* In this task you’ll focus on using various work items to set up the plan to extend the eShopOnWeb site with a product training section. 
* While it can be daunting to build out such a substantial part of a company’s offering, Azure DevOps and the Scrum process make it very manageable.

> **Note**: This task is designed to illustrate a variety of ways you can create different kinds of work items, as well as to demonstrate the breadth of features available on the platform. As a result, these steps should not be viewed as prescriptive guidance for project management. The features are intended to be flexible enough to fit your process needs, so explore and experiment as you go.

---

1.  In the vertical navigational pane of the Azure DevOps portal, select the **Boards** icon and, select **Work Items**.
    
     > **Note**: There are many ways to create work items in Azure DevOps, and we’ll explore a few of them. Sometimes it’s as simple as firing one off from a dashboard.
    
2.  On the **Work Items** window, click on **\+ New Work Item > Epic**.
    
     ![In the "Boards">"Work Items" window, click on "New work item" >Epic](./images/EShop-WEB-create_epic_v1.png)
    
3.  In the **Enter title** textbox, type **Product training**.
4.  In the upper left corner, select the **Unassigned** entry and, in the dropdown list, select your user account in order to assign the new work item to yourself. If your name doesn’t appear to start with, begin typing your name and click **Search**.
5.  Next to the **Area** entry, select the **eShopOnWeb** entry and, in the dropdown list, select **EShop-WEB**. This will set the **Area** to **eShopOnWeb\\EShop-WEB**.
6.  Next to the **Iteration** entry, select the **eShopOnWeb** entry and, in the dropdown list, select **Sprint 2**. This will set the **Iteration** to **eShopOnWeb\\Sprint 2**.
7.  Click **Save** to finalize your changes. **Do not close it**.
    
     ![Enter previously shown information and click "Save" in Epic window](./images/EShop-WEB-epic_details_v1.png)
    
     > **Note**: Ordinarily you would want to fill out as much information as possible, but this is sufficient for the purposes of this lab.
    
     > **Note**: The work item form includes all of the relevant work item settings. This includes details about who it’s assigned to, its status across many parameters, and all the associated information and history for how it has been handled since creation. One of the key areas to focus on is the **Related Work**. We will explore one of the ways to add a feature to this epic.
    
8.  In the **Related work** section on the lower right-side, select the **Add link** entry and, in the dropdown list, select **New item**.
9.  On the **Add link** panel, in the **Link Type** dropdown list, select **Child**. Next, in the **Work item type** dropdown list, select **Feature**, in the **Title** textbox, type **Training dashboard**.
    
     ![Include Title "Training Dashboard" and click "OK"](./images/EShop-WEB-create_child_feature.png)
    
     > **Note**: On the **Training dashboard** panel, note that the assignment, **Area**, and **Iteration** are already set to the same values as the epic that the feature is based on. In addition, the feature is automatically linked to the parent item it was created from.
    
10.  Click **Add link** to save the Child item. On the (New Feature) **Training dashboard** panel, click **Save & Close**.
    
     ![Epic with Linked Child Item](./images/EShop-WEB-epic_with_linked_item_v1.png)
    
11.  In the vertical navigation pane of the Azure DevOps portal, in the list of the **Boards** items, select **Boards**.
12.  On the **Boards** panel, select the **EShop-WEB boards** entry. This will open the board for that particular team.
    
     ![ In "Boards>Boards" window, select "EShop-WEB boards"](./images/EShop-WEB-_boards_v1.png)
    
13.  On the **Boards** panel, in the upper right corner, select the **Backlog items** entry and, in the dropdown list, select **Features**.
    
     > **Note**: This will make it easy to add tasks and other work items to the features.
    
14.  Hover with the mouse pointer over the rectangle representing the **Training dashboard** feature. This will reveal the ellipsis symbol (…) in its upper right corner.
15.  Click the ellipsis (…) icon and, in the dropdown list, select **Add Product Backlog Item**.
    
     ![Click on the ellipis for "Training dashboard" feature and click "Add Product Backlog Item"](./images/EShop-WEB-add_pb_v1.png)
    
16.  In the textbox of the new product backlog item, type **As a customer, I want to view new tutorials** and press the **Enter** key to save the entry.
    
     > **Note**: This creates a new product backlog item (PBI) work item that is a child of the feature and shares its area and iteration.
    
17.  Repeat the previous step to add two more PBIs designed to enable the customer to see their recently viewed tutorials and to request new tutorials named, respectively, **As a customer, I want to see tutorials I recently viewed** and **As a customer, I want to request new tutorials**.
    
     ![Repeat by clicking on "Add Product Backlog" ](./images/EShop-WEB-pbis_v1.png)
    
18.  On the **Boards** panel, in the upper right corner, select the **Features** entry and, in the dropdown list, select **Backlog items**.
    
     ![View Backlog Items" ](./images/EShop-WEB-backlog_v1.png)
    
     > **Note**: Backlog items have a state that defines where they are relative to being completed. While you could open and edit the work item using the form, it’s easier to just drag cards on the board.
    
19.  On the **Board** tab of the **EShop-WEB** panel, drag the first work item named **As a customer, I want to view new tutorials** from the **New** to **Approved** stage.
    
     ![Move the WIT from "New" state to "Approved"](./images/EShop-WEB-new2ap_v1.png)
    
     > **Note**: You can also expand work item cards to get to conveniently editable details.
    
20.  Hover with the mouse pointer over the rectangle representing the work item you moved to the **Approved** stage. This will reveal the down facing caret symbol.
21.  Click the down facing caret symbol to expand the work item card, select the **Unassigned** entry, and in the list of user accounts, select your account to assign the moved PBI to yourself.
22.  On the **Board** tab of the **EShop-WEB** panel, drag the second work item named **As a customer, I want to see tutorials I recently viewed** from the **New** to the **Committed** stage.
23.  On the **Board** tab of the **EShop-WEB** panel, drag the third work item named **As a customer, I want to request new tutorials** from the **New** to the **Done** stage.
    
     ![WITs moved to the specified columns from previous steps](./images/EShop-WEB-board_pbis_v1.png)
    
     > **Note**: The task board is one view into the backlog. You can also use the tabular view.
    
24.  On the **Board** tab of the **EShop-WEB** pane, at the top of the pane, click **View as Backlog** to display the tabular form.
    
     ![In the "EShop-WEB" board, click "View as Backlog"](./images/EShop-WEB-view_backlog_v1.png)
    
> **Note**:
> * You can use the plus sign directly under the **Backlog** tab label of the **EShop-WEB** panel to view nested tasks under these work items.
 >   
>* You can use the second plus sign directly left to the first backlog item to add a new task to it.
    
1.   On the **Backlog** tab of the **EShop-WEB** pane, in the upper left corner of the pane, click the second plus sign from the top, the one next to the first work item. This will display the **NEW TASK** panel.
    
     ![Click on "+" to create Task](./images/new_task_v1.png)
    
2.   At the top of the **NEW TASK** panel, in the **Enter title** textbox, type **Add page for most recent tutorials**.
3.   On the **NEW TASK** panel, in the **Remaining Work** textbox, type **5**.
4.   On the **NEW TASK** panel, in the **Activity** dropdown list, select **Development**.
5.   On the **NEW TASK** panel, click **Save & Close**.
    
     ![Fill in "New task" fields and click "Save and Close"](./images/EShop-WEB-save_task_v1.png)
    
6.   Repeat the last five steps to add another task named **Optimize data query for most recent tutorials**. Set its **Remaining Work** to **3** and its **Activity** to **Design**. Click **Save & Close** once completed.

