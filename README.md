# SEC_DB
Securities Database

This database contains the structure and function for the Securities Database or SEC_DAT.  The database is key to the investment sourcing and scoring process used by BAR Capital.  


Overview of Process
The SEC_DAT is used to generate the one page summary sheet used to evaluate investment ideas.  The data is sourced from EDGAR and valuation ratios and F-Score calculations are applied.  Basic information about the stock is also presented.  The database will be updated on a weekly basis.  The broader process includes the following steps:
  1) Collection of data points
  2) Calculation of relevant ratios and scores
  3) Ranking of investment opportunities
  4) Output of summary 

Data Sourcing 
The data will be pulled from the SEC website using a Python program.  Once the basic information about the securities is downloaded, MySQL database is used to store base information.  

Calculations
Calculations are now performed to determine the F-Score as well as valuation ratios.  The scoring methodology is run across all companies that filed an earnings statement in the prior and upcoming 4 week period.  This narrowing of focus allows for a more maneagable grouping as well as relevancy due to stock price movements around public disclosures.  

Ranking Methodology
The investment choices will be ranked according to F-Score and attractiveness based on financial and valuation ratios.   Once the ranking methodology is complete, the top quartile of most attractive investment choices will be displayed along with the most important scoring factors.  

Output
The final output screen is the one page summary of the investment opportunity.  This page will display the key aspects of the company that  are needed to determine whether it should be further researched or deferred for future review.  
