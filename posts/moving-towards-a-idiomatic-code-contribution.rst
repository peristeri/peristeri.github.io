.. title: Moving towards an idiomatic code contribution
.. slug: moving-towards-an-idiomatic-code-contribution
.. date: 2018-11-20
.. tags: collaboration, process,
.. category: how-to
.. description: A guide to how to begin contributing to a software project.
.. status: featured
.. header-image: https://farm1.staticflickr.com/138/352972944_4f9d568680.jpg
.. status: draft

This article was inspired by my experience working on `OpenStack
<https://www.openstack.org>`_ and then later as project owner of `Spinal cord
toolbox <https://github.com/neuropoly/spinalcordtoolbox>`_. I realized that a
contributor need to some research before coding anything that is not trivial.
Like any form of research, communicating your intent is the fundamental to get
your work recognized.

As a developer being paid to work on an open source project, the business
obligation sometime blinded me that not everyone saw the intent of my
contribution. Later, I had the responsibility of managing an open source project
where some of the core contributions are from people with little or no
experience in software development. I became quickly aware of how complicated it
was to contribute, and in most cases, causes communication breakdown.

Why does this matter? Some promote a `incremental
<https://blog.newrelic.com/engineering/open-source_gettingstarted/>`_
`contributions approach <https://opensource.guide/how-to-contribute/>`_. I don't
disagree with this approach, it works to get new developers familiar with the
project. But you don't see the big picture, how the control and data flows
across the application. This article is a complement to their advice and hope it
helps structure a game plan when approaching a complex development problem.

I will be the first to admit to jumping into a project and quickly put together
a pull request to solve a problem I needed to solve, and payed for it. I annoyed
the project maintainer, became frustrated and finally abandoned my pull request.
And later as a maintainer, sometimes a pull request was dumped on my lap with no
context and my supervisor stressed how important this contribution was. The
worst case scenario was to rewrite the pull request, and not to mention the
grief of reverse engineering the code.

This is part 1 of 3 articles exploring the soft skills that can improve the
quality of the contribution, no matter what type of project you are working on.

.. TEASER_END

Part 1. Understanding the project's control flow
================================================

The goal is to get into the mind of the development team. Some projects are
straight forward, while others require context and deep domain knowledge. The
goal here is to have a good understanding of:

#. What is the problem this project solving? What is the objective of this
   project?
#. What is the project's architecture? How does it go about implementing the
   solution?
#. What are the dependencies? What projects depend on this project?
#. Identify the limitations and potential improvements of the project.

Read the docs
=============

.. image:: https://imgs.xkcd.com/comics/rtfm.png
   :align: center

This one is a given, yet so many of us bypass this. In a `paper on software
maintenance <https://dblp.org/rec/journals/jss/ChenH09>`_, documentation is
among the key requirements to achieve good understanding of the project. Here
are some of the strategies to get a good overview on how the program does.

1. What is this application trying to solve?
--------------------------------------------

Start with the easiest question. The larger applications are solving a
collection of problems. The answer will provide you with the right mind frame
to understand the project. For example, the  `Django Project's
<https://djangoproject.org>`_ problem statement is:

2. How does it solve that problem?
----------------------------------

With the problem statement identified, the solution

Take notes of what you learn so far and what might interest you. Also, build a
glossary of the terms most emphasized in the documentation, chances are those
terms will reappear in the code.

What makes a high quality documentation is outside the scope of this article.
One form of documentation I found easy to read are those that address a specific
audience. For example: "User Manual", "Developer Manual" and "Administration
Manual". For large projects, this method centralizes the information needed to
accomplish a task and thus lowers the learning curve.

Read the code
=============

.. image:: https://imgs.xkcd.com/comics/future_self.png
   :align: center

There's an entire research field in software engineering dedicated to code
comprehension. Factors such as programming experience, familiarity of the
language and domain knowledge will help gauge how long you it takes you to build
a representative mental model of the project's code. There's a paper researching
the `cognitive models <http://dx.doi.org/10.1109/2.402076>`_ commonly used to
generate these mental models. What is interesting is =======

I recommend a fully-featured IDE. Being able to navigate around the project's
code is crucial. I will posting a article on how I go about reading code soon.

I realized how a project following a coding style helps in reading the code.

Read the rest
=============

.. image:: https://imgs.xkcd.com/comics/new_bug.png
   :align: center

There's no project that doesn't have pain points. If the project is in active
development, then there must be a system to track the list of issues the project
has. In most cases, project owners use an issue tracker such as `Jira
<https://www.atlassian.com/software/jira>`_ and `Github <https://github.com>`_.
The completed and open issues can tell you a lot about the state and quality of
the code.


Conclusion
==========

Learning to understanding is program's work flow is a fundamental skill in your
arsenal of project comprehension.

to make
your contribution to a software project. Once you have a

With the right approach, a developer's
time and energy is used optimally.

Happy reading!
