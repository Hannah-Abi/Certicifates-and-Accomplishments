## Chapter 1 - Data Models with DAX
### DAX for creating tables and columns 
- DAX formulas include functions, operators and values to perform advanced calculations
- DAX formulas are used in: Measures, Calculated columns, Calculated tables, Row-level security
- DAX formula depends on the 3 types of contents: ROW, QUERY, FILTER context.
    1. Row context:
        - "The current row"
        - DAX formula for calculated columns columns evaluate at ROW level
    2. Query context:
        - Refers to the subset of data that is implicitly retrieved for a formula
        - Controlled by **slicers, page filters, table columns** and **row headers**
        - Controlled by **chart/visual filters**
        - Applies after row context
    3. Filter context:
        - The set of values allowed in each column, or in the values retrieved from a related table
        - By using arguments to a formula or by using report filters on row and column headings
        - Applies after query context

### DAX for calcualted tables and columns
## Chapter 2 - DAX and Measures 
## Chapter 3 - Filtering and counting with DAX 
## Chapter 4 - Interating Functions 
