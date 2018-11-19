.. title: Moving towards an idiomatic open source contribution
.. slug: moving-towards-an-idiomatic-open-source-contribution
.. date: 2018-01-26
.. tags: open source, introduction, draft
.. category: Guide
.. description: A guide to how to begin contributing to open source.
.. type: text
.. status: draft


==================================
Open source development work-flow
==================================

Most aspiring developers, the enthusiasm of contributing sometime blinds them to
the size and complexity of the task.

I had the responsibility of managing an open source project, and became quickly
aware of the common oversights and how following a work-flow can help
communicate your intent. I find this to be more important then the killer
feature I don't understand what it is suppose to do.

Step 1. Explore the project
===========================

I will be the first to admit to jumping into a project without reading the docs
or the code. And payed for it, by annoying the project maintainer and
frustrating myself.

Code comprehension strategies
-----------------------------

There's part of software engineering dedicated to improving the techniques for
code comprehension. Research points to alternate between depth


Step 2. Setup your development environment
==========================================

I will bypass the basic definition of the fundamentals of version control. If
you need a refresher I suggest `Git Pro <https://git-scm.com/book/en/v2>`_.

You can find most of the open source projects on `GitHub <https://github.com/>`_.

Fork the project
----------------

.. code:: sh

   git clone https://github.com/peristeri/spinalcordtoolbox.git
   git remote add sct https://github.com/neuropoly/spinalcordtoolbox.git
   git fetch sct

   # The most important part
   git branch sct-master --track sct/master
   git checkout sct-master

   git checkout -b new-feature


.. code:: python

   def test_denoise():
       assert 1 + 1 = 2
