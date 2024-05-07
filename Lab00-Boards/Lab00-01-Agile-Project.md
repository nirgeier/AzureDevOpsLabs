
Agile planning and portfolio management with Azure Boards
=========================================================

Lab requirements
----------------
    
*   **Set up an Azure DevOps organization:** If you don’t already have an Azure DevOps organization that you can use for this lab, create one by following the instructions available at [Create an organization or project collection](https://docs.microsoft.com/azure/devops/organizations/accounts/create-organization?view=azure-devops).
    

Objectives
----------

After you complete this lab, you will be able to:

*   Manage teams, areas, and iterations.

Instructions
------------

### Exercise: Configure the lab prerequisites

* In this exercise, you will set up the prerequisites for the lab, which consist of a new Azure DevOps project with a repository based on the [eShopOnWeb](https://github.com/MicrosoftLearning/eShopOnWeb).

#### Task: Create and configure the team project

In this task, you will create an **eShopOnWeb** Azure DevOps project to be used by several labs.

1.  On your lab computer, in a browser window open your Azure DevOps organization. Click on **New Project**. Give your project the name **eShopOnWeb**. Define **Private** as Visibility option.
2.  Click **Advanced** and specify **Scrum** as **Work Item Process**. Click on **Create**.
    
     ![Create Project](./images/create-project.png)
    

### Exercise: Manage Agile project

In this exercise, you will use Azure Boards to perform a number of common agile planning and portfolio management tasks, including management of teams, areas, iterations, work items, sprints and capacity, customizing Kanban boards, defining dashboards, and customizing team processes.

#### Task: Manage teams, areas, and iterations

In this task, you will create a new team and configure its area and iterations.

Each new project is configured with a default team, which name matches the project name. You have the option of creating additional teams. Each team can be granted access to a suite of Agile tools and team assets. The ability to create multiple teams gives you the flexibility to choose the proper balance between autonomy and collaboration across the enterprise.

1.  Verify that the web browser displays your Azure DevOps organization with the **eShopOnWeb** project you generated in the previous exercise.
    
     > **Note**: Alternatively, you can access the project page directly by navigating to the \[[https://dev.azure.com/](https://dev.azure.com/)`<your-Azure-DevOps-account-name>`/eShopOnWeb) URL, where the `<your-Azure-DevOps-account-name>` placeholder, represents your account name.
    
2.  Click the cogwheel icon labeled **Project settings** located in the lower left corner of the page to open the **Project settings** page.
    
     ![Azure DevOps project window. Click on "Project settings" option](./images/project_settings_v1.png)
    
3.  In the **General** section, select the **Teams** tab. There is already a default team in this project, **eShopOnWeb Team** but you’ll create a new one for this lab. Click **New Team**.
    
     ![In project settings window, "Teams" tab, click on "New Team"](./images/new_team_v1.png)
    
4.  On the **Create a new team** pane, in the **Team name** textbox, type **EShop-Web**, leave other settings with their default values, and click **Create**.
    
     ![In "create a new team" window, call your new team "EShop-Web" and click "Create"](./images/eshopweb-team_v1.png)
    
5.  In the list of **Teams**, select the newly created team to view its details.
    
     > **Note**: By default, the new team has only you as its member. You can use this view to manage such functionality as team membership, notifications, and dashboards.
    
6.  Click **Iterations and Area Paths** link at the top of the **EShop-Web** page to start defining the schedule and scope of the team.
    
     ![In project settings window, "Teams" tab, "EShop-WEB" team, click on "Iterations and Area Paths"](./images/EShop-WEB-iterationsareas_v1.png)
    
7.  At the top of the **Boards** pane, select the **Iterations** tab and then click **\+ Select iteration(s)**.
    
     ![In the "iterations" tab, click on "Select Iteration"](./images/EShop-WEB-select_iteration_v1.png)
    
8.  Select **eShopOnWeb\\Sprint 1** and click **Save and close**. Note that this first sprint will show up in the list of iterations, but the Dates are not set yet.
9.  Select **Sprint 1** and click the **ellipsis (…)**. From the context menu, select **Edit**.
    
     ![In the "iterations" tab, click on "Edit"](./images/EShop-WEB-edit_iteration_v1.png)
    
     > **Note**: Specify the Start Date as the first work day of last week, and count 3 full work weeks for each sprint. For example, if March 6 is the first work day of the sprint, it goes until March 24th. Sprint 2 starts on March 27, which is 3 weeks out from March 6.
    
10.  Repeat the previous step to add **Sprint 2** and **Sprint 3**. You could say that we are currently in the 2nd week of the first sprint.
    
      ![Do the same for Sprint 2 and 3, make sure they are created for "EShop-Web" team](./images/EShop-WEB-3sprints_v1.png)
    
1.   Still in the **Project Settings / Boards / Team Configuration** pane, at the top of the pane, select the **Areas** tab. You will find there an automatically generated area with the name matching the name of the team.
    
     ![From Areas, select eShopOnWeb\EShop-Web](./images/EShop-WEB-areas_v1.png)
    
2.   Click the ellipsis symbol (…) next to the **default area** entry and, in the dropdown list, select **Include sub areas**.
    
     ![In the "Areas" tab, clik on the ellipsis icon (...) for "EShop-WEB" area and select "Include sub areas"](./images/EShop-WEB-sub_areas_v1.png)
    
     > **Note**: The default setting for all teams is to exclude sub-area paths. We will change it to include sub-areas so that the team gets visibility into all of the work items from all teams. Optionally, the management team could also choose to not include sub-areas, which automatically removes work items from their view as soon as they are assigned to one of the teams.
    

