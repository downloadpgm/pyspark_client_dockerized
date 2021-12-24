# pyspark_client_dockerized
pyspark_client_dockerized

Run jupyter notebook --generate-config
```shell
$jupyter notebook --generate-config
```

Edit /root/.jupyter/jupyter_notebook_config.py
```shell
$ vi /root/.jupyter/jupyter_notebook_config.py
c.NotebookApp.ip = '*'
c.NotebookApp.open_browser = False
c.NotebookApp.port = 8888
```

$ jupyter notebook password
```shell
Enter password:  ****
Verify password: ****
```

Run pyspark
```shell
PYSPARK_DRIVER_PYTHON_OPTS="notebook --no-browser --allow-root --port=8082" pyspark &
```