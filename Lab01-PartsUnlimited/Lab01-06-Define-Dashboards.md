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

### Task: Defining dashboards

1. Select **Overview \| Dashboards**.

    ![](images/086.png)

1. From the dashboard dropdown, select **Parts Unlimited Team Overview**. Dashboards allow teams to visualize status and monitor progress across the project. 
   - At a glance, you can make informed decisions without having to drill down into other parts of your team project site. 
   - The Overview page provides access to a default team dashboard which you can customize by adding, removing, or rearranging the tiles. 
   - Each tile corresponds to a widget that provides access to one or more features or functions.

    ![](images/087.png)

2. From the dashboard dropdown, select **New dashboard**.

    ![](images/088.png)

3. Set the **Name** to **"Product training"** and select the **PUL-Web** team. 
   - Click **Create**.

    ![](images/089.png)

4. Click **Add a widget**.

    ![](images/090.png)

5. In the **Add Widget** panel, search for **"sprint"** to find existing widgets that focus on sprints. 
   - Select **Sprint Overview** and click **Add**.

    ![](images/091.png)

6. Many widgets have options you can configure. 
   - Click the **Settings** button.

    ![](images/092.png)

7. The quantity and depth of settings will vary by widget. 
   - Click **Close** to dismiss.

    ![](images/093.png)

8. Search the widgets again for **"sprint"** and add the **Sprint Capacity** widget.

    ![](images/094.png)

9.  Click **Done Editing**.

    ![](images/095.png)

10. You can now review two important aspects of your current sprint on your custom dashboard.

    ![](images/096.png)

11. Another way of customizing dashboards is to generate charts based on work item queries, which you can share to a dashboard. 
    - Select **Boards \| Queries**.

    ![](images/097.png)

12. Click **New query**.

    ![](images/098.png)

13. Set the first term to **Work Item Type = Task** and the second term to **Area Path = Parts Unlimited\PUL-Web**.

    ![](images/099.png)

14. Click **Save query**.

    ![](images/100.png)

15. Set the **Name** to **"Web tasks"** and the **Folder** to **Shared Queries**. 
    - Click **OK**.

    ![](images/101.png)

16. Select the **Charts** tab and click **New chart**.

    ![](images/102.png)

17. Click **New chart**.

    ![](images/103.png)

18. Set the **Name** of the chart to **"Web tasks - By assignment"** and **Group by** to **Assigned To**. 
    - Click **OK** to save.

    ![](images/104.png)

19. You can now add this chart to a dashboard.

    ![](images/105.png)

