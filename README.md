# eb_django_sample
Minimal django 1.8 configuration w/ postgresql on aws elastic beanstalk (runs on the default python 3.4)

Basically a clean `django-admin startproject` with postgresql baked in and some configuration for aws eb deployment.

Based on:
 - http://docs.aws.amazon.com/elasticbeanstalk/latest/dg/create-deploy-python-django.html
 - https://realpython.com/blog/python/deploying-a-django-app-to-aws-elastic-beanstalk/

No extra configuration required (at least as of the date of this commit):
 - Clone this repo
 - Set up an IAM user and get aws credentials
 - `eb init`
 - `eb create`

`eb create` will exit with error because no DB is configured. Go to your aws console and create a postgresql db in your environment. Once your environment completes the automatic update, you're up and running.

Follow the 2nd link above if you need help deploying to aws eb. Read both links to understand the specifics of running django on aws eb.

**NOTE**: my_su creates an admin account admin:admin. Make sure to change it as soon as you deploy!
