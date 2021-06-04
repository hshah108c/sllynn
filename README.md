# spark-xgboost

Spark users can use XGBoost for classification and regression tasks in a distributed environment through the excellent [XGBoost4J-Spark](https://xgboost.readthedocs.io/en/latest/jvm/xgboost4j_spark_tutorial.html) library. As of July 2020, this integration only exposes a Scala API. A [PR](https://github.com/dmlc/xgboost/pull/4656) is open on the main XGBoost repository to add a Python equivalent, but this is still in draft. 

This repository contains the Python wrapper components from that PR. By building and installing the appropriate .whl (see 'releases' in this repository), PySpark users can directly use this wrapper with the XGBoost library.

Tested with Databricks Runtime for ML, versions 6.6 (Spark 2.4.5, XGBoost 0.9) and 7.1 (Spark 3.0.0, XGBoost 1.0)

See the notebook in `/examples` for a practical illustration of usage.