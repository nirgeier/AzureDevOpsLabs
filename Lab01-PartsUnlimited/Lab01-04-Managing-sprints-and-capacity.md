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
### Task: Managing sprints and capacity 

* Your team builds the sprint backlog during the sprint planning meeting, typically held on the first day of the sprint. 
* Each sprint corresponds to a time-boxed interval which supports your team's ability to work using Agile processes and tools. 
* During the planning meeting, your product owner works with your team to identify those stories or backlog items to complete in the sprint.

* Planning meetings typically consist of **two parts**. 
* In the first part, the team and product owner identify the backlog items that the team feels it can commit to completing in the sprint, based on experience with previous sprints. 
* These items get added to the sprint backlog. 
* In the second part, your team determines how it will develop and test each item. 
* They then define and estimate the tasks required to complete each item. Finally, your team commits to implementing some or all the items based on these estimates.

---

 * Your sprint backlog should contain all the information your team needs to successfully plan and complete work within the time allotted without having to rush at the end. 
  
    > **Note**: Before you start planning your sprint, you'll want to have created, prioritized, and estimated your backlog and defined your sprints. 
    
1. Navigate to the **Sprints** view using the navigation.

    ![](images/036.png)

2. From the **View options** dropdown, select the **Work details** panel option.
   
    ![](images/037.png)

3. The current sprint has a pretty limited scope. 
    - There are two tasks in the **To do** stage that combine for 8 hours of estimated work. 
    - At this point, neither task has been assigned.

    ![](images/038.png)

4. Assign the **Add page** task to yourself. Note that this updates the capacity view.

    ![](images/039.png)

5. Select the **Capacity** tab. 
   - This view enables you to define what activities a user can take on and at what level of capacity. 
   - In this case, set your capacity to allow **"1"** hour of **Development** per day. 
   - Note that you can add additional activities per user in the case they do more than just development.

    ![](images/040.png)

6. However, let's assume you're going to take some vacation. Click **0 days** under **Days off**.

    ![](images/041.png)

7. Set your vacation to span five work days during the current sprint (within the next few weeks). Click **OK**.

    ![](images/042.png)

8. Click **Save**.

    ![](images/043.png)

9.  Return to the **Taskboard**.

    ![](images/044.png)

10. Note that the capacity view has been updated to reflect your available bandwidth. This exact number may vary, but for the screenshots here, that sprint capacity is 11 hours (1 hour per day over 11 working days).

    ![](images/045.png)

11. One convenient feature of the boards is that you can easily update key data in-line. It's a good practice to regularly update the **Remaining Work** estimate to reflect the amount of time expected for each task. 
    
      - Let's say you've reviewed the work for the **Add page** task and found that it will actually take longer than originally expected. 
      - Set it to whatever your total capacity is for this sprint.

    ![](images/046.png)

12. Note how this expands the **Development** and your personal capacities to their maximum. 
    - Since they're large enough to cover the assigned tasks, they stay green. 
    - However, the overall **Team** capacity is exceeded due to the additional 3 hours required by the other task.

    ![](images/047.png)

13. One way to resolve this capacity issue would be to move the task to a future iteration. There are a few ways this could be done. 
    - First, you could open the task here and edit it in the dialog. 
    - The **Backlog** view, on the other hand, provides an in-line menu option to move it. 
    - Don't move it now.

    ![](images/048.png)

14. Return to the **Taskboard** view.

    ![](images/049.png)

15. Select **People** from the **View options** dropdown.

    ![](images/050.png)

16. This adjusts your view such that you can review the progress of tasks by person instead of by backlog item.

    ![](images/051.png)

17. There is also a lot of customization available. Click the **Configure team settings** button.

    ![](images/052.png)

18. On the **Styles** tab, click **Add Styling rule** and set the **Name** to **"Development"**. Choose a green **Card color**. This will color all cards green if they meet the rule criteria set below.

    ![](images/053.png)

19. Add a rule for **Activity = Development**. This will set all cards assigned to **Development** activities green.

    ![](images/054.png)

20. The **Backlogs** tab allows you to set the levels available for navigation. Epics are not included by default, but you could change that here.

    ![](images/055.png)

21. You can also specify the **Working days** the team follows. This applies to capacity and burndown calculations.

    ![](images/056.png)

22. The **Working with bugs** tab allows you to specify how bugs are presented on the board.

    ![](images/057.png)

23. Click **Save and close** to save the styling rule.

    ![](images/058.png)

24. The task associated with **Development** is now green and very easy to identify.

    ![](images/059.png)

