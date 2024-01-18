# athletic_sales_analysis

The code can be found in the repo as athletic_sales_analysis

There was a problem with the datetime format that I initially used where I would get NaT as the value for invoice_date. It wouldn't let me create the last pivot table
where "total_sales" was the value. The TA helped me out before class and we resolved the issue.

This line was the corrected code: merged_sales["invoice_date"]= pd.to_datetime(merged_sales["invoice_date"], errors='coerce') 
