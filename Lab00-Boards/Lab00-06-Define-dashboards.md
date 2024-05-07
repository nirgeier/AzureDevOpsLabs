
Agile planning and portfolio management with Azure Boards
=========================================================

Lab requirements
----------------

* **Completion of previous labs**
    
Objectives
----------

After you complete this lab, you will be able to:

*   Define dashboards.

Instructions
------------

### Exercise: Define dashboards

* In this task, you will step through the process of creating dashboards and their core components.

* Dashboards allow teams to visualize status and monitor progress across the project. 
* At a glance, you can make informed decisions without having to drill down into other parts of your team project site. 
* The Overview page provides access to a default team dashboard which you can customize by adding, removing, or rearranging the tiles. 
* Each tile corresponds to a widget that provides access to one or more features or functions.

---

1.  In the vertical navigational pane of the Azure DevOps portal, select the **Overview** icon and, in the list of the **Overview** items, select **Dashboards**.
2.  If necessary, on the **Dashboards** pane, in the upper left corner, in the **eShopOnWeb Team** section, select **eShopOnWeb Team - Overview** and review the existing dashboard.
    
     ![If necessary, on the "Dashboards" pane, in the upper left corner, in the "eShopOnWeb Team" section, select "eShopOnWeb Team - Overview"](./images/EShop-WEB-dashboard_v1.png)
    
3.  On the **Dashboards** pane, select the drop-down menu next to the **eShopOnWeb Team - Overview** title, and select **\+ New dashboard**.
    
     ![On the "Dashboards" pane, in the upper left corner, in the "eShopOnWeb Team" section, select "+ New dashboard"](./images/new_dashboard_v1.png)
    
4.  On the **Create a dashboard** pane, in the **Name** textbox, type **Product training**, in the **Team** dropdown list, select the **EShop-WEB** team, and click **Create**.
    
     ![On the "Create a dashboard" pane, in the "Name" textbox, type "Product training", in the "Team" dropdown list, select the "EShop-WEB" team, and click "Create"](./images/EShop-WEB-create_dash_v1.png)
    
5.  On the new dashboard pane, click **Add a widget**.
6.  On the **Add Widget** panel, in the **Search** textbox, type **sprint** to find existing widgets that focus on sprints. In the list of results, select **Sprint Overview** and click **Add**.
7.  In the rectangle representing the newly added widget, click the **Settings** cogwheel icon and review the **Configuration** pane.
    
     > **Note**: The customization level will vary by widget.
    
8.  On the **Configuration** pane, click **Close** without making any changes.
9.  Back on the **Add Widget** pane, in the **Search** textbox, type **sprint** again to find existing widgets that focus on sprints. In the list of results, select **Sprint Capacity** and click **Add**.
10.  In the **Dashboard** view, at the top of the pane, click **Done Editing**.
    
     ![Review finished dashboard should include both widgets](./images/EShop-WEB-finished_dashboard_v1.png)
    
     > **Note**: You can now review two important aspects of your current sprint on your custom dashboard.
    
     > **Note**: Another way of customizing dashboards is to generate charts based on work item queries, which you can share to a dashboard.
    
11.  In the vertical navigational pane of the Azure DevOps portal, select the **Boards** icon and, in the list of the **Boards** items, select **Queries**.
12.  On the **Queries** pane, click **\+ New query**.
13.  On the **Editor** tab of **Queries > My Queries** pane, in the **Value** dropdown list of the **Work Item Type** row, select **Task**.
14.  On the **Editor** tab of **Queries > My Queries** pane, in the second row, in the **Field** column, select **Area Path** and, in the corresponding **Value** dropdown list, select **eShopOnWeb\\EShop-WEB**.
15.  Click **Save query**.
    
     ![On the "Editor" tab of "Queries > My Queries" pane, in the second row, in the "Field" column, select "Area Path" and, in the corresponding "Value" dropdown list, select "eShopOnWeb\EShop-WEB"](./images/EShop-WEB-query_v1.png)
    
16.  In the **New query** panel, in the **Enter name** textbox, type **Web tasks**, in the **Folder** dropdown list, select **Shared Queries**, and click **OK**.
17.  From the **Queries>Shared Queries** view, select the **Charts** tab and click **\+ New chart**.
18.  On the **Configure Chart** panel, in the **Name** textbox, type **Web tasks - By assignment**, in the **Group by** dropdown list, select **Assigned To**, and click **Save Chart** to save the changes.
    
     ![On the "Configure Chart" panel, in the "Name" textbox, type "Web tasks - By assignment", in the "Group by" dropdown list, select "Assigned To", and click "OK" to save the changes](./images/EShop-WEB-chart_v1.png)
    
     > **Note**: You can now add this chart to a dashboard.
    
19.  Return to the **Dashboards** section in the **Overview** Menu. From the **EShop-Web** section, select the **Product Training** dashboard you used earlier, to open it.
    
20.  Click **Edit** from the top menu. From the **Add Widget** list, search for **Chart** , and select **Chart for Work Items**. Click **Add** to add this widget to the EShop-Web dashboard.
    
21.  Click the **configure** (cogwheel) within the **Chart for Work Items** to open the widget settings.
    
22.  Accept the title as is. Under **Query**, select **Shared Queries / Web Tasks**. Keep **Pie** for Chart Type. Under **Group By**, select **Assigned To**. Keep the Aggregation (Count) and Sort (Value / Ascending) defaults.
    
23.  Confirm the configuration by clicking **Save**.
    
24.  Notice the query results pie chart is shown on the dashboard. **Save** the changes by pressing the **Done Editing** button on top.
