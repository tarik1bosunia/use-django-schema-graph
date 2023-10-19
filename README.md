## use of [django-schema-graph](https://github.com/meshy/django-schema-graph/tree/master#django-schema-graph) package



```bash
pip install django-schema-graph
```

### Add to INSTALLED_APPS:
```python
INSTALLED_APPS = [
    ...
    'schema_graph',
    ...
]
```

### urls.py
```python
from django.contrib import admin
from django.urls import path
from schema_graph.views import Schema

urlpatterns = [
    path('admin/', admin.site.urls),
    path("schema/", Schema.as_view()),
]
```

![schema image]("readme%20images/1.png" schema)
![Schema Default Django](./readme%20images/1.png "Schema Default Django")