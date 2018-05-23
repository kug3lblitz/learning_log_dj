_______-----------------------
web app which will allow users to create topics and create log entries 
on that topic. The homepage should describe this function, and allow
users to register/sign in. Once logged in, users should be able to
create new topics, add new entries, and read/edit existing entries.
__-----------------------

django shell debugging

python manage.py shell - opens interactive repl shell in directory/env

ex:
>>> from learning__logs.models import Topic
>>> Topic.objects.all()
[<Topic:>, <Topic:>]

>>> topics = Topic.objects.all()
>>> for topic in topics:
>>>     print(topic.id, topic)

>>> t = Topic.objects.get(id=1)
>>> t.text
'returns "text"'
>>> t.date_added
'returns "text"'

>>> t.entry_set.all()
'returns "text"'
