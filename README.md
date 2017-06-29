#Deploy EC2

##requirements

**Python**
3.6.1

**pip**

```
pip install -r requirements.txt
```

##create secret config file

###Projcet structure
```
project_foloder/
	.conf_secret/
		settings_common.json
		settings_debut.json
		settings_deploy.json
	.django_app/
	...
	...
```

###settings_common.json example
```
{
  "django":{
    "secret_key":"django projcet secret key"
  }
}
```

###settings_debug.json example
```
{
  "django":{
    "allowed_hosts": [
      "*"
    ]
  }
}
```

###settings_deploy.json example
```
{
  "django":{
    "allowed_hosts": [
      "*"
    ]
  }
}
```
###runserver
```
# local developement
python3 manage.py runserver --settings=config.settings.debug
```
