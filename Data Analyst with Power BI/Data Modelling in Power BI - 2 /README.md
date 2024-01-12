### The course cover:
## 1. Date Dimensions & Relationships 
- **Create Date & Time Dimensions** by:
  - Hosting a database
  - Create a text file
  - Creating using DAX ``Calendar()``
-  **Defining Relationships** :
  - **Keys**: Natural key - existing column (e.g. email), Surrogate key - artificial column (e.g. ID), Composite key - a key made up of at leasttwo columns
  - **Cardinality**: one to one, many to many, one to many, many to one
 ### 2. Granularity, measures, and hierarchies
 - **Granularity**:
   - At which level is the data stored with respect to dimensions?
   - Define granularity with ``by`` statement (by product, by customer, by day)
   - Changing granularity by aggregating measures happend in Power Query
 - **Measures**: calcualted and aggregated using DAX
 - **Hierarchies**:
   - Natural: Year >> Month >> Day
   - Artificial: Intake Ywar >> Favourtie Coloir >> Favourite Sport

### 3. Adbacned Data Modelling
- **Relationships**:
  - **Cross-filtering**: selecting a value in one visual narrows down inside data in other visuals
  - **Filter directtions**: single direction, bi-directional directions
  - Bi-directional filtering CANNOT allow for 2 separate paths betwee two tables 
  - 
- Role-play dimensions
  - Dimension that can fileter related facts differenty
  - Sometimes we need to create multiple relationships btw table:
    -  Create multiple relationships on a dimension but only one is active
    -  `` USERELATIONSHIP()`` in DAX to specify which relationship to use
