# Navigation with Terminal

```bash
django_blog/
│
├── manage.py                  # Django's project command-line utility
│
├── django_blog/                # Global configuration folder (Project Core)
│   ├── __init__.py
│   ├── settings.py            # Global project settings (database, apps, middleware)
│   ├── urls.py                # Main URL routing routing to your apps
│   ├── asgi.py                # Deployment entry point for async servers
│   └── wsgi.py                # Deployment entry point for standard servers
```

Above is the tree structure of our django_blog and below is the breakdown of the structure:

- __django_blog__ is the folder (or directory) which is also the parent, in other word, the root of all other folders and files
- __manage.py__ is a file inside __django_blog__
- __django_blog__, the folder right after __manage.py__ file is also a directory inside the parent __django_blog__. It contains:
  - \__init__.py, settings.py, urls.py, asgi.py, and wgsi.py files

### 1. Navigation

To navigate, we use __cd__ command. c = change, d = directory
In plain statement, we are changing the current working directory to another one

#### Syntax

```bash
cd to_directory

# Examples

# Before navigation, we have
C:/Users/Documents>
# This tells us that `Documents` is our current working directory

# navigate to the parent folder i.e. django_blog
C:/Users/Documents> cd django_blog
# becomes C:/Users/Documents/django_blog> when you press 'Enter' key



# navigate to django_blog folder inside django_blog
C:/Users/Documents> cd django_blog/django_blog
# becomes C:/Users/Documents/django_blog/django_blog> when you press 'Enter' key

# navigate back to the first django_blog
C:/Users/Documents/django_blog/django_blog> cd .. # goes one step behind
# becomes C:/Users/Documents/django_blog> when you press 'Enter' key


# navigate back to Documents
C:/Users/Documents/django_blog/django_blog> cd ../.. # goes two steps behind
# becomes C:/Users/Documents> when you press 'Enter' key
```

### 2. List files and/or folders

Use __ls__ to see what is/are within:

1. The directory you navigated to or you want to navigate to
2. The directory you are about to navigate to
3. The directory you just want to know what is/are within it

```bash
# Examples

# Display files/folders within Documents
C:/Users/Documents> ls

# Outputs:
django_blog
# and others files and folders within Documents

# Display files/folders within django_blog
C:/Users/Documents> ls django_blog

# outputs
manage.py
django_blog

# Display files/folders within django_blog/django_blog
C:/Users/Documents> ls django_blog/django_blog

# Outputs
__init__.py
settings.py
urls.py
asgi.py
wsgi.py
```
