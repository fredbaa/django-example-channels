Based on the tutorial from this link: https://testdriven.io/blog/django-channels/

Requirements: Python 3.6

How to run:
```
python3.6 -m venv env
source env/bin/activate
pip install -r requirements.txt

# run redis here if you have, configured at 127.0.0.1:6379

python manage.py migrate
python manage.py runserver

# since we implemented authentication, only logged in users can chat. create an admin user
python manage.py createsuperuser

# and proceed to /admin to create more users. make sure to add them as staff
```

How to chat:
1. Navigate to http://localhost:8000/admin to login
2. Once logged in, navigate to http://localhost:8000/chat to start chatting
3. You can open incognito windows / other browsers to login other users
4. Chat away!