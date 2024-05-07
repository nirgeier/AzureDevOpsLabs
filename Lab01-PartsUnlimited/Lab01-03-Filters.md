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
 
### Task: Working with filters in backlogs and boards 

* Azure Boards comes with filtering capabilities. 
* With filter functions, you can interactively apply one or more filters to an Azure Boards tool.  
* Filter functions available in Work items, Boards, Backlogs, Sprint Backlogs and Taskboards, Queries, and Delivery Plans. 
* In this exercise, you will see the filters in the boards and backlogs.

---

1. Navigate to the **Backlog Items** view. 
   **You should how to by now**
   - Boards > Backlog > `Backlog name`

2. Choose Filter ![](images/filter-icon.png) Or, enter the **Ctrl+Shift+f** keyboard shortcut.
  
   ![](images/backlog_filter.png)

3. Choose the filters of interest. The filter icon changes to a solid icon, Filter ![](images/filtered.png) , to indicate filtering is applied.

   Only those work items that satisfy all of the chosen filter criteria are showed on the page.


   ![](images/backlog_filter2.png)

    > **Note** When filtering is applied for backlogs, the add-a-backlog-item panel, reordering (stack ranking), and forecasting tools are disabled.

4. To clear the filtering, choose **Clear and dismiss filters**.
   ![](images/clearfilters.png)

   Filters remain in place until you explicitly clear them. When you refresh your backlog, board, or other tool, or sign in from another browser, filters remain set to your previous values.

5. Filtering functions similarly in Boards and Backlog view. 
To choose the filter criteria, switch to the Boards view and select filter.
    
    ![](images/boards_filter.png)

6. You can filter the work items in boards or backlog view uisng a key word or Assigned To, Work Item Type, States, Area Path and Iteration Path fields.

    > **Note**: For more detailed information about the filter functions and how you can apply one or more filters to an Azure Boards tool visit this  page
    [Interactively filter backlogs, boards, queries, and plans in Azure Boards](https://learn.microsoft.com/en-us/azure/devops/boards/backlogs/filter-backlogs-boards-plans?view=azure-devops)


