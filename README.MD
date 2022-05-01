# Network Forensics (Industrial Intrusion Detection Lab)
*Assumes a working jupyter environment in VSCode*

### Start Server
Unfortunately due to the fact that raw sockets need elevated privileges, we have to run the notebook-server as root.
```
sudo su
jupyter notebook --autoreload --allow-root --no-browser
```

### Connect VSCode 
When the Notebook is opened, select the jupyter server on the lower right:

> Connect Server > Remote > *Enter copied URL with token from console*

Set the appropriate kernel on the top right of the notebook: e.g. Python 3 (ipykernel - Remote)