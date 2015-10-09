---
type: description
---
Creating a new Quality Model 
----------------------------
The user selects the option of creating a new quality model.  The quality model details are requested: name, short name, company and description. If no other quality model is active for the company, the user can define this new quality model as the reference model. The user fills in the information and saves it. The platform stores the model and updates the user interface, as presented in the following figure. 


<img src="qm_create.png " width="760" alt="Quality Model: Defining a Quality Model" />


If the quality model does not have any quality objective, the model is marked as incomplete. Alternatively, if the user wishes to cancel the creation, no data is saved.

Defining a Quality Objective 
----------------------------
The user selects the option of creating a new quality objective by adding it to a quality model.
As shown in the following figure, the quality objective details are requested by the platform: name, domain, purpose, development paradigm if the purpose is 'Process' and version if the purpose is 'Product', description, target audience, acceptance limits, target value, weight and tags. The quality objective can be labelled in order to classify it according to tags or keywords.


<img src="qm_createQO.png " width="760" alt="Quality Model: Defining a Quality Objective" />


The user fills in the information and saves it. The platform associates the quality objective to the model. If the quality objective does not have any quality indicator, the objective is marked as incomplete. Alternatively, if the user wishes to cancel the creation, no data is saved.

Defining a Quality Indicator 
----------------------------
The user selects the option of creating a new quality indicator by adding it to a quality objective. The following figure shows the indicators details requested by the platform: name, description, target audience and acceptance limits. 


<img src="qm_createQI.png " width="760" alt="Quality Model: Defining a Quality Indicator" />


The user can select also if the indicator will be applied to a product, selecting its version; or to a development process, selecting the paradigm and life cycle stage. The user fills in the information and saves it. The new quality indicator is associated to the objective. If the quality indicator does not have any metric, the indicator is marked as incomplete. Alternatively, if the user wishes to cancel the creation, no data is saved.
The objectives, indicators and metrics in the quality model will never contain calculated data. It will contain the expected value for them, although this value can change during the life of the QA Project.

Defining a Metric 
-----------------
The user selects the option of creating a new metric by adding it to a quality indicator from the quality model tree menu as shown in the following figure.
The details are requested by the platform: name, description, source of the measure, scale and unit. The user fills in the information and saves it. The system stores the information and up-dates the quality model structure. Alternatively, if the user wishes to cancel the creation, no data is saved.


<img src="qm_createMetric.png " width="760" alt="Quality Model: Defining a Metric" />

