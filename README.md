# rosetta-suit

Integration of django-rosetta into django-suit admin interface.

Original author: [kunitoki](https://github.com/kunitoki)

Posted in this [issue](https://github.com/darklow/django-suit/issues/138)

## Installation

Recursively copy the folder *rosetta* into your virtualenv site-packages, that’s all.

    /bin/cp -uvr rosetta your/virtualenv/lib/python2.7/site-packages

## Usage

Item in SUIT_CONFIG:

    {'label': 'Translations', 'icon':'icon-globe', 'url': '/admin/translate/'}

Your urls.py:

    url(r'^admin/translate/', include('rosetta.urls')),
