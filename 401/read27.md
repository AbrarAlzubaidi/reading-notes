# Models in django

 Models define the structure of stored data, including the field types and possibly also their maximum size, default values, selection list options, help text for documentation, label text for forms, etc. 

 ## Fields

 A model can have an arbitrary number of fields, of any type — each one represents a column of data that we want to store in one of our database tables. Each database record (row) will consist of one of each field value.

ex: 

    my_field_name = models.CharField(max_length=20, help_text='Enter field documentation')

## Common field arguments
1. help_text
2. verbose_name
3. default
4. null
5. blank
6. choices
7. primary_key: represent the table and it is a unique not repeated data (with it you can classify data)

## Common field types
1. CharField
2. TextField
3. IntegerField
4. DateField
5. EmailField
6. FileField and ImageField
7. AutoField is a special type of IntegerField that automatically increments. 
8. ForeignKey: to make relation between tables (for one-to-many relationship)
![One2Many](https://miro.medium.com/max/533/1*he69DGDktscuNpBGVnjrpg.png)
9. ManyToManyField: to make relation between tables (for many-to-many relationship)
![Many2Many](https://www.codechit.com/wp-content/uploads/2020/06/ManyToOneRelationship.png)


----


# Django Admin

- Django admin application can use your models to automatically build a site area that you can use to create, view, update, and delete records
- The admin application can also be useful for managing data in production, depending on the type of website

## Registering models
1. open `admin.py`
2. regester model by `admin.site.register(model_name)`
3. to create a super admin/user type `python manage.py createsuperuser` in terminal
   - it will appear some question about the name of the super user, email, password and confirm password
   
4. To login to the site, open the /admin URL (e.g. http://127.0.0.1:8000/admin) 

5. you can display your wanted field by using 
```
class BookAdmin(admin.ModelAdmin):
    list_display = ('title', 'author', 'display_genre') 
```
