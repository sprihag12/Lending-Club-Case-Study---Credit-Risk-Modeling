# Lending Club Case Study - Credit Risk Modeling

The case study was a part of the Machine Learning for Problem Solving graduate-level course (95-828) at Carnegie Mellon University and was divided into 3 phases:
Phase 1: Intended to understand the motivation behind the problem statement, working on P2P lending, and data overview. Some of the questions answered were:
i) Note that loans are temporal entities (36 or 60 months-long terms). Different loans could default at different times; some will default soon after approval, some much
later. Some, on the other hand, might be repaid early, before their term ends. Would these facts affect your downstream analysis and decision-making? How/Why?
ii) When investing in future loans, could you train a model that uses total pymnt as a variable? Why (not)?
iii) It is unclear whether the values of the variables in the dataset are current as of the date the loan was issued, or as of the date the data were provided. (For
example, suppose we download the data in Dec 2017, and consider the feature fico range low for a loan that was issued in Jan 2015. It is unclear whether the score listed was 
the score in Jan 2015, or the score in Dec 2017.) Would this matter for your downstream modeling? Why (not)?

Phase 2: Intended to perform a preliminary analysis of data including cleaning, preparation, and exploration.  This included removing outliers, identifying correlations and 
calculating returns ( a new feature engineered). 3 separate methods were used to assess - M1 supposes that, once the loan is paid back, the investor is forced to sit with the money
without reinvesting it anywhere else. M2 supposes that, once the loan is paid back, the investor's money is returned and the investor can immediately invest in another loan
with the same return. M3 considers a mixed time horizon (e.g., T months) and assumes that any revenues paid out from a loan are immediately reinvested at a yearly rate
of i%, compounded monthly, until the T-month horizon is over. Loan grades were assessed against the 3 methods to analyze the accuracy of these methods.

Phase 3: Intended to employ predictive analytics (evaluated several models against multiple metrics) to predict how likely a loan is to default. Based on the results, built
investment strategies for investors from the following: random/ default based/ returns based/ default& returns based. Assessed these against the methods described in Phase 2 to 
select the best strategy that would work on 1000 loans.


Acknowledgments:
Cohen MC, Guetta CD, Jiao K, Provost F. (2018) Data-driven investment strategies for peer-to-peer lending: a case study for teaching data science. Big Data 6:3, 191213, 
DOI: 10.1089/ big.2018.0092.
