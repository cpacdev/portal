# AA-DR Portal

A simple portal that allows vendors to sign up to apply, view application progress and status, as well as providing a central location for documents.

### **Local Setup**

---

To begin simply pull this repository and its submodules using the following command:

`git clone --recurse-submodules https://github.com/cpacdev/portal.git`

...or if you setup SSH already:

`git clone --recurse-submodules git@github.com:cpacdev/portal.git`

### **Running Locally With Docker**

---

_This method will build both front-end and back-end at once with minimal local installation!_

1. Make sure to install Docker for your system first!

2. After doing so simply run `docker compose up -d --build`

3. To shutdown both the front-end and backend run `docker compose down`

**You will now see the frontend on `localhost:3000` and the backend on `localhost:3001`**

### **Running VSCode Devcontainers**

---

Requirements:

- VSCode
- Docker
- VSCode Dev Containers plugin

**Running the backend**

1. In vscode click `File` and then click `Open Folder...`
2. Open the `backend` folder
3. Click `Ctrl + Shift + P` and then select `Dev Containers: Rebuild and Reopen in Container`
4. See steps **Running the backend** in **Running Locally without Docker** below to see how to start the backend

**Running the frontend**

1. In vscode click `File` and then click `Open Folder...`
2. Open the `frontend` folder
3. Click `Ctrl + Shift + P` and then select `Dev Containers: Rebuild and Reopen in Container`
4. See steps **Running the frontend** in **Running Locally without Docker** below to see how to start the frontend

### **Running Locally without Docker**

---

Make sure to have the following installed before proceeding:

- Node.js
- Yarn package manager
- Python 3.10+

**Running the backend**

1. `cd backend`
2. `pip install -r requirements.txt`
3. `python app.py`

**Running the frontend**

1. `cd frontend`
2. `yarn`
3. `yarn run dev`

### **Pushing your changes**

---

`git push --recurse-submodules=on-demand`
