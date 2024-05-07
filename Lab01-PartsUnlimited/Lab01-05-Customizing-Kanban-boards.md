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

### Task: Customizing Kanban boards 

* To maximize a team's ability to consistently deliver high quality software, Kanban emphasize two main practices. 
* The first, visualize the flow of work, requires you to map your team's workflow stages and configure your Kanban board to match. 
* The second, constrain the amount of work in progress, requires you to set work-in-progress (WIP) limits. 
* You're then ready to track progress on your Kanban board and monitor key metrics to reduce lead or cycle time. 
* Your Kanban board turns your backlog into an interactive signboard, providing a visual flow of work. 
* As work progresses from idea to completion, you update the items on the board. 
* Each column represents a work stage, and each card represents a user story (blue cards) or a bug (red cards) at that stage of work. 
* However, every team develops its own process over time, so the ability to customize the Kanban board to match the way your team works is crucial.

---

1. Navigate to **Boards**.

    ![](images/060.png)

2. Click the **Configure team settings** button.

    ![](images/061.png)

3. You can apply style rules to change the color of cards on kanban boards and task boards. 
   - Styling rules make the cards with important information stand out. Select **Styles** tab. 
   - On the Styles tab, click Add Styling rule and set the Name to `High Priority`. 
   - Choose a Red Card color. This will color all cards red if they meet the rule criteria set below.
    
    ![](images/styles_kanban.png)

4. Add a rule for **Priority = 1**. 
  - This will set all cards with priority **1** to  red. You can add more clauses in the query if required. 
  - Open the work item **As a customer, I want to view new tutorials** and change priority to **1**

    ![](images/styles_kanban2.png)

5. Click **Save and close** to save the styling rule.

6. The backlogs with priority **1** is now red and very easy to identify.
   
    ![](images/styles_kanban3.png)

7. Click the **Configure team settings** button.

    ![](images/061.png)

8. The team is emphasizing work done with data, so there is special attention paid to any task associated with accessing or storing data. 
   - Select the **Tag colors** tab. Click **Add tag color** enter a tag of **"data"**. 
   - Whenever a backlog item or bug is tagged with **data**, that tag will be highlighted.

    ![](images/062.png)

9. You can also specify which **Annotations** you would like included on cards to make them easier to read and navigate. 
   - When an annotation is enabled, the child work items of that type are easily accessible by clicking the visualization on each card.

    ![](images/063.png)

10. The **Tests** tab enables you to configure how tests appear and behave on the cards.

    ![](images/064.png)

11. Click **Save and close**.

    ![](images/065.png)

12. Open the **view new tutorials** backlog item.

    ![](images/066.png)

13. Add tags for **"data"** and **"ux"**. Click **Save & Close**.

    ![](images/067.png)

14. Note that the two tags are now visible on the card, although the **data** tag is highlighted yellow as configured.

    ![](images/068.png)

15. Click the **Configure team settings** button.

    ![](images/069.png)

16. Select the **Columns** tab. 
    - This section allows you to add new stages to the workflow. 
    - Click **Add Column** and set the **Name** to **"QA Approved"**. 
    - Move the column right (under the ... menu)

17. Set the **WIP limit** to **"1"**, which indicates that only one work item should be in this stage at a time. 

18. You would ordinarily set this higher, but there are only two work items to demonstrate the feature with here. Move the stage to occur between **Committed** and **Done**.

    ![](images/070.png)

19. Click **Save and close**.

    ![](images/071.png)

20. You will now see the new stage in the workflow.

    ![](images/072.png)

21. Move the work items from **Committed** and **Done** into **QA Approved**.

    ![](images/073.png)

22. The stage now exceeds its **WIP** limit and is colored red as a warning.

    ![](images/074.png)

23. Move the **recently viewed** backlog item back to **Committed**.

    ![](images/075.png)

24. Click the **Configure team settings** button.

    ![](images/076.png)

25. Return to the **Columns** tab and select **QA Approved**. 
    - A lag often exists between when work gets moved into a column and when work starts. 
    - To counter that lag and reveal the actual state of work in progress, you can turn on split columns. 
    - When split, each column contains two sub-columns: **Doing** and **Done**. Split columns let your team implement a pull model. 
    - Without split columns, teams push work forward, to signal that they've completed their stage of work. 
    - However, pushing it to the next stage doesn't necessarily mean that a team member immediately starts work on that item. 
    - Check **Split column into doing and done** to create two separate columns for this.

    ![](images/077.png)

26. As your team updates the status of work as it progresses from one stage to the next, it helps that they agree on what **done** means. 
    - By specifying the **Definition of done** criteria for each Kanban column, you help share the essential tasks to complete before moving an item into a downstream stage. 
    - Add a **Definition of done** using markdown, such as **"Passes \*\*all\*\* tests."**. 
    - Click **Save and close**.

    ![](images/078.png)

27. Note that the **QA Approved** stage now has **Doing** and **Done** columns.

    ![](images/079.png)

28. You can also click the icon next to the column header to read the **Definition of done**.

    ![](images/080.png)

29. Click the **Configure team settings** button.

    ![](images/081.png)

30. Your Kanban board supports your ability to visualize the flow of work as it moves from new to done. 
    - When you add **swimlanes**, you can also visualize the status of work that supports different service-level classes. 
    - You can create a swimlane to represent any other dimension that supports your tracking needs. 
    - From the **Swimlanes** tab, click **Add Swimlane** and set the **Name** to **"Expedite"**. Click **Save and close**.

    ![](images/082.png)

31. Drag and drop the **Committed** work item onto **QA Approved \| Doing** so that it gets recognized as having priority when QA bandwidth becomes available.

    ![](images/083.png)

32. If you would like to review a more sophisticated board with many more work items, select the **Parts Unlimited Team** from the team dropdown.

    ![](images/084.png)

33. This board provides a playground for you to experiment with and review the results.

    ![](images/085.png)

