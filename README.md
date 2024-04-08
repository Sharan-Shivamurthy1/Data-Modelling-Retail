# Data-Modelling-Retail
The repository provides a deeper insight into retail data modelling, data pipelining and data mart creation.

Requirement 1:

The company’s marketing department requests a segmentation of the users to create
dedicated marketing campaigns for these segments. To determine the segments the
Data Science Team wants to cluster the users and needs appropriate features to create
the model.

Tasks:
● Design a data pipeline, which provides a data mart with the next features for
each customer:
- age
- country
- state
- nearest distribution center
- product return rate in the last year
- customer profit level in the last year
Level 1 if the customer has bought products for 50$ or less,
Level 2 - more than 50 but less than 150$,
Level 3 - more than 150$.
What additional features would you recommend? Why?

Solution: 

The file "ETL-Code" gives us the initial ETL script for our requirements. The file further provides us the script for the incremental load as well.

The file "DataMart-SQL" provides the detailed queries for the data mart and the logic for the metrics.

Additional Features:




-----------------------------------------------------------------------------------------------------------------------------
Requirement 2:
You and the Data Science team have created segments and the efforts from the
team are really appreciated by stakeholders. Now the task is to operationalise
the preprocessing flow + model to run weekly. Draw an architecture
diagram/block diagram to show the operationalised pipeline, please feel free to
use your favorite cloud provider or tools known to you.

Solution:

The pipeline is operationalised using AWS. The detailed modelling diagram can be found as "Data Modelling Diagram". The diagram "Scheduling Architecture" depicts the steps chosen for scheduling strategy.

-----------------------------------------------------------------------------------------------------------------------------
