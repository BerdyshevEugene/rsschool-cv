# rsschool-cv
## Eugene Berdyshev
Python developer
____

## Contacts:
- Location: Saint Petersburg, Russia
- Email: berdyshevevg9081@gmail.com
- Phone: 8 (950) 435-14-69
- GitHub: https://github.com/BerdyshevEugene
- tg: @nezvester_eugene
____
## About Me:
I'm studying python development. In the course of learning a programming language, I have developed several projects such as:
- Youtube project. Social network for bloggers;
- telegram bot for tracking homework status;
- telegram bot translator;
- alien invasion game - a classic 2D game about spaceships;
- foodgram-project-reaction. The foodgram project is designed to create recipes and share them. Users can create their own recipes, subscribe to other authors, upload recipes and add recipes to favorites;
- job_hunter. Find Job is designed for job search. Users can subscribe to vacancies. Search for vacancies of interest, by city or specialty
____
## Skills and Proficiency:
- Python
- Django
- REST API
- SQLite
- Git
- Docker
---
## Code Examples:
```sh
from sqlite3 import Timestamp
from django.db import models

from scraping.utils import from_cyrillic_to_eng


def default_urls():
    return {'work_habr': ''}


class City(models.Model):
    name = models.CharField(max_length=50, unique=True, blank=True)
    slug = models.SlugField(max_length=50, unique=True, blank=True)

    class Meta:
        verbose_name = 'city'
        verbose_name_plural = 'cities'

    def __str__(self):
        return self.name

    def save(self, *args, **kwargs):
        if not self.slug:
            self.slug = from_cyrillic_to_eng(str(self.name))
        super().save(*args, **kwargs)
```
____
## Education
- 2022
Yandex.Practicum
Python backend developer
- 2016
Siberian Federal University, Krasnoyarsk
Law Institute, International Public and Private Law
____
## Languages:
English: upper-intermediate

Russian: native
