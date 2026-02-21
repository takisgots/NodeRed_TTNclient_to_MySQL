🧰 1. Install Node.js and Node‑RED

Install Node.js (LTS version recommended)
Download from: https://nodejs.org

Install Node‑RED

Open a terminal (PowerShell or Git Bash):

Code:

npm install -g --unsafe-perm node-red
(This gives you a fresh Node‑RED installation.)


📥 2. Clone your GitHub repository

Choose where you want your Node‑RED user directory to live.

Most people use:

Code:

C:\Users\YourUser\.node-red
(If that folder already exists, rename or delete it.)

Then clone your repo into that location:

Code:

cd C:\Users\<YourUser>

git clone https://github.com/<yourname>/<repo>.git .node-red

Now your .node-red folder contains your flows and package.json.


📦 3. Install all Node‑RED dependencies

Inside the .node-red folder:

Code:

cd C:\Users\<YourUser>\.node-red

npm install

(This installs all the nodes listed in your package.json.)

This step is crucial — it recreates your environment exactly as before.


🔐 4. (Optional) Restore credentials

If you included your flows_<hostname>_cred.json in GitHub, Node‑RED will load it automatically.

If you did not include it, you’ll need to re-enter credentials manually in the editor (MQTT passwords, API keys, etc.).

