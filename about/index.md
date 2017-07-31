---
layout: page
title: About
tags: [about, resume, cv]
date: 2016-10-30
comments: false
---

I work as a Senior Engineer on the Core ML team for Amazon.com. The opinions here are my own and do not represent my employer. Previously, I worked as the technical lead of the R&D team for ARGO Data. We used data science to solve challenging problems in banking and healthcare. I have 10+ years of industry experience building high-volume, distributed transaction processing systems. My academic background includes a PhD in Computer Science and publications in Natural Language Processing, Probabilistic Graphical Models, and Data Mining. I split my time between data science, research engineering, and software architecture responsibilties.

## Technology & Skills

Engineering

* **Language Expertise**: Java, Python, Groovy, Scala, C#/.NET, C++14, SQL
* **Data Mining, Machine Learning**: jPMML, Mallet, scikit-learn, NumPy, Pandas, Matplotlib, KNIME, Weka, Factorie, NLTK, Deeplearning4j, Spark MLLib
* **Infrastructure**: Spark, Spark Streaming, Hadoop, Elasticsearch, Spring, Spring Boot, Hibernate/JPA, Jooq
* **Storage**: MSSQL, Oracle, Cassandra, GridGain/Ignite, Kafka, HDFS

Computer Science

* **Natural Language Processing**: parsing, grapheme to phoneme (G2P) transduction, structured prediction, topic modeling, sentiment anlaysis
* **Data Mining**: record linkage, clustering, learning to rank, fuzzy matching, Levenshtein automata
* **Statistics, Learning**: probabilistic graphical models, logistic regression, regularization, Bayesian treatments, hypothesis testing, survival analysis, time-series analysis, neural networks, optimization
* **Database Systems**: query optimization, optimizing storage subsystems for SSDs
* **Distributed Systems**: distributed hash tables, routing, distributed two-phase commit

## Work Experience

### Amazon.com (2017-Present) - Seattle, WA

Senior Software Engineer - Machine Learning, Big Data. Core ML Group.

### ARGO Data (2010-2017) - Memphis, TN

Analytic Science Group, Lead; Software Architect

* Collaborate with C-level executives and product owners to identify opportunities where intelligent analytic solutions can provide value to our products
* Develop strategies to scope, prioritize, and deliver intelligent solutions
* Lead a team of 5 data scientists and research engineers to execute projects
* Perform data science tasks, such as exploration, visualization, modeling, and experimentation
* Engineer production-ready components to deploy analytic solutions into our commercial products
* Participate in sales support activities that communicate value and credibility to prospective customers
* Accountable for design and architecture responsibilities for multiple software projects across the company
* Performance engineering for database and Java application performance optimization
* New project team bootstrapping to establish initial design, architecture, and toolchain

#### Project Overview

* **Master Patient Index** (EMPI): resolving the identities of patients across multiple care facilities. Developed state-of-the-art solution which empirically beats competitors in accuracy. The solution enhances the traditional Fellegi-Sunter probabilistic formulation by incorporating informative priors and modeling interaction/dependence. We use NLP techniques, supervised ML, and sophisticated data quality models to match using the semantic information in noisy data records. This solution is in production in numerous integrated facilities and health information exchanges in Texas, Oklahoma, New York, and California.
* **Patient re-admission risk** predictive modeling: predicting risk of unexpected re-admission for patients based on medical history, social factors, episode and discharge features to improve the quality of care and reduce the risk of hopsital CMS penalties.
* Multi-cultural **personal name parsing** using a pipeline design with structured prediction, gender and culture classification, and re-ranking
* Semi-structured **address parsing** using Conditional Random Fields and USPS and Census data (patent pending US 20160147943).
* Detecting **check fraud** in batch-processing banking transactions. We deploy champion/challenger models with offline re-training. This is running in production at a large multi-bank processor. We achieved a ~90% detection rate with < 2% review rate, beating our competitor.
* Branch teller **real-time fraud detection** and compliance. Lead both the architecture, software design, and analytics development for ARGO's Teller-integrated fraud detection solution. This is a distributed, highly available solution that does metadata analysis of teller transactions to prevent loss at the branch. In addition, the solution tracks cash and monetary instruments for compliance reporting. This is in production with more customer implementations in progress.
* Cash Inventory Optimization **forecasting cash needs** at branches and ATMs to reduce cost.
* **Customer attrition risk** predictive modeling to indicate which customers are likely to be risk of leaving the institution.
* Semi-structured **text topic modeling**, summarization, and sentiment analysis for customer complaint workflow optimization.
* String similarity measurement and clustering at scale (patent US9129010 B2).
* Low-level integration libraries to bridge a proprietary 4th Generation Language to the .NET CLR handling marshalling and tracing.

### FIS (previously Metavante, VectorSGI; 2006-2010)

Software Engineer, II

* Worked on a small team of software developers building new versions of the VECTOR:Image Exchange product, which is in production at dozens of top-50 banks in the USA
* Designed and engineered new features working with business analysts, product management, quality assurance, and support to scope and prioritize work 
* Executed Java and MSSQL Database performance engineering to increase throughput to over 30M transactions per day in a small window of time

## Education

* **PhD, Computer Science**. University of Memphis. 2017.
  * Dissertation Title: "Improving Accuracy of Patient Demographic Matching and Identity Resolution"
* **MS, Computer Science**. University of Memphis. 2012.
* **BA, Computer Science**. Rhodes College. 2006.

## Publications
* Stephen Ash (2017). **Improving Accuracy of Patient Demographic Matching and Identity Resolution** (Doctoral dissertation). University of Memphis. Retrieved from [https://umwa.memphis.edu/etd/](https://umwa.memphis.edu/etd/).
* Stephen Ash and David Lin. 2016 (In Press). **Incorporating syllable phonotactics to improve grapheme to phoneme translation**. _Future and Emerging Trends in Language Technologies (FETLT 2016)_.
* Stephen Ash and David Lin. 2016. **Grapheme to phoneme translation using conditional random fields with re-ranking**. _Proceedings of the 19th International Conference on Text, Speech, and Dialogue (TSD 2016)_, 314-325. [http://link.springer.com/chapter/10.1007/978-3-319-45510-5_36](http://link.springer.com/chapter/10.1007/978-3-319-45510-5_36)
* Stephen Ash and David Lin. 2015. **Embracing the sparse, noisy, and interrelated aspects of patient demographics for use in clinical medical record linkage**.  _AMIA Summits on Clinical Research Informatics 2015_, 425-429. [https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4525218/](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4525218/)
* Stephen Ash and David Lin. 2014. **The discriminating power of information within patient demographics for clinical medical record linkage**. _Global Identity Summit (GIS 2014)_. Invited Talk.
* Stephen Ash and David Lin. 2014. **Optimizing database index performance for solid state drives**. _Proceedings of the 18th International Database Engineering & Applications Symposium (IDEAS '14)_, 237-246. [http://dl.acm.org/citation.cfm?id=2628255](http://dl.acm.org/citation.cfm?id=2628255).

## Patents

* Stephen Ash and Jerry Bowman. 2015. **System and method of partitioned lexicographic search**. US Patent No. US9129010 B2, Filed May 16, 2011, Issued Sept. 8, 2015.
* Stephen Ash and Michael Siler. 2014. **Semantic address parsing using a graphical discriminative probabilistic model**. US Patent Application No. 20160147943, Filed Nov. 21, 2014.


## Awards

* **2nd Place Student Research Symposium**. University of Memphis. 2012. Research in Neural Networks for object identification and extraction on banking check images.
* **Metavante Key Results**. Metavante. 2008. Awarded by a director to employees that uniquely contribute to success of key corporate strategic goals.
* **President's Award**. Tristate Independant Theatre Association. 2008. Awarded to a single individual each year for leadership and contribution to business initiatives.
* **Jack U. Russell Award** for Outstanding Work in Computer Science. Rhodes College. 2006. Awarded by the faculty of the Math and Computer Science department at Rhodes College to a graduating senior for outstanding work during their undergraduate career.
* **Outstanding Work in First-Year Computer Science**. Rhodes College. 2004. Awarded by the faculty of the Math and Computer Science department at Rhodes College for outstanding work during the first year of study in the department.
