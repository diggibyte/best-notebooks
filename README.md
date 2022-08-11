# demo-workspace
This is the refrence workspace for WoW  

- notebooks:   
consist notebook for in dir structure <layer/area> / <source>  
- pmodule:  
used to store python module code relent to your code it should have common code udfs and other businiss logic.
- tests:   
Consist unit test module for pmodule and notebooks  
- requerments.txt:   
python module dependency 


[<img src="https://github.com/diggibyte/best-notebooks/blob/main/img/dir_structure.png" width="250"/>](image.png)





#Setting up dbconnect to connect with databricks 


-Create Virtual env 
install python veriosn 
```
python3.8 -m pip install pipenv
```
Install Pipenv:

Class variable required to databricks connect 
````
export DATABRICKS_ADDRESS=“https://adb-XXXXXXXXX.azuredatabricks.net”
export DATABRICKS_API_TOKEN=“dXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX”
export DATABRICKS_CLUSTER_ID=“XXXXXXXXXXXXXXXXXX”
export DATABRICKS_ORG_ID=“XXXXXXXXX”
export DATABRICKS_PORT=15001

export PYSPARK_PYTHON =
export PYSPARK_DRIVER_PYTHON =
````



```
python3.8 -m pip install pipenv
python3.8 -m venv dbconnect
source dbconnect/bin/activate
pip3 install -U "databricks-connect==10.4.*"
databricks-connect test
```



