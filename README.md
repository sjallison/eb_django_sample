# eb_django_sample
Minimal django 1.8 configuration w/ postgresql on aws elasticbeanstalk (runs on default python3.4 amazon linux)

Basically a clean `django-admin startproject django_eb` with postgresql baked in and some config to allow deployment on aws be.

Based on:
 - http://docs.aws.amazon.com/elasticbeanstalk/latest/dg/create-deploy-python-django.html
 - https://realpython.com/blog/python/deploying-a-django-app-to-aws-elastic-beanstalk/

Follow the 2nd link for help deploying to aws eb.

NOTE: my_su creates an admin account admin:admin. Make sure to change this once deployed!
