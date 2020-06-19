# portfolio
Its awesome
1. The first step to make a website is to think how it will be going to look like
2. for creating a virtualenv enter command  
  -virtualenv <nameofvirtualenv>
3. After making a new app you should commit it into the github
4. for importing models
 - Allows us to create a new class and all things to save it in the database
 - from django.db import models
 - class Job(models.Model):
 - You can add imagefield with parameters, get it in (www.djangoproject.com) 
5. For a new app we also have to add it to the INSTALLED_APPS list in the settings.py
6. we specify MEDIA_ROOT to specify that if one wants to store some sort of image file then 
he should go here
So we can use os.path.join(BASE_DIR,'media') and you should not put media/ but only media
it is like db.sqlite3 also you can put
If someone wants to access the image where he should go is specified by MEDIA_URl
MEDIA_URL = '/media/'
7. You also have to add this media in the url patterns like this
from django.com import settings
from django.conf.urls.static import static
urlpatterns = [hare Krsna]+static(settings.MEDIA_URL,document_root=settings.MEDIA_URL)
8. Without pillow installed it may not identify the new apps
9. With apps in django the templates work much easier way 
creating job/templates/job folder and creating home.html also we will return the following 
from home function 
def home(request):
  return render(request, 'jobs/home.html')
10. Bootstrap is a framework so that our website good look
You can use documentation for the bootstrap
Go to the examples and pick the components some components if fine not have.
On the component just do the page source and copy the html code into home.html
Then startchopping.
We can also get direct access to code with CDN and very fast to load our page.
Go to home page and look for Bootstrap CDN and copy the css and html and paste the things 
Also custom styles for this template you can see
10. 
The Grid system in the documentation can help you nicely in the bootstrap
Look at the documentation of the Navbar and under the Nav section you can see the cool examples for NavBar
11. light to dark in the css
12. We can use a for loop for generating sequences going with one job or challenge
13. 
from .models import Job
jobs = Job.objects and then passing as a dictionary
return render(request, 'jobs/home.html',{'jobs':jobs
14. jobs.all allows us to loop through all the jobs
15. You can use functions and images to display the further things
16. template does not exist then you should see whether it is looking in the correct location
blog/allblogs.html

