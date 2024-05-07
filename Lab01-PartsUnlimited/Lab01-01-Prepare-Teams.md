## Overview 

* In this lab, you will learn about the agile planning and portfolio management tools and processes provided by Azure Boards and how they can help you quickly plan, manage, and track work across your entire team. 
* You will explore the product backlog, sprint backlog, and task boards which can be used to track the flow of work during the course of an iteration. 
* We will also take a look at how the tools have been enhanced in this release to scale for larger teams and organizations.


### Prerequisites

- This lab requires you to create the project from 
https://azuredevopsdemogenerator.azurewebsites.net/ 

## Exercise: Agile Project Management

### Task: Working with teams, areas, and iterations 

1. Navigate to your Parts Unlimited project on Azure DevOps.   
   
2. It will be something like [https://dev.azure.com/YOURACCOUNT/Parts%20Unlimited](https://dev.azure.com/YOURACCOUNT/Parts Unlimited).

3. Open the settings page using the **Project settings** navigation located at the bottom left of the page.

    ![](images/settings.png)

4. Select the **Teams** tab. There are already a few teams in this project, but you'll make a new one for this lab. Click **New team**.

    ![](images/001.png)

5. Use **"PUL-Web"** as the **Team name** and click **Create team** (Leave defaults).

    ![](images/002.png)

6. Select the newly created team to view its details.

    ![](images/003.png)

7. By default, the new team has only you as its member. You can use this view to manage membership, notifications, dashboards, and more. But first you will want to define the schedule and scope of the team. Click **Iterations and Area Paths**.

    ![](images/004.png)

8. Select the **Iterations** tab and click **Select iterations**. This team will use the same iteration schedule that's already in place for the other teams, although you can take a different route if that's better for your organization.

    ![](images/iteration.png)

9.  Select **Parts Unlimited\Sprint 1** and click **Save and close**. Note that this first sprint has already passed. This is because the demo data generator is designed to build out project history so that this sprint occurs in the past.

    ![](images/006.png)

10. Repeat the process to add **Sprint 2** and **Sprint 3** (add them as in previous step). The second sprint is our current iteration, and the third is in the near future.

    ![](images/007.png)

11. Select the **Areas** tab. By default, there is an area matching the name of the team.

    ![](images/008.png)

12. From the area dropdown, select **Include sub areas**. The default setting for all teams is to exclude sub-area paths. We will change it to include sub-areas so that the team gets visibility into all of the work items from all teams. Optionally, the management team could also choose to not include sub-areas, thereby removing work items from their view as soon as they are assigned to one of the teams.

    ![](images/009.png)

