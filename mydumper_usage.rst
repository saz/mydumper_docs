.. _mydumper_usage:

.. image:: ../images/horizontal/color-dark.svg
  :width: 50%
  :alt: MyDumper's logo
  :class: only-dark

.. image:: ../images/horizontal/color-light.svg
  :width: 50%
  :alt: MyDumper's logo
  :class: only-light

mydumper Usage
==============

Synopsis
--------

:program:`mydumper` [:ref:`OPTIONS <mydumper-options-label>`]

Description
-----------

:program:`mydumper` is a tool used for backing up MySQL database servers much
faster than the mysqldump tool distributed with MySQL.  It also has the
capability to retrieve the binary logs from the remote server at the same time
as the dump itself.  The advantages of mydumper are:

  * Parallelism (hence, speed) and performance (avoids expensive character set conversion routines, efficient code overall)
  * Easier to manage output (separate files for tables, dump metadata, etc, easy to view/parse data)
  * Consistency - maintains snapshot across all threads, provides accurate master and slave log positions, etc
  * Manageability - supports PCRE for specifying database and tables inclusions and exclusions

.. _mydumper-options-label:

Options
-------

The :program:`mydumper` tool has several available options:

.. program:: mydumper

.. include:: mydumper_usage_autogenerated.rst
