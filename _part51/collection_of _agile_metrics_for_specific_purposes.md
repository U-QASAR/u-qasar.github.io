---
title: Collection of Agile Metrics for Specific Purposes
type: flyer
---
<embed src="Metrics_summary_by_purpose.pdf" width="500" height="375" type='application/pdf'>
<h2>Spring and project planning</h2>
<h3>Prioritization</h3>
Prioritization of tasks is one of the main purposes of metrics in agile sprint and project planning. Various metrics are used to support prioritization decisions:

* Effort estimates 
* cost types
* rate of requirements over phases
* variance in handovers
* lead time
* revenue per customer

<h3>Scoping</h3>
Scoping metrics are needed to estimate the size and number of features when planning the contents of a sprint or release. 

* Effort estimate metrics provide the estimate of the size 
* Velocity is a central metric in agile development that measures the actual productivity of a team 
* Lead time metrics reveal if the task could be completed by the end of the release 

<h3>Resourcing</h3>
In resourcing the metrics are used to plan the resources match the tasks at hand and identify dependencies

* The expected date of task completion metric helps analysing the task dependencies
* Effort estimates, required skills, and predicted number of defects are useful for planning the resourcing.

<h2>Sprint and Project Tracking</h2>
The purpose of the use of metrics in progress tracking is divided into project progress, increasing visibility, achieving goals, and balancing workflow.

<h3>Project progress</h3>
Metrics that are used to monitor the progress number of completed features(or completed web pages for example)

* number of passing automated tests
* burn-down
* The release burndown metric and graphs show project progress trends and can be used to predict the completion date or more importantly indicate the need for re-scoping by addition or removal of stories or tasks. 

<h3>Increasing visibility</h3>
Metrics work as a way to simplify complex aspects of software development and provide visibility for all stakeholders. 

* Cost types, rate of requirements over phases, and variance in handovers can be used to increase the transparency of end-to-end flow in a complex system. 
* The technical debt board is a measurement instrument that can be used to make technical debt issues visible and help managing and reacting to technical debt. 
* The common progress tracking metrics are good for increasing the visibility of project status among variety of stakeholders, not just project manager. 
* Burn-down graphs, check-ins per day, number of passing automated tests, number of open and new defects metrics are beneficial. 
* The defect trend indicators, cycle time metrics, and metrics for completed stories have been found useful in agile teams.

<h3>Achieving goals</h3>
Certain metrics help to understand whether project goals could be achieved and to highlight the need for scope cut-down, if it seems that all tasks cannot be completed at the current pace. 

* Common tempo time can act as a simple indicator of workload imbalance. Common tempo time measures net available work days per required work units. 
* Release burndown make the relationship clear between work remaining and the team's progress and indicates clearly if the goal is going to be achieved with the current pace.
* Story flow percentage, i.e., the actual implementation effort per estimated effort, describes how efficiently developers are performing in comparison to the plan.

<h3>Balancing workflow</h3>
Metrics are efficient tool to balance workflow and prevent overloading certain people. 

* The common tempo time is a simple metric that measures the relationship between available effort and planned or required tasks. This gives a high level overview of the workload of a team or individual people.
* Following the inventory of requirements over time or measuring requirements per phase can reveal large handovers or peaks of requirements that would cause overloading situations to employees. 
* Measuring check-ins per day can help make developers to commit code to the main trunk regularly. This would prevent overly large commits towards the end of a sprint causing a lot of integration and quality problems and, thus, peak workload.
* Setting task size limits, e.g., measured by story points, is another way of preventing large tasks blocking other work and causing integration challenges. 

<h2>Understanding and Improving Quality</h2>
Metrics can be applied to understand the level of quality and improve the quality. Another approach is to use metrics to ensure that the product is tested thoroughly.

<h3>Understand the level of quality</h3>
The level of product quality can be measured after the release or before the release. 

* Net Promoter Score can be used to measure both pre-release and post-release quality by asking pre-release users or customers in customer surveys. 
* Number of change requests from the customer is a direct indicator of customer satisfaction.
* Maintenance effort is an indicator of overall, both internal and external, quality of the released product. 
* Number of maintenance requests is another way of quantifying the post-release quality.
* Numbers of defects in different pre-release testing phases. 
* Number of deferred defects, i.e., known defects not fixed for the release, can indicate the level of quality customers would experience. 

<h3>Increase quality</h3>
* Metrics can be used as governance mechanisms, for example, burn-down, check-ins per day, and number of automated passing test steps, work as a governance mechanisms to promote development behavior that contributes to increasing product quality.
* Build status measure ensures that broken versions do not proceed in the build pipeline.
* Number of unit tests, test coverage, and test growth ratio measure the rigorousness of the testing practices
* Violations of static code analysis is used to prevent critical violations
* Technical debt board is useful for reducing technical debt.

<h3>Ensure the level of testing</h3>
A very central aspect of agile and lean development principles is the reliance on thorough testing and emphasis on automation. Many metrics can be used to ensure that the testing process is working properly and the developed code is well tested.

* Number of passing automated tests is the simplest metric for assessing the thoroughness of testing and ensuring that there are no untested areas in the code base
* Test coverage metrics are a common and straightforward way of analyzing the extent of testing. 
* The test growth ratio can be better metric in contexts where there is a large legacy code base without many tests. 
* Monitoring cycle times reveals testing activities that require high effort or calendar time and, thus, are good candidates for automation. 
* Number of written and passed unit tests should be constantly increasing in normal situation.

<h2>Fixing Process Problems</h2>
Value Stream Maps (VSM) are used to spot waste in several phases of the development process. 

* First, lead time, processing time, and queue time metrics are used to identify waste, i.e., time features spend in different waiting states during development and before deployment to customers.
* Rate of requirements over phases, cumulative number of work items, and variance in handovers are metrics that can be used to track flow of requirements and features to reveal bottlenecks in the development process. 
* Throughput and queue time metrics can also be used as bottleneck indicators.
* Defect trend indicator to identify problems with the defect backlog by estimating the expected change in the defect backlog
* Story percent complete to see the early symptoms of various problems that can cause delays
* Work in progress was used to identify blocked work items and the development phase where the blockage occur 
* Inventory of requirements over time to identify problems in the continuous flow of fea-tures
* Velocity to improve throughput and estimating capability
* Burn-down to identify deviation from iteration plan
* Story flow and implementation flow metrics to identify implementation challenges that need to be addressed
* Number of work items per phase to identify development overload situation
* Fix time of broken builds and violations to static code analysis metrics to detect decrease in code quality

<h2>Motivating people</h2>
Metrics can serve as concrete indicators providing hard evidence and visibility for people. This way metrics motivate people to react faster to problems. 

* Common ways of using metrics for motivational purposes are various forms of radiators and dashboards that make the selected metrics highly visible in the working environment. 
* Simple metrics, such as the number of defects or broken builds, can be shown in monitors to make teams constantly aware of the development situation and motivate to improve the measured aspects. 
* Showing reported and open defects, test failure rate, and test success rate on monitors motivating people to avoid problems and fix the problems fast. 
* Showing broken build fix time keeps people aware of the long fix time problem, provokes discussion about the causes, and leads to fix time improvements.
* Keeping build status visible in real time helps to create a culture of reacting with high priority to broken builds.
* Provide developers immediate feedback of violations to static code analysis to motivate them to keep the coding style and quality high at all times. 
* Defect trend indicator can be used to create crisis awareness and motivate the developers to take actions to avoid bigger problems
