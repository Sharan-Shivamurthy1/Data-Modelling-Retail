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

When designing a customer segmentation data mart,  there were some additional features that I recommend including, along with reasons why they could be valuable. Some of them are:

a) Customer Lifetime Value (CLV Decay in business terms)
An estimation of the total value a business can expect from a single customer account throughout the business relationship.
Reason: CLV helps in identifying high value customers over time, allowing for more targeted marketing strategies and resource allocation.
b) Frequency of Purchases
The number of purchases a customer makes within a given timeframe can  be included.
Reason: Understanding purchase frequency can help in recognizing loyal customers and planning campaigns to increase retention or re-engage less active customers.
c) Product Preferences
Categorization of customers based on the types of products they purchase.
Reason: Knowing product preferences allows for more targeted product recommendations and personalized marketing messages.
d) Channel Preference
The preferred communication or sales channel of the customer (e.g., email, social media, in-store).
Reason: Channel preference can optimize the effectiveness of marketing campaigns by reaching customers through their preferred mediums.


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
