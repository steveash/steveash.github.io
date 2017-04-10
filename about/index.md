---
layout: page
title: About
tags: [about, resume, cv]
date: 2016-10-30
comments: false
---

I work as the lead of the Analytic Sciences Group (ASG), the R&D team for ARGO Data. We work across ARGO to use data science to solve challenging problems in banking and healthcare. I have 10+ years of industry experience building high-volume, distributed transaction processing systems. My academic background includes a PhD in Computer Science and publications in Natural Language Processing, Probabilistic Graphical Models, and Data Mining. I split my time between data science, research engineering, and software architecture responsibilties.

## Technology & Skills

* **Language expertise**: Java, Python, Groovy, C#/.NET, C++14, SQL
* **Data Mining, Machine Learning**: jPMML, Mallet, scikit-learn, NumPy, Pandas, Matlib, KNIME, Weka, Factorie, NLTK, Deeplearning4j
* **Infrastructure**: Spark, Spark Streaming, Hadoop, Elasticsearch, Spring, Spring Boot, Hibernate/JPA, Jooq
* **Storage**: MSSQL, Oracle, Cassandra, GridGain/Ignite, Kafka, HDFS

* **Natural Language Processing**: Grapheme to Phoneme (G2P) transduction, Parsing, Probabilistic Graphical Models, Structured Prediction
* **Database Systems**: Query Optimization, Optimizing Storage Subsystems for SSDs
* **Distributed Systems**: distributed hash tables, routing, distributed two-phase commit
* **Statistics**: record linkage, classification, logistic regression, regularization, bayesian treatments, hypothesis testing, survival analysis, time-series analysis

## Work Experience

### ARGO Data (2010-Present)

Analytic Science Group, Lead; Software Architect

* Work with C-level executives and product owners to identify opportunities where intelligent analytic solutions can provide value to our products
* Develop strategies to scope, prioritize, and deliver intelligent solutions in line with company initiatives and strategy
* Lead a team of 5 data scientists and research engineers to execute projects
* Perform data science tasks such as exploration, visualization, modeling, and experimentation
* Engineer production-ready components to deploy analytic solutions into our commercial products
* Participate in sales support activities to communicate the value and credibility of ARGO analytic solutions to prospective customers
* Accountable for design and architecture responsibilities for multiple software projects across the company
* Performance engineering for database and Java application performance optimization
* New project team bootstrapping to establish initial design, architecture, and toolchain

#### Project Overview

* Healthcare Master Patient Index (EMPI): resolving the identities of patients across multiple care facilities. Developed state-of-the-art solution which empirically beats competitors in accuracy. The solution enhances the traditional Fellegi-Sunter probabilistic formulation by incorporating informative priors and modeling interaction/dependence. We use NLP techniques, supervised ML, and sophisticated data quality models to match using the semantic information in noisy data records. This solution is in production in numerous integrated facilities and health information exchanges in Texas, Oklahoma, New York, and California.
* Patient re-admission risk predictive modeling: predicting risk of unexpected re-admission for patients based on medical history, social factors, episode and discharge features to improve the quality of care and reduce the risk of hopsital CMS penalties.
* Multi-cultural personal name parsing using a pipeline design with structured prediction, gender and culture classification, and re-ranking
* Semi-structured address parsing using Conditional Random Fields and USPS and Census data (patent pending US 20160147943).
* Detecting check fraud in batch-processing banking transactions. We deploy champion/challenger models with offline re-training. This is running in production at a large multi-bank processor. We achieved a ~90% detection rate with < 2% review rate, beating our competitor.
* Branch teller real-time fraud detection and compliance. Lead both the architecture, software design, and analytics development for ARGO's Teller-integrated fraud detection solution. This is a distributed, highly available solution that does metadata analysis of teller transactions to prevent loss at the branch. In addition, the solution tracks cash and monetary instruments for compliance reporting. This is in production with more customer implementations in progress.
* Cash Inventory Optimization forecasting cash needs at branches and ATMs to reduce cost.
* Customer attrition risk predictive modeling to indicate which customers are likely to be risk of leaving the institution.
* Semi-structured text topic modeling, summarization, and sentiment analysis for customer complaint workflow optimization.
* String similarity measurement and clustering at scale (patent US9129010 B2).
* Low-level integration libraries to bridge a proprietary 4th Generation Language to the .NET CLR handling marshalling and tracing.

### FIS (previously Metavante, VectorSGI; 2006-2010)

Software Engineer, II

* Work on a small team of software developers building new versions of the VECTOR:Image Exchange product in production at dozens of top-50 banks in the USA
* Design and engineer new features working with business analysts, product management, quality assurance, and support to scope and prioritize work 
* Execute Java and MSSQL Database performance engineering to increase throughput to over 30M transactions per day in a small window of time

## Education

* **PhD, Computer Science**. University of Memphis. 2017.
  * Dissertation Title: "Improving Accuracy of Patient Demographic Matching and Identity Resolution"
* **MS, Computer Science**. University of Memphis. 2012.
* **BA, Computer Science**. Rhodes College. 2006.

## Publications

* Ash, Stephen; Lin, David. **Incorporating Syllable Phonotactics to Improve Grapheme to Phoneme Translation**. Future and Emerging Trends in Language Technologies FETLT 2016 (in press).
* Ash, Stephen; Lin, David. **Grapheme to Phoneme Translation using Conditional Random Fields with Re-ranking**. TSD 2016 Proceedings of the 19th International Conference on Text, Speech and Dialogue. 2016. [http://link.springer.com/chapter/10.1007/978-3-319-45510-5_36](http://link.springer.com/chapter/10.1007/978-3-319-45510-5_36)
* Ash, Stephen; Lin, David. **Embracing the Sparse, Noisy, and Interrelated Aspects of Patient Demographics for use in Clinical Medical Record Linkage**. AMIA Summits on Clinical Research Informatics 2015. 2015. [https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4525218/](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4525218/)
* Ash, Stephen; Lin, David. **The Discriminating Power of Information within Patient Demographics for Clinical Medical Record Linkage**. GIS 2014 Global Identity Summit. 2014. _Invited Talk_.
* Ash, Stephen; Lin, David. **Optimizing database index performance for solid state drives**. IDEAS '14 Proceedings of the 18th International Database Engineering & Applications Symposium. 2014. [http://dl.acm.org/citation.cfm?id=2628255](http://dl.acm.org/citation.cfm?id=2628255).

## Patents

* Ash, Stephen; Siler, Michael. US Patent Application US 20160147943. **Semantic Address Parsing Using a Graphical Discriminative Probabilistic Model**. 21 November 2014.
* Ash, Stephen; Bowman, Jerry. US Patent US9129010 B2. **System and Method of Partitioned Lexicographic Search**. 16 May 2011.

## Awards

* 2nd Place Student Research Symposium. University of Memphis. 2012. Research in Neural Networks for object identification and extraction on banking check images.
* Metavante Key Results. Metavante. 2008. Awarded by a director to employees that uniquely contribute to success of key corporate strategic goals.
* President's Award. Tristate Independant Theatre Association. 2008. Awarded to a single individual each year for leadership and contribution to business initiatives.
* Jack U. Russell Award for Outstanding Work in Computer Science. Rhodes College. 2006. Awarded by the faculty of the Math and Computer Science department at Rhodes College to a graduating senior for outstanding work during their undergraduate career.
* Outstanding Work in First-Year Computer Science. Rhodes College. 2004. Awarded by the faculty of the Math and Computer Science department at Rhodes College for outstanding work during the first year of study in the department.
