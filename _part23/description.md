---
type: description
---
2.2.3.1 Quality Model
=====================
Creating a new Quality Model 
The user selects the option of creating a new quality model.  The quality model details are re-quested: name, short name, company and description. If no other quality model is active for the company, the user can define this new quality model as the reference model. The user fills in the information and saves it. The platform stores the model and updates the user interface, as presented in the following figure. 

![Quality Model: Creating a new Quality Model]({{ http://webbook.uqasar.eu }}/part23/img/qm_create.png)

If the quality model does not have any quality objective, the model is marked as incomplete. Alternatively, if the user wishes to cancel the creation, no data is saved.

Defining a Quality Objective 
----------------------------
The user selects the option of creating a new quality objective by adding it to a quality model.
As shown in the following figure, the quality objective details are requested by the platform: name, domain, purpose, development paradigm if the purpose is ‘Process’ and version if the purpose is ‘Product’, description, target audience, acceptance limits, target value, weight and tags. The quality objective can be labelled in order to classify it according to tags or keywords.

![Quality Model: Defining a Quality Objective]({{ http://webbook.uqasar.eu }}/part23/img/qm_createQO.png)

The user fills in the information and saves it. The platform associates the quality objective to the model. If the quality objective does not have any quality indicator, the objective is marked as incomplete. Alternatively, if the user wishes to cancel the creation, no data is saved.

Defining a Quality Indicator 
----------------------------
The user selects the option of creating a new quality indicator by adding it to a quality objective. The following figure shows the indicators details requested by the platform: name, description, target audience and acceptance limits. 

![Quality Model: Defining a Quality Indicator]({{ http://webbook.uqasar.eu }}/part23/img/qm_createQI.png)

The user can select also if the indicator will be applied to a product, selecting its version; or to a development process, selecting the paradigm and life cycle stage. The user fills in the information and saves it. The new quality indicator is associated to the objective. If the quality indicator does not have any metric, the indicator is marked as incomplete. Alternatively, if the user wishes to cancel the creation, no data is saved.
The objectives, indicators and metrics in the quality model will never contain “calculated” data. It will contain the expected value for them, although this value can change during the life of the QA Project.

Defining a Metric 
-----------------
The user selects the option of creating a new metric by adding it to a quality indicator from the quality model tree menu as shown in the following figure.
The details are requested by the platform: name, description, source of the measure, scale and unit. The user fills in the information and saves it. The system stores the information and up-dates the quality model structure. Alternatively, if the user wishes to cancel the creation, no data is saved.

![Quality Model: Defining a Metric]({{ http://webbook.uqasar.eu }}/part23/img/qm_createMetric.png)

Further Quality Model related functionalities on U-QASAR
--------------------------------------------------------
* Importing a new Quality Model
* Exporting a new Quality Model
* Specifying new metrics from the already connected tools
* Specifying metrics that have manual input
* Deleting an existing Quality Model
* Quality Models Tree Filtering by "Status" (Active/Not Active)
* Create New Quality Model item (QO/QI/Metric) by copying a previously created item
* Configuration of hierarchical levels of Quality Model


2.2.3.2 Quality Project
=====================
Using QA Project
----------------
One of the central functionalities of the U-QASAR platform is the management of quality projects.  shows an example of a Quality Project at the U-QASAR Platform. Each project is structured as tree-like structure where Quality Objectives, Indicators and Metrics are presented in relationship to the project. U-QASAR user can add or delete new items, edit existing ones, move the item's locations in the tree etc. In the section to the right the fields of the item are shown, can be viewed and further edited. To make it less painful to search for relevant information there are fields used for filtering data in the upper part of the screen.

Creating QA Projects
--------------------
The user may create quality projects from scratch or use the import functionality to make existing projects available to the platform. 
The user selects the option of creating a new QA project. The project details are requested by the platform from the user: name, acronym, start date, end date, target value, LC Stage, method for the quality average calculation (weighted or not) and description. The user fills in the information and saves it. This results in a new QA project. Alternatively, if the user wishes to cancel the creation, no data is saved.

![Quality Project: Creating a new Quality Project]({{ http://webbook.uqasar.eu }}/part23/img/qp_create.png)


Creating a new QO/QI/Metric for QA Project
------------------------------------------
In order to calculate the quality of a project, several elements are needed in Project’s Tree: Quality Objectives, Quality Indicators and Metrics. These elements should be created depending hierarchically from the Project. There are two ways of doing that: the first one, which consists on selecting a subset of the active Quality Model, has been explained in chapter  Creating QA Projects; the second one, consists on creating one by one the needed elements in Projects' Tree. To do that the user needs to click on the “+” icon at the bottom of the Tree and select which type of element wants to be created, as shown in the following figure:

![Quality Project: Creating a Quality Objective for a Quality Project]({{ http://webbook.uqasar.eu }}/part23/img/qp_createQO.png)
 
By doing that a new window will appear for the user to enter element’s details, which in general are: Name, Description, Thresholds, Target value, Weight and Formula
A Quality Objective is an aggregation of one or more Quality Indicators. At the same time, a Quality Indicator is an aggregation of a set of metrics. In the field named Formula, which exists only for quality objectives and indicators, the mathematical formula for calculating the value of the element using its children’s values is entered. This feature will be explained later in this document (see Section 3.7.1 – Computation of QA Project QO/QI values).
The hierarchy of elements is established by creating each element depending on the corresponding parent in the Tree.
Once all the needed elements are created, they will appear in Projects' Tree:
Each time the user needs to edit the details of an element he/she can do it by clicking on the “Edit” icon which appear on the right side of the screen when the element is selected in the Tree.

Further Quality Project related functionalities on U-QASAR
----------------------------------------------------------
* Deleting a QA Project 
* Create a new QA Project item by copying a previously created entity
* Configuring Thresholds


2.2.3.3 Data Retrieval and Usage (Adapter)
========================================
Configuring Automatic Metrics
-----------------------------
As mentioned before the quality of one Project is measured by aggregations of its children elements. Quality Objectives are aggregations of Quality Indicators and those are aggregations of Metrics. The last element in Project’s hierarchy is the metric. Metrics are used to retrieve measurements and they can be configured to get the data from external tools. Those tools should have been previously set up in the “Adapter Settings” option  (see Section 3.7.8).
To configure automatic Metrics the user has to select the data source in the “Metric Source” field. It should be different from “Manual”, for instance “Static Analysis”. Then, in the “Metric Type” field the specific metric to be retrieved should be selected (see Figure: Configuring automatic metrics): 

![Adapter: Configuring Automatic Metrics]({{ http://webbook.uqasar.eu }}/part23/img/adpt_auto.png)

Inputting the measurement data manually
---------------------------------------
There are plenty of situations where a desired measurement value is not available, the measured value is false, no longer valid, not in a suitable format etc. This leads that the value has to be added/updated manually later. The Quality Project view enables editing of metric values. The metric type and source are set to manual. After this, the metric value can be set and the changes can be saved.

![Adapter: Inputting the measurement data manually]({{ http://webbook.uqasar.eu }}/part23/img/adpt_manual.png)

Retrieving the data automatically from the connected tools (JIRA, SonarQube, TestLink, Cubes, Jenkins, Gitlab)
-------------------------------------------------------------------------------------------------------------- 
For the Integrated Platform, adapters for the JIRA bug tracking system (https://www.atlassian.com/software/jira), the SonarQube code analysis software tool (http://www.sonarqube.org/), the TestLink test management software (http://testlink.org/), the Cubes OLAP Framework (http://cubes.databrewery.org/), Jenkins continuous integration server (https://jenkins-ci-org), and the Gitlab version management server (https://gitlab.com) were implemented. The adapters are used in the Integrated Platform to obtain quality metric data for the platform. The data is parsed, stored internally and may be further viewed, analysed and visualized on the platform etc

Further Data Retrieval and Usage related functionalities on U-QASAR
-------------------------------------------------------------------
* Retrieving Data from JIRA, SonarQube, TestLink, Cubes, Jenkins, Gitlab

2.2.3.4 Reporting and Visualization
=================================
U-QASAR Reporting and Visualization services enable rich visualization of data and generation of reports about project / product quality and status. A set of the available options regarding that is presented below

Projects Visualization
----------------------
From the Projects menu the user can access to the option of visualizing the current values and measurements of the Projects altogether. The option is “Visualize projects”: All the projects which the user has the proper rights to access to, are shown by the system. If more details about one item (Quality Objective, Quality Indicator or Metric) of a specific Project are wanted, the user can access them by clicking on the item. The system then will show item’s details in the corresponding Quality Project Tree.
Whenever a Quality Project is selected in the Project Tree, details of that projects are shown. Apart from details like quality value, thresholds or start date, a graph with the trend of its Quality Objectives along the time is presented under the Historic data. In that graph the user can select which Quality Objectives should be shown:

![Project Visualization]({{ http://webbook.uqasar.eu }}/part23/img/viz_PV.png)

Dashboard Widgets
-----------------
The user dashboard has been mainly designed to present central QA related information in an easily digestible format, i.e. visualizations of quality metrics, and different types of reports. This section presents a couple of sample widgets implemented for the platform and what kind of information the user is able to obtain from those. The general functionalities and use of the dashboards are described in Section 3.7.9 Specifying personal or role based views (dashboards) of measurement data. 

![Project Visualization: Dashboard with sample Widgets]({{ http://webbook.uqasar.eu }}/part23/img/viz_dashboard.png)

The figure illustrates a widget visualizing the computed overall project quality value (Project Quality Widget). The dominant graph on the upper part of the widget shows the current value and the plotted line graph illustrates the historical development of the quality within the project so that the user can get a quick overview, whether the quality is improving or getting worse. 

Historical data
---------------
Continuous monitoring of one Project can inform about its current Quality at one specific moment. However, in order to know the evolution of the Project Quality along the different development lifecycle stages, the corresponding values need to be stored by persisting them in the database as soon as any change is produced.
The Project Quality is calculated by aggregating the different levels of the Project tree. This process is made following a bottom-up approach, it starts retrieving the metric values, followed by the calculation of the quality indicators and objectives; and finally the Project Quality is calculated based on the values of its Quality Objectives. So, whenever a change is produced in one metric, the whole process is repeated, updating the values of all the levels of the tree affected by the change (re-calculations). At this moment, taking a look at the different levels of the Project Tree, their values have been updated and new values have replaced the old ones. Before this replacement happens, the Quality Project / Objective / Indicator / Metric values are persisted in the Historical database.
On every update the platform persists all the new values in the actual database and feeds historical data with the old ones. Evolution of Project values are depicted graphically to fast identify trends and inflexion points. All the values drawn in the graph are also presented in a table ordered by date and can be deleted in case of they are not usable anymore.

Further Reporting and Visualization related functionalities on U-QASAR
----------------------------------------------------------------------
* Drill down metrics
* Exporting reports
* Analytic Workbench
	

2.2.3.5 Enhancement Services
==========================
The enhancement services of U-QASAR are utilized to enhance the data obtained from the analytics services and thus create added value to the information and to the user. 
In the Integrated Platform a set of use cases of enhancement services were implemented: suggestions to make changes to quality objectives, quality indicators and metrics based on the con-text. Also the historical data related to a QA project and the trends detected in the data are used to provide different kinds of suggestions to the user. In addition to those the use of the platform is attempted to be made easier due to the enhancement services, e.g. by providing suggestions for suitable configurations based on the context, e.g. user’s role in the project, and assist the user in creating a new QA project or suggest for a suitable dashboard setup for a user.

![Enhancement Services: System Suggestions as Notifications]({{ http://webbook.uqasar.eu }}/part23/img/es_notifications.png)