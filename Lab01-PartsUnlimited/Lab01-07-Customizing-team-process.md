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


### Task: Customizing team process

* In Azure DevOps, you customize your work tracking experience through a process. 
* A process defines the building blocks of the work item tracking system as well as other sub-systems you access through Azure DevOps. 
* Whenever you create a team project, you select the process which contains the building blocks you want for your project.

* *zure DevOps supports two process types. 
* The first, the core system processes-Scrum, Agile, and CMMI system processes-are locked. 
* You cannot customize these processes.
*  The second type, inherited processes, you create from a core system process. 
*  These processes you can customize.

* In addition, all processes are shared. 
* That is, one or more team projects can reference a single process. 
* Instead of customizing a single team project, you customize a process. Changes made to the process automatically update all team projects that reference that process.

* Once you've created an inherited process, you can customize it, create team projects based on it, and migrate existing team projects to reference it. 
* The Git team project can't be customized until it's migrated to an inherited process.

* In this task we'll create a new process that inherits from Scrum. 
* The one change we'll make is to add a backlog item field designed to track to a proprietary PartsUnlimited ticket ID.

1. Click the **Azure DevOps** logo in the top left corner to navigate to the account root.
   
    ![](images/106.png)

2. From the left bottom corner, click **Organization settings**.

    ![](images/107.png)

3. Select the **Process** tab under **Boards**.

    ![](images/process.png)

4. From the **Scrum** dropdown, select **Create inherited process**.

    ![](images/109.png)

5. Set the name of the inherited process to **Customized Scrum** and click **Create process**.

    ![](images/110.png)

6. Open **Customized Scrum**. 
   - You may need to refresh the browser for this to become visible.

    ![](images/111.png)

7. Select **Product Backlog Item**.

    ![](images/112.png)

8. Click **New field**.

    ![](images/113.png)

9.  Set the **Name** of the new field to **"PUL Ticket ID"**.

    ![](images/114.png)

10. On the **Layout** tab, set the **Label** to **"Ticket ID"**. Also **Create a new group** for **"PartsUnlimited"**. Click **Add field**.

    ![](images/115.png)

11. Now that the customized process has been configured, let's switch the Parts Unlimited project to use it. 
    - Return to the **All processes** root using the breadcrumb.

    ![](images/116.png)

12. Our project currently uses **Scrum**, so select that process.

    ![](images/117.png)

13. Switch to the **Projects** tab.

    ![](images/118.png)

14. From the context menu for **Parts Unlimited**. 
    - Select **Change process**.

    ![](images/119.png)

15. Select the **Customized Scrum** process and click **Save**.

    ![](images/120.png)

16. Return to the account dashboard using the logo link.

    ![](images/121.png)

17. Open the **Parts Unlimited** portal.

    ![](images/122.png)

18. Select **Boards \| Work Items**.

    ![](images/123.png)

19. Open the first backlog item.

    ![](images/124.png)

20. You will now see the **Ticket ID** field under the **PartsUnlimited** group defined during the process customization. You can treat this like any other text field.

    ![](images/125.png)

21. Once the work item is saved, Azure DevOps will also save the new custom information so that it will be available for queries and through the rest of Azure DevOps.

