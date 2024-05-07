
Agile planning and portfolio management with Azure Boards
=========================================================

Lab requirements
----------------

* **Completion of previous labs**

Objectives
----------

After you complete this lab, you will be able to:

*   Customize Kanban boards.

Instructions
------------

#### Task: Customize Kanban boards

* In this task, you will step through the process of customizing Kanban boards.
* To maximize a team’s ability to consistently deliver high quality software, Kanban emphasizes two main practices. 
* The first, visualizing the flow of work, requires that you map your team’s workflow stages and configure a Kanban board to match. 
* The second, constraining the amount of work in progress, requires that you set work-in-progress (WIP) limits. 

* You’re then ready to track progress on your Kanban board and monitor key metrics to reduce lead or cycle time. 
* Your Kanban board turns your backlog into an interactive signboard, providing a visual flow of work. 
* As work progresses from idea to completion, you update the items on the board. 
* Each column represents a work stage, and each card represents a user story (blue cards) or a bug (red cards) at that stage of work. 
* However, every team develops its own process over time, so the ability to customize the Kanban board to match the way your team works is critical for the successful delivery.

---

1.  In the vertical navigational pane of the Azure DevOps portal, in the list of the **Boards** items, select **Boards**.
2.  On the **Boards** panel, click the **Configure board settings** cogwheel icon (directly to the right of the funnel icon).
    
     > **Note**: The team is emphasizing work done with data, so there is special attention paid to any task associated with accessing or storing data.
    
3.  On the **Settings** panel, select the **Tag colors** tab, click **\+ Tag color**, in the **Tag** textbox, type **data** and leave the default color in place.
    
     !["Settings" window, "Tag colors", include "data" tag](./images/EShop-WEB-tag_color_v1.png)
    
     > **Note**: Whenever a backlog item or bug is tagged with **data**, that tag will be highlighted.
    
4.  From the **Configure board settings** (cogwheel) On the **Settings** panel, select the **Annotations** tab.
    
     > **Note**: You can specify which **Annotations** you would like included on cards to make them easier to read and navigate. When an annotation is enabled, the child work items of that type are easily accessible by clicking the visualization on each card.
    
5.  On the **Settings** panel, select the **Tests** tab.
    
     > **Note**: The **Tests** tab enables you to configure how tests appear and behave on the cards.
    
6.  On the **Settings** panel, click **Save and close** to save the styling rule.
7.  From the **Board** tab of the **EShop-WEB** panel, open the Work Item representing the **As a customer, I want to view new tutorials** backlog item.
8.  From the detailed item view, at the top of the panel, to the right of the **0 comments** entry, click **Add tag**.
9.  In the resulting textbox, type **data** and press the **Enter** key.
10.  Repeat the previous step to add the **ux** tag.
11.  Save these edits by clicking **Save & Close**.
    
     ![On the ""As a customer, I want to view new tutorials" panel, click "Save & Close"](./images/EShop-WEB-tags_v1.png)
    
     > **Note**: The two tags are now visible on the card, with the **data** tag highlighted in yellow as configured.
    
12.  On the **Boards** panel, click the **Configure board settings** cogwheel icon (directly to the right of the funnel icon).
13.  On the **Settings** panel, select the **Columns** tab.
    
     > **Note**: This section allows you to add new stages to the workflow.
    
14.  Click **\+ Column**, under the **Column name** label, in the **Name** textbox, type **QA Approved** and, in the **WIP limit** textbox, type **1**
    
     > **Note**: The Work in progress limit of 1 indicates that only one work item should be in this stage at a time. You would ordinarily set this higher, but there are only two work items to demonstrate the feature.
    
     ![On the "Settings" panel, clikc "Save & Close"](./images/EShop-WEB-qa_column_v1.png)
    
15.  On the **Settings** panel, select the **Columns** tab again. Notice the ellipsis next to the **QA Approved** column you created. Select **Move right** twice, so that the QA Approved column gets positioned in-between **Committed** and **Done**.
16.  On the **Settings** panel, click **Save**.
    
17.  **Refresh** the **Boards portal**, so the **QA Approved** column is visible in the Kanban board view now.
18.  Drag the **As a customer, I want to see tutorials I recently viewed** work item from the **Committed** stage into the **QA Approved** stage.
19.  Drag the **As a customer, I want to view new tutorials** work item from the **Approved** stage into the **QA Approved** stage.
    
     ![The stage now exceeds its **WIP** limit and is colored red as a warning next to "QA Approved" column](./images/EShop-WEB-wip_limit_v1.png)
    
     > **Note**: The stage now exceeds its **WIP** limit and is colored red as a warning.
    
20.  Move the **As a customer, I want to see tutorials I recently viewed** backlog item back to **Committed**.
21.  On the **Boards** panel, click the **Configure board settings** cogwheel icon (directly to the right of the funnel icon).
22.  On the **Settings** panel, return to the **Columns** tab and select the **QA Approved** tab.
    
     > **Note**: A lag often exists between when work gets moved into a column and when work starts. To counter that lag and reveal the actual state of work in progress, you can turn on split columns. When split, each column contains two sub-columns: **Doing** and **Done**. Split columns let your team implement a pull model. Without split columns, teams push work forward, to signal that they’ve completed their stage of work. However, pushing it to the next stage doesn’t necessarily mean that a team member immediately starts work on that item.
    
23.  On the **QA Approved** tab, enable the **Split column into doing and done** checkbox to create two separate columns.
    
     > **Note**: As your team updates the status of work as it progresses from one stage to the next, it helps that they agree on what **done** means. By specifying the **Definition of done** criteria for each Kanban column, you help share the essential tasks to complete before moving an item into a downstream stage.
    
24.  On the **QA Approved** tab, at the bottom of the panel, in the **Definition of done** textbox, type **Passes \*\*all\*\* tests**.
25.  On the **Settings** panel, click **Save and close**.
    
     ![On the "Settings" panel, review information and click "Save and close"](./images/dd_v1.png)
    
     > **Note**: The **QA Approved** stage now has **Doing** and **Done** columns. You can also click the informational symbol (with letter **i** in a circle) next to the column header to read the **Definition of done**.
    
     ![Split Columns for QA Approved](./images/EShop-WEB-qa_2columns_v1.png)
    
26.  On the **Boards** panel, click the **Configure boards settings** cogwheel icon (directly to the right of the funnel icon).
    
     > **Note**: Your Kanban board supports your ability to visualize the flow of work as it moves from new to done. When you add **swimlanes**, you can also visualize the status of work that supports different service-level classes. You can create a swimlane to represent any other dimension that supports your tracking needs.
    
27.  On the **Settings** panel, select the **Swimlanes** tab.
28.  On the **Swimlanes** tab, click **\+ Swimlane**, directly under the **Swimlane name** label, in the **Name** textbox, type **Expedite**.
29.  On the **Settings** panel, click **Save**.
    
     ![On the "Settings" panel, review information and click "Save"](./images/EShop-WEB-swimlane_v1.png)
    
30.  Back on the **Board** tab of the **Boards** panel, drag and drop the **Committed** work item onto the **QA Approved | Doing** stage of the **Expedite** swimlane so that it gets recognized as having priority when QA bandwidth becomes available.

