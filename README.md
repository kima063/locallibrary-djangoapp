Django Local Library
---------------------------------------------------------------------------------------------------------------------------
For detailed information about this project go to this link: https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Tutorial_local_library_website
--------------------------------------------------------------------------------------------------------------------------
Setting up a Django development environment
--------------------------------------------------------------------------------------------------------------------------------------

I did this using Windows. So here goes the setup for windows 10.

1. Check if you have python installed in your machine already :
command : python --version
if not download it from python's official site. Here's the link: https://www.python.org/downloads/
**make sure to check on the " Add Python ... to Path"**

2. Installing pip. If you installed python correctly it will be installed along side the python earlier. To check it existence type **pip --version** in cmd

3. Installing Django. For checking use the command: **django-admin --version**
Now, for installing django let's not disturb the entire system. Instead create a virtual environment and install django inside that environment. 

 a) Installing the virtual environment wrapper.  
 command: pip install virtualenvwrapper-win <br>
 b) Creating the environment.
 command: mkvirtualenv THENAMEYOUWANTTOGIVE
 
  N.B: for entering into the virtual environment anytime from cmd use the command :cd path_of_your_virtual_environment\Scripts\activate OR use the command: workon THENAMEYOUWANTTOGIVE
  
 c) installing django.
 command: pip install django
 for checking if it's installed or the version run **django-admin -version**
  N.B: Django is now installed in your virtual environment, not in your whole system.

Now, the virtual environment and django set up is done, and one is good to go! Cheers!

---------------------------------------------------------------------------------------------------------

Setting up the Project
------------------------------------------------------------------------------------------------------
After cloning run these command:
1. pip3 install -r requirements.txt
2. python manage.py makemigrations
3. python manage.py migrate
4. python manage.py collectstatic
5. python manage.py test # Run the standard tests. These should all pass.
6. python manage.py createsuperuser # Create a superuser
7. python manage.py runserver

After these,
Open a browser to http://127.0.0.1:8000/admin/ to open the admin site
Create a few test objects of each type.
Open tab to http://127.0.0.1:8000 to see the main site, with your new objects.

And, it's Done!