
Agile planning and portfolio management with Azure Boards
=========================================================

Lab requirements
----------------

* **Completion of previous labs**

Objectives
----------

After you complete this lab, you will be able to:

*   Manage sprints and capacity.

Instructions
------------

#### Task: Manage sprints and capacity

* In this task, you will step through common sprint and capacity management tasks.

* Teams build the sprint backlog during the sprint planning meeting, typically held on the first day of the sprint. 
* Each sprint corresponds to a time-boxed interval which supports the team’s ability to work using Agile processes and tools. 
* During the planning meeting, the product owner works with the team to identify those stories or backlog items to complete in the sprint.

* Planning meetings typically consist of two parts. 
* In the first part, the team and product owner identify the backlog items that the team feels it can commit to completing in the sprint, based on experience with previous sprints. 
* These items get added to the sprint backlog. In the second part, the team determines how it will develop and test each item. 
* They then define and estimate the tasks required to complete each item.
* Finally, the team commits to implementing some or all the items based on these estimates.

* The sprint backlog should contain all the information the team needs to successfully plan and complete work within the time allotted without having to rush at the end. 
* Before planning the sprint, you’d want to have created, prioritized, and estimated the backlog and defined the sprints.

---

1.  In the vertical navigational pane of the Azure DevOps portal, select the **Boards** icon and, in the list of the **Boards** items, select **Sprints**.
2.  On the **Taskboard** tab of the **Sprints** view, in the toolbar, on the right hand side, select the **View options** symbol (directly to the left of the funnel icon) and, in the **View options** dropdown list, select the **Work details** entry. Select **Sprint 2** as filter.
    
     ![In the "Boards">"Sprints" window, "EShop-WEB" team, select "View options" icon and click on "Work details"](./images/EShop-WEB-work_details_v1.png)
    
     > **Note**: The current sprint has a pretty limited scope. There are two tasks in the **To do** stage. At this point, neither task has been assigned. Both show a numeric value to the right of **Unassigned** entry representing the remaining work estimate.
    
3.  Within the **ToDo** Column, notice the Task Item **Add page for most recent tutorials**, click the **Unassigned** entry and, in the list of user accounts, select your account to assign the task to yourself.
    
4.  Select the **Capacity** tab of the **Sprints** view.
    
     ![Sprint Capacity View](./images/EShop-WEB-capacity_v1.png)
    
     > **Note**: This view enables you to define what activities a user can take on and at what level of capacity.
    
5.  On the **Capacity** tab of the **Sprints** view, click **+Add User** and select your user account. For this user, set the **Activity** field to **Development** and, in the **Capacity per day** textbox, type **1**.
    
     > **Note**: This represents 1 hour of development work per day. Note that you can add additional activities per user in the case they do more than just development.
    
     ![Set Development Capacity for a user](./images/EShop-WEB-capacity-setdevelopment_v1.png)
    
     > **Note**: Let’s assume you’re also going to take some vacation. Which should be added to the capacity view too.
    
6.  On the **Capacity** tab of the **Sprints** view, directly next to the entry representing your user account, in the **Days off** column, click the **0 days** entry. This will display a panel where you can set your days off.
7.  In the displayed panel, use the calendar view to set your vacation to span five work days during the current sprint (within the next three weeks) and, once completed, click **OK**.
    
     ![Enter "Start", "End" and "Days Off" as mentioned](./images/EShop-WEB-days_off_v1.png)
    
8.  Back on the **Capacity** tab of the **Sprints** view, click **Save**.
9.  Select the **Taskboard** tab of the **Sprints** view.
    
     ![Review the "Work details" section information, all timing bars should be green. ](./images/EShop-WEB-work_details_window_v1.png)
    
     > **Note**: Note that the **Work details** panel has been updated to reflect your available bandwidth. The actual number displayed in the **Work details** panel might vary, but your total sprint capacity will be equal to the number of working days remaining till the end of the sprint, since you allocated 1 hour per day. Take a note of this value since you will use it in the upcoming steps.
    
     > **Note**: One convenient feature of the boards is that you can easily update key data in-line. It’s a good practice to regularly update the **Remaining Work** estimate to reflect the amount of time expected for each task. Let’s say you’ve reviewed the work for the **Add page for most recent tutorials** task and found that it will actually take longer than originally expected.
    
10.  On the **Taskboard** tab of the **Sprints** view, in the square box representing the **Add page for most recent tutorials**, set the estimated number of hours to **14**, to match your total capacity for this sprint, which you identified in the previous step.
    
     ![Review the "Work details" section information, team´s assigned time is bigger than capacity.](./images/EShop-WEB-over_capacity_v1.png)
    
     > **Note**: This automatically expands the **Development** and your personal capacities to their maximum. Since they’re large enough to cover the assigned tasks, they stay green. However, the overall **Team** capacity is exceeded due to the additional 3 hours required by the **Optimize data query for most recent tutorials** task.
    
     > **Note**: One way to resolve this capacity issue would be to move the task to a future iteration. There are a few ways this could be done. You could, for example, open the task here and edit it within the panel providing access to the task details. Another approach would be to use the **Backlog** view, which provides an in-line menu option to move it. At this point though, don’t move the task yet.
    
11.  On the **Taskboard** tab of the **Sprints** view, in the toolbar, on the right hand side, select the **View options** symbol (directly to the left of the funnel icon) and, in the **View options** dropdown list, select the **Assigned To=** entry.
    
     > **Note**: This adjusts your view such that you can review the progress of tasks by person instead of by backlog item.
    
     > **Note**: There is also a lot of customization available.
    
12.  Click the **Configure team settings** cogwheel icon (directly to the right of the funnel icon).
13.  On the **Settings** panel, select the **Styles** tab, click **\+ Styling rule**, under the **Rule name** label, in the **Name** textbox, type **Development**, and, in the **Card color** dropdown list, select the green rectangle.
    
     > **Note**: This will color all cards green if they meet the rule criteria set directly below, in the **Rule criteria** section.
    
14.  In the **Rule criteria** section, in the **Field** dropdown list, select **Activity**, in the **Operator** dropdown list, select **\=**, and, in the **Value** dropdown list, select **Development**.
    
     !["Settings" window, make sure all fields have mentioned information](./images/EShop-WEB-styles_v1.png)
    
     > **Note**: This will set all cards assigned to **Development** activities green.
    
     ![Sprint Tasks styles](./images/EShop-WEB-sprint-green_v1.png)
    
15.  On the **Settings** panel, select the **Backlogs** tab.
    
     > **Note**: Entries on this tab allow you to set the levels available for navigation. Epics are not included by default, but you could change that.
    
16.  On the **Settings** panel, select the **Working days** tab.
    
     > **Note**: Entries on this tab allow you to specify the **Working days** the team follows. This applies to capacity and burndown calculations.
    
17.  On the **Settings** panel, select the **Working with bugs** tab.
    
     > **Note**: Entries on this tab allow you to specify how bugs are presented on the board.
    
18.  On the **Settings** panel, click **Save and close** to save the styling rule.
    
     > **Note**: The task associated with **Development** is now green and very easy to identify.