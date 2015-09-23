---
type: description
---
U-QASAR Reporting and Visualization services enable rich visualization of data and generation of reports about project / product quality and status. A set of the available options regarding that is presented below

Projects Visualization
----------------------
From the Projects menu the user can access to the option of visualizing the current values and measurements of the Projects altogether. The option is "Visualize projects": All the projects which the user has the proper rights to access to, are shown by the system. If more details about one item (Quality Objective, Quality Indicator or Metric) of a specific Project are wanted, the user can access them by clicking on the item. The system then will show item's details in the corresponding Quality Project Tree.
Whenever a Quality Project is selected in the Project Tree, details of that projects are shown. Apart from details like quality value, thresholds or start date, a graph with the trend of its Quality Objectives along the time is presented under the Historic data. In that graph the user can select which Quality Objectives should be shown:


<img src="viz_PV.png " width="760" alt="Project Visualization" />


Dashboard Widgets
-----------------
The user dashboard has been mainly designed to present central QA related information in an easily digestible format, i.e. visualizations of quality metrics, and different types of reports. This section presents a couple of sample widgets implemented for the platform and what kind of information the user is able to obtain from those. This can be observed in the following figure:


<img src="viz_dashboard.png " width="760" alt="Project Visualization: Dashboard with sample Widgets" />


The figure illustrates a widget visualizing the computed overall project quality value (Project Quality Widget). The dominant graph on the upper part of the widget shows the current value and the plotted line graph illustrates the historical development of the quality within the project so that the user can get a quick overview, whether the quality is improving or getting worse. 

Historical data
---------------
Continuous monitoring of one Project can inform about its current Quality at one specific moment. However, in order to know the evolution of the Project Quality along the different development life cycle stages, the corresponding values need to be stored by persisting them in the database as soon as any change is produced.
The Project Quality is calculated by aggregating the different levels of the Project tree. This process is made following a bottom-up approach, it starts retrieving the metric values, followed by the calculation of the quality indicators and objectives; and finally the Project Quality is calculated based on the values of its Quality Objectives. So, whenever a change is produced in one metric, the whole process is repeated, updating the values of all the levels of the tree affected by the change (re-calculations). At this moment, taking a look at the different levels of the Project Tree, their values have been updated and new values have replaced the old ones. Before this replacement happens, the Quality Project / Objective / Indicator / Metric values are persisted in the Historical database.
On every update the platform persists all the new values in the actual database and feeds historical data with the old ones. Evolution of Project values are depicted graphically to fast identify trends and inflexion points. All the values drawn in the graph are also presented in a table ordered by date and can be deleted in case of they are not usable any more.
