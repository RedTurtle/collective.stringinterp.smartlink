Take advantage of **redturtle.smartlink backend/frontend URLs conversion** feature, overriding
Plone URLs when sending e-mails using **content rules**.

Introduction
============

When using Plone content rules **mail action**, you can rely on some URL-like variables:

* ``${url}``
* ``${absolute_url}``
* ``${parent_url}``

This product could help your when your Plone site use different URLs for backend (http://admin.yourcompany.com/) and
front-end (http://www.yourcompany.com/).
Action taken in the backend (for example: a contributor add a new document) could trigger e-mail message where variables
above will be replaced by backend URLs.

If e-mail messages are targeted to front-end users, this can be a problem.

This product take advantage of `redturtle.smartlink`__ Plone add-on and its `backend-frontend transformation feature`__.
Before replacing URL variables, it try to apply Smart Link configuration to them.

__ http://plone.org/products/redturtle.smartlink/
__ http://plone.org/products/redturtle.smartlink/#handle-back-end-front-end-urls

Original mappings (that do not use Smart Link configuration) will be still available using new names:

* ``${original_url}``
* ``${original_absolute_url}``
* ``${original_parent_url}``

Credits
=======

Developed with the support of `Regione Emilia Romagna`__;
Regione Emilia Romagna supports the `PloneGov initiative`__.

__ http://www.regione.emilia-romagna.it/
__ http://www.plonegov.it/

Authors
=======

This product was developed by RedTurtle Technology team.

.. image:: http://www.redturtle.it/redturtle_banner.png
   :alt: RedTurtle Technology Site
   :target: http://www.redturtle.it/
