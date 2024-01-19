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

### DAX for calculated tables and columns
- One can use DAX to clean data. For example ```SUBSTITUTE()```
- New coluns ```Costs = Total revenue - Profit```
## Chapter 2 - DAX and Measures 
### Implicit measures 
- AUTOMATICALLY created by Power BI
- COme directly from database
- Example: drag ```Sales``` to table visaul =< SUM(Sales) automatically created
### Explicit measures 
- Writing measures in an explicit way
- E.g.: Total Sales = SUM(Orders[Sales])
- Offer flexibility
#### Use variable to improve formulas 
```
--- Calculate the sales from last year and store it as a variable
VAR SALESPRIORYEAR = CALCULATE([SALES],SAMEPERIODLASTYEAR('DATE'))
RETURN
--- Use the variable in a formula
Sales growth = [Sales] - SALESPRIORYEAR
```
## Chapter 3 - Filtering and counting with DAX 
## Chapter 4 - Interating Functions 
