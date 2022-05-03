# Network Forensics (Industrial Intrusion Detection Lab)
*Assumes a working jupyter environment in VSCode*

### Start Server
Unfortunately due to the fact that raw sockets need elevated privileges, we have to run the notebook-server as root.
```bash
sudo su
pip3 install jupyter #if not already accessible as root 
jupyter notebook --autoreload --allow-root --no-browser
```

### Connect VSCode 
Select the jupyter server in VScode on the lower right, when the .ipynb is focused:

> Connect Server > Remote > Existing > *Enter copied URL with token from console*

Set the appropriate kernel on the top right of the notebook: e.g. Python 3 (ipykernel - Remote)