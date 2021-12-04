# Django

## what is Django?
Django is a high-level Python web framework that enables rapid development of secure and maintainable websites. developed between 2003 and 2005 by a web team who were responsible for creating and maintaining newspaper websites

**Django helps you write software that is:**
1. **Complete**

provides almost everything developers might want to do "out of the box"

2. **Versatile**

It can work with any client-side framework, and can deliver content in almost any format

3. **Secure**
4. **Scalable**

Having a clear separation between the different parts means that it can scale for increased traffic by adding hardware at any level: caching servers, database servers, or application servers

5. **Maintainable**

Django code is written using design principles and patterns that encourage the creation of maintainable and reusable code

6. **Portable**

runs on many platforms: Linux, Windows, and Mac OS X


## how to use it to create a website?

1. creating a model that is a scheme for your data by s.th like this: 


        class Band(models.Model):
            """A model of a rock band."""
            name = models.CharField(max_length=200) # indicate that the name is a group of characters 
            can_rock = models.BooleanField(default=True) # indicate that booleanfield have either true or false


2. design URLs for an application and view it by: 

        from django.urls import path

        from . import views

        urlpatterns = [
            path('bands/', views.band_listing, name='band-list'),
            path('bands/<int:band_id>/', views.band_detail, name='band-detail'),
            path('bands/search/', views.band_search, name='band-search'),
]


3. view the html code (page) by render method

        from django.shortcuts import render

        def band_listing(request):
            """A view of all bands."""
            bands = models.Band.objects.all()
            return render(request, 'bands/band_listing.html', {'bands': bands})


4. HTML template: for examlpe

        <html>
        <head>
            <title>Band Listing</title>
        </head>
        <body>
            <h1>All Bands</h1>
            <ul>
            {% for band in bands %}
            <li>
                <h2><a href="{{ band.get_absolute_url }}">{{ band.name }}</a></h2>
                {% if band.can_rock %}<p>This band can rock!</p>{% endif %}
            </li>
            {% endfor %}
            </ul>
        </body>
        </html>


***resources***

1. [what is django](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Introduction) 
2. [intro to django](https://www.djangoproject.com/start/)
