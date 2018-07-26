# Pandas_Pivot_Table
PIVOT TABLES

Pandas Pivot Table Explained
Posted by Chris Moffitt in articles   

Introduction
Most people likely have experience with pivot tables in Excel. Pandas provides a similar function called (appropriately enough) pivot_table . While it is exceedingly useful, I frequently find myself struggling to remember how to use the syntax to format the output for my needs. This article will focus on explaining the pandas pivot_table function and how to use it for your data analysis.

If you are not familiar with the concept, wikipedia explains it in high level terms. BTW, did you know that Microsoft trademarked PivotTable? Neither did I. Needless to say, I’ll be talking about a pivot table not PivotTable!

As an added bonus, I’ve created a simple cheat sheet that summarizes the pivot_table. You can find it at the end of this post and I hope it serves as a useful reference. Let me know if it is helpful.

The Data
One of the challenges with using the panda’s pivot_table is making sure you understand your data and what questions you are trying to answer with the pivot table. It is a seemingly simple function but can produce very powerful analysis very quickly.

In this scenario, I’m going to be tracking a sales pipeline (also called funnel). The basic problem is that some sales cycles are very long (think “enterprise software”, capital equipment, etc.) and management wants to understand it in more detail throughout the year.

Typical questions include:

How much revenue is in the pipeline?
What products are in the pipeline?
Who has what products at what stage?
How likely are we to close deals by year end?
Many companies will have CRM tools or other software that sales uses to track the process. While they may have useful tools for analyzing the data, inevitably someone will export the data to Excel and use a PivotTable to summarize the data.

Using a panda’s pivot table can be a good alternative because it is:

Quicker (once it is set up)
Self documenting (look at the code and you know what it does)
Easy to use to generate a report or email
More flexible because you can define custome aggregation functions
