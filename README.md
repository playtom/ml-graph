# ml-graph

This repo shows explanatory ways to create an effective graph structure out of the ml dataset at http://files.grouplens.org/datasets/movielens/ml-20m.zip 

# Prerequisites

* Ubuntu 18.04.1 LTS
* Anaconda 
* Java Runtime Environment (JRE) 
* neo4j
* neo4j-driver
* Jupyter (comes along with Anaconda)
* Python 3.7 (comes along with Anaconda)
* Data file from http://files.grouplens.org/datasets/movielens/ml-20m.zip

# Optional

* vim editor
* Pycharm IDE 

# Neo4J configuration 

In order to ingest your data sources in non-default graph database in Neo4j we need to modify the Neo4j configuration file.

Once you have installed listed software under paragraph "Prerequisites" ensure Neo4j DB is shutdown: 
sudo service neo4j stop

In the configuration file:
/etc/neo4j/conf/neo4j.conf 

vim command:
sudo vim /etc/neo4j/conf/neo4j.conf 

add a line like:
dbms.active_database=ml-graph.db

start neo4j server again:
sudo service neo4j start

# References

* https://www.anaconda.com/download/#linux
* https://neo4j.com/product/
* https://neo4j.com/download/?ref=product
* http://docs.anaconda.com/anaconda/install/linux/
* https://www.anaconda.com/download/#linux
* https://www.ubuntu.com/download/desktop/thank-you?version=18.04.1&architecture=amd64
