# Directed Acrylic Graph Overview

A single DAG is a collection of tasks organized in a way that defines their execution order (It refers to a data pipeline where tasks are executed in a specific sequence without any cycles in the context of Apache Airflow and Cloud Composer)

* The flow of execution doesn't loop back to itself
* Each task in a DAG can depend on the completion of other tasks