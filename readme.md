django-cache-middleware
=========================

django-cache-middleware is a Django app for the caching api data while get method and removing after data altered or created.

Installation
------------

    * pip install django-cache-middleware
    * Add ``cache_middleware`` to your ``INSTALLED_APPS``
    * Add ``cache_middleware.middlewares.CacheMiddleware`` to your ``MIDDLEWARE``
    * set django redis for your project (https://pypi.org/project/django-redis/) 

::

Setup in settings
-----------------

    * REMOVE_RELATED_CACHE : bool # default True # remove related model data i.e o2m, m2o, m2m, 020 dat 
    * CACHE_REMOVE_TIMEOUT : integer | None # default None # cache removing time
    * BASE_API_URL : str # default /api/ # base api url
    * CACHE_NAME : str # default settings.ROOT_URLCONF.split('.')[0] #  name of cache base key name

::


Compatibility
-------------
{py37, py38, py310}-django{4.* above}
