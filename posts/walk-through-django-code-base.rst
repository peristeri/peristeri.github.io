.. title: Walk through the Django code base
.. slug: walk-through-django-code
.. date: 2018-11-20
.. tags: code reading, python, django
.. category: walk-through
.. description: A walk through of the Django code base.
.. status: draft

==========================================
A walk through the Django code base
==========================================

In my previous article, I wrote about reading code and it is best I demonstrated
some of the techniques I use to understand the code. This is not a critique of
the code or how to improve it, this is an exercise of developing a mental model
of part of the code base.

    The version of `Django Project <https://www.djangoproject.org>`_ for this
    exercise is **2.0.0**


I get myself a pad and pencil and write at the top of the page: **How does
middle-ware component work?** and use this to take notes. Once I'm ready, I turn
my attention to the directory names. The names are a good base line on how
things are organized and what artifacts the project generates.
