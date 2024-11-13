



Django 3 Social Network | Social media

1. Create project Socialgram - django-admin startproject Socialgram
2. Change directory (cd Socialgram)and create app core - django-admin startapp core
3. Add core in installed app section of settings.py
4. Install crispy form and add in installed app of settings.py
5. Set path of static files
6. Set path of templates files
7. Set database
8. Make migrations
    - python manage.py makemigrations
    - python manage.py migrate
9. Run Django server
    - python manage.py runserver

install all the dependencies before run the project and enjoy.....

pip install crispy-bootstrap4==2024.10
pip install django-bootstrap-datepicker==1.5.0
pip install django-debug-toolbar==4.4.2
pip install django-unused-media==0.2.2
pip install mysql-connector-python==8.4.0
pip install mysqlclient==2.2.4
pip install opencv-python==4.10.0.82
pip install pillow==10.3.0
pip install pipdeptree==2.23.4
pip install pipreqs==0.5.0
pip install pydantic==2.7.2
pip install pydub==0.25.1
pip install scipy==1.13.0


CREATING A FOLLOWER AND FOLLOWING VIA DJANGO SHELL.

1. Launch Django shell - python manage.py shell
2. Import model User - from django.contrib.auth.models import User
3. Import model Follower - from core.models import Follower
4. Import model Following - from core.models import Following

Himanshu following Aman

Himanshu is a follower and Aman is following
disciple = 'Himanshu' and leader = 'Aman'


follower = Follower()
leader = User.objects.get(username='Aman')
disciple = User.objects.get(username='Himanshu')

following = Following()
leader.follower_set.create(follower_user=disciple)
disciple.following_set.create(following_user=leader)



CREATING A POST VIA TERMINAL
import model Post - from core.models import Post
a = Post(user_id=3, post_text='Hi Socialgram')
a.save()





   
