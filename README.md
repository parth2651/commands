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
