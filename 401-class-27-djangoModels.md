## Django Models

> django web applications access and manage python object reffered to as models. models define the structure of stored data

## Local library models

>  when designing models it makes sense to have seperate models for every "object"

> you can also use models to represent things such as lists as opposed to having them hard coded into the site


## Model definition

> models are usually defined in an applications models.py file and are implemented as subclasses of `django.db.models.Model` and can include fields,methods and meta data a typical model will look something akin to the below

-`from django.db import models`

-`class ExampleName(models.Model):`
  
-`   #Fields`
  
  -`example_field_name = models.CharField(max_length=20,help_text='Enter field documentation'`
  
  -`#MetaData`

  -`class Meta:`
    
    -`ordering = ['example_field_name']`
  
  -`#Methods`
  
  -`def get_absolute_url(self):`
  
    -`return reverse('model-detail-view`,args=[str(self.id)])
  
  -`def __str__(self):`
  
    -`return self.example_field_name`

