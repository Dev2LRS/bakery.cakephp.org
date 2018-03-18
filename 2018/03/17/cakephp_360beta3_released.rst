CakePHP 3.6.0-beta3 Released
============================

The CakePHP core team is happy to announce the immediate availability of CakePHP
3.6.0-beta3. This is the first beta release for 3.6.0, and it contains several
new major features.

Updating to the beta
--------------------

You can use composer to upgrade to the beta version of CakePHP 3.6.0::

    php composer.phar require --update-with-dependencies "cakephp/cakephp:3.6.0-beta3"

We would greatly appreciate it if you temporarily upgraded your application,
and ran your tests. By opening issues for any regressions in the beta, we can
help ensure a smoother release of 3.6.0 before the stable release.

What's new in 3.6.0?
--------------------

The `migration guide
<https://book.cakephp.org/3.next/en/appendices/3-6-migration-guide.html>`_ has
a complete list of what's new in 3.6.0, and what has been deprecated. We
recommend you give that page a read when upgrading.

Changes Since 3.6.0-beta2
-------------------------

* Added ``Query::whereInList()`` and ``Query::whereNotInList()`` to enable more
  explict ``IN`` condition creation.
* ``TranslateBehavior::locale()`` was deprecated and replaced by ``setLocale()``
  and ``getLocale()``.
* ``Query::getContain()`` was added and the get mode of ``contain()`` was
  deprecated.
* Fix recursive plugin bootstrapping.
* Fix ``Plugin::load()`` not including bootstrap files in testsuite setup.


Contributors to 3.6.0-beta3
---------------------------

Thank you to all the contributors that helped make this release happen:

* Mark Scherer
* Mark Story
* chinpei215
* ndm2
* saeideng

As always, we would like to thank all the contributors that opened issues,
created pull requests or updated the documentation.

.. author:: markstory
.. categories:: release, news
.. tags:: release, news
