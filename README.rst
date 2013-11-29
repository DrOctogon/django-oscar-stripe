===================================
Stripe integration for django-oscar
===================================

*This repo just supports Stripe Checkout at the moment. Although it should work with Stripe.js equally well,
it has only been used with Checkout so far. It isn't complete yet.*

This package provides integration between Stripe_ and Oscar_.  It is currently a
work-in-progress - contributions are welcome.  Any questions, please use the Oscar mailing list: `django-oscar@googlegroups.com`_

.. _Stripe: https://stripe.com
.. _Oscar: http://oscarcommerce.com
.. _`django-oscar@googlegroups.com`: https://groups.google.com/forum/?fromgroups#!forum/django-oscar

Useful information:

* `Stripe's Python API`_

.. _`Stripe's Python API`: https://stripe.com/docs/libraries

Contributing
============

Clone the repo, create a virtualenv and run::

    make install

to install all dependencies.  Run the tests with::

    ./runtests.py

There is a sandbox site that you can browse and use to test the Stripe
integration.  Create is using::

    make sandbox

and browse it after::

    cd sandbox
    ./manage.py runserver

TODO
====

* Create a "Stripe transaction" model that tracks each request/response to
  Stripe's servers
