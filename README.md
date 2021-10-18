# PySpark_vs_Pandas
The takeaways of using PySpark for distributed data analytics, comparing with other engines/frameworks (Pandas, Dask and Hadoop)

### :zap: PySpark vs Pandas :zap:
Features of Pandas:
- Tabular data
- matured framework and rich features 

Cons of Pandas: 
- Limited to a single machine, cannot be _**distributed** (what PySpark is capable of!)_

A cheatsheet comparing the general usage of PySpark vs Pandas: \
See _PySpark vs Pandas.xlsx_

### :zap: PySpark vs Dask :zap:
Features of Dask: \
Python module for parallel computing
|                  |         PySpark        |             Dask             |
|:----------------:|:----------------------:|:----------------------------:|
|       Scale      | 1-1000 machine cluster |    1-1000 machine cluster    |
|     Ecosystem    |   All-in-one project   | Part of the Python ecosystem |
|  DataFrames/SQL  |     Spark API, SQL     |      Pandas API, no SQL      |
|     Streaming    |    Great performance   |    More complex, difficult   |
| Machine Learning |    Common operations   |  Relies on Python libraries  |
| Graph processing |     GraphX library     |             None             |

### :zap: PySpark vs Hadoop :zap:
Pros: 
- big data platform, with MapReduce as compute system and Hadoop Distributed File System (HDFS) as storage system
- has to read from and write to _disk (While Spark does in **memory**: would require RAM memory, can be more expensive to set up Spark clusters)_

Cons: 
- closely integrated, cannot use in a _**public cloud environment** (AWS, Azure, GCP) (Spark does!)_
- Inefficient in iterative and interactive computing jobs
