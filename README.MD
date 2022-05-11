# Network Forensics (Industrial Intrusion Detection Lab)
*Assumes a working jupyter environment in VSCode*

### Start Server
Unfortunately due to the fact that raw sockets need elevated privileges, we have to run the notebook-server as root.
```bash
sudo su
pip3 install jupyter #if not already accessible as root 
jupyter notebook --autoreload --allow-root --no-browser
```
This will start a server and expose a token-URL. For example:
 `http://localhost:8889/?token=3c441bd52cc1b2875b1c454a7f400ab33336aff9edd62fc4`
 Copy this for the next step...

### Connect VSCode 
Select the jupyter server in VScode on the lower right, when showcase.ipynb is open and focused:

> Connect Server > Remote > Existing > *Paste token-URL*

Set the appropriate kernel on the top right of the notebook: e.g. Python 3 (ipykernel - Remote). Make sure its the *Remote* kernel, so you actually have root access.