# excel-arrays
In Excel, an array is a collection of values (text, numbers, or logical values) structured in rows and columns. 
Key Array Functions
1. SORT
Purpose: Automatically sorts an array in ascending or descending order.

Syntax:

excel
=SORT(array, [sort_column], [order], [by_col])
order = 1 (ascending), -1 (descending)

by_col = TRUE (sort by column), FALSE (default, sort by row)

2. UNIQUE
Purpose: Extracts distinct values, removing duplicates.

Syntax:

excel
=UNIQUE(array, [by_col], [occurrence])
occurrence = FALSE (all unique values), TRUE (only values appearing once)

Combining Arrays with &
Purpose: Concatenates arrays element-wise (like JOIN in programming).

Syntax:

excel
=array1 & array2
If arrays are different sizes, Excel aligns them and fills mismatches with #N/A.

Dynamic Array Behavior
Results spill automatically into neighboring cells.

Requires Excel 365/2021+ (legacy versions need Ctrl+Shift+Enter for static arrays).

Blocked spill ranges return #SPILL! errors.

Use Cases
Clean and sort datasets dynamically.

Merge columns/text without complex formulas.
