# Sample commands

### Create a python virtual environment and initialize it - MAC
```
python3 -m venv .venv
source .venv/bin/activate
```

### Install the necessary libraries
```
pip install -r requirements.txt
```


### Create a python virtual environment and initialize it - windows 

```
python -m venv .venv
<environment_name>\Scripts\activate.ps1

# if error .\.venv\Scripts\activate.ps1 : File D:\Parth\quant\multichart\.venv\Scripts\Activate.ps1 cannot be loaded because     
running scripts is disabled on this system. For more information, see about_Execution_Policies at 
https:/go.microsoft.com/fwlink/?LinkID=135170.

#use this command
Set-ExecutionPolicy Unrestricted -Scope Process
.\.venv\Scripts\activate.ps1
```


Add local python project to Github

1. Initialize Git in your project (if not already done)
```
cd your-project-directory
git init
```
2. Create a .gitignore file
```
# Python
__pycache__/
*.py[cod]
*$py.class
*.so
.Python
env/
venv/
.venv/
pip-log.txt
pip-delete-this-directory.txt
.idea/
.vscode/settings.json
*.egg-info/
dist/
build/
```

3. Stage and commit your files

```
git add .
git commit -m "Initial commit"
```

4. Create a repository on GitHub
* Go to GitHub.com and sign in
* Click the "+" icon → "New repository"
* Name your repository
* Don't initialize with README, .gitignore, or license (since you already have files)
* Click "Create repository"
  
5. Connect your local repo to GitHub
```
git remote add origin https://github.com/yourusername/your-repo-name.git
git branch -M main
git push -u origin main
```

6. if authentication failed
7.Solution 1: Use Personal Access Token (Recommended)
* Step 1: Create a Personal Access Token
  Go to GitHub.com → Settings (click your profile picture)
  Scroll down to "Developer settings" → "Personal access tokens" → "Tokens (classic)"
  Click "Generate new token" → "Generate new token (classic)"
  Give it a name (e.g., "VSCode Project")
  Select scopes: check "repo" (full repository access)
  Click "Generate token"
  Copy the token immediately (you won't see it again)
* Step 2: Use the token instead of password
  When you run the push command, use:
  Username: your GitHub username
  Password: paste the personal access token (not your actual password)
```
git push -u origin main
```
