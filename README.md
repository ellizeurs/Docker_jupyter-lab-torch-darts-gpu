# JupyterLab Container
Repository created to host the JupyterLab Dockerfile
Contains
- JupyterLab on port 10101
- Darts
- Optuna
- RayTune
- PySwarm
- Other dependencies
---
###### Usage
The container is hosted on DockerHub and can be used with the command:
- Docker
``` bash
$ docker pull ellizeurs/jupyter-lab-torch-darts-gpu:latest
$ docker run -d --gpus all -p 10101:10101 ellizeurs/jupyter-lab-torch-darts-gpu:latest
```
- Singularity
``` bash
$ singularity pull docker://ellizeurs/jupyter-lab-torch-darts-gpu:latest
$ singularity run --nv jupyter-lab-torch-darts-gpu_latest.sif
```