# This is the project for Django and React integration  

Step 1: start project for backend Using Django

``` pip install virtualenv ```

``` virtualenv venv``` or ``` python -m virtualenv venv ```

``` venv/Scripts/activate ``` for windows
``` source venv/bin/activate ``` for Linux

   ## If you get any error in activating in virtualenv
   search on google
   
   if you get  **script disabled** error 

   1. open powershell and run as administrator
   2. run this command 
   ```  Set-ExecutionPolicy -ExecutionPolicy Unrestricted ```
   it fix you issue

step 2: start project requirements

``` pip install -r requirements.txt ```

step 3: make migrations 

``` python manage.py migrate```
step 4: run server

``` python manage.py runserver.py ```


# Now Backend running successfully

# Now frontend part


1. if you want to create a new project just run this command

``` npm create vite@latest frontend -- --template react ```

or 

``` npm install ```

2. now start your frontend 

``` npm run dev ```

# Note

if you want to use sqlite3 for backend change files to 

1. manage.py line 9

this ```  os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'backend.settings.production')```

to ``` os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'backend.settings.developement')```


2. wsgi.py line 14

this ```os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'backend.settings.production')```

to ```os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'backend.settings.developement')```

3. asgi.py line 14

this ```os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'backend.settings.production')```

to ```os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'backend.settings.developement')```





