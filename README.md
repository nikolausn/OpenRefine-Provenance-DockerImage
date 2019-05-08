# OpenRefine-Provenance-DockerImage

Docker Image for OpenRefine Provenance Demo, contains Dockerfile to build image of JupyterNotebook with OpenRefine and Python2, including the OpenRefine client API and orprov-cli scripts

To start the openrefine server in the JupyterNotebook / MyBinder include this code snippet in the begining cell of you Jupyter Notebook

```
import subprocess
import time
subprocess.call("./start_refine.sh",shell=True)

#wait for 10 seconds
time.sleep(10)
```
