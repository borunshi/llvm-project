About
========

.. warning::

   If you are using a released version of LLVM, see `the download page
   <http://llvm.org/releases/>`_ to find your documentation.

The LLVM compiler infrastructure supports a wide range of projects, from
industrial strength compilers to specialized JIT applications to small
research projects.

Similarly, documentation is broken down into several high-level groupings
targeted at different audiences:

LLVM Design & Overview
======================

Several introductory papers and presentations.

.. toctree::
   :hidden:

   Lexicon
   FAQ

`Introduction to the LLVM Compiler`__
  Presentation providing a users introduction to LLVM.

  .. __: http://llvm.org/pubs/2008-10-04-ACAT-LLVM-Intro.html

`Intro to LLVM`__
  Book chapter providing a compiler hacker's introduction to LLVM.

  .. __: http://www.aosabook.org/en/llvm.html


`LLVM: A Compilation Framework for Lifelong Program Analysis & Transformation`__
  Design overview.

  .. __: http://llvm.org/pubs/2004-01-30-CGO-LLVM.html

`LLVM: An Infrastructure for Multi-Stage Optimization`__
  More details (quite old now).

  .. __: http://llvm.org/pubs/2002-12-LattnerMSThesis.html

`Publications mentioning LLVM <http://llvm.org/pubs>`_
   ..

:doc:`Lexicon`
   Definition of acronyms, terms and concepts used in LLVM.

:doc:`FAQ`
   A list of common questions and problems and their solutions.

Documentation
=============

Getting Started, How-tos, Developer Guides, and Tutorials.

.. toctree::
   :hidden:

   UserGuides
   ProgrammingDocumentation
   SubsystemDocumentation

:doc:`UserGuides`
  For those new to the LLVM system.

:doc:`ProgrammingDocumentation`
  For developers of applications which use LLVM as a library.

:doc:`SubsystemDocumentation`
  For API clients and LLVM developers.

Getting Started/Tutorials
-------------------------

.. toctree::
   :hidden:

   GettingStarted
   tutorial/index
   GettingStartedVS

:doc:`GettingStarted`
   Discusses how to get up and running quickly with the LLVM infrastructure.
   Everything from unpacking and compilation of the distribution to execution
   of some tools.

:doc:`tutorial/index`
   Tutorials about using LLVM. Includes a tutorial about making a custom
   language with LLVM.

:doc:`GettingStartedVS`
   An addendum to the main Getting Started guide for those using Visual Studio
   on Windows.

Reference
---------

.. toctree::
   :hidden:

LLVM and API reference documentation.

.. toctree::
   :hidden:

   LangRef
   CommandGuide/index
   TestingGuide
   CompilerWriterInfo
   MIRLangRef

:doc:`LLVM Language Reference Manual <LangRef>`
  Defines the LLVM intermediate representation and the assembly form of the
  different nodes.

:doc:`LLVM Command Guide <CommandGuide/index>`
   A reference manual for the LLVM command line utilities ("man" pages for LLVM
   tools).

:doc:`LLVM Testing Infrastructure Guide <TestingGuide>`
   A reference manual for using the LLVM testing infrastructure.

:doc:`CompilerWriterInfo`
  A list of helpful links for compiler writers.

:doc:`Machine IR (MIR) Format Reference Manual <MIRLangRef>`
   A reference manual for the MIR serialization format, which is used to test
   LLVM's code generation passes.

`Doxygen generated documentation <http://llvm.org/doxygen/>`_
  (`classes <http://llvm.org/doxygen/inherits.html>`_)

`Documentation for Go bindings <http://godoc.org/llvm.org/llvm/bindings/go/llvm>`_

`Github Source Repository Browser <http://github.com/llvm/llvm-project//>`_
   ..

Community
=========

LLVM has a thriving community of friendly and helpful developers.
The two primary communication mechanisms in the LLVM community are mailing
lists and IRC.

Getting Involved
----------------

LLVM welcomes contributions of all kinds. To get started, please review the following topics:

.. toctree::
   :hidden:

   Contributing
   DeveloperPolicy
   SphinxQuickstartTemplate
   Phabricator
   HowToSubmitABug
   BugLifeCycle
   CodingStandards

:doc:`Contributing`
   An overview on how to contribute to LLVM.

:doc:`DeveloperPolicy`
   The LLVM project's policy towards developers and their contributions.

:doc:`SphinxQuickstartTemplate`
  A template + tutorial for writing new Sphinx documentation. It is meant
  to be read in source form.

:doc:`Phabricator`
   Describes how to use the Phabricator code review tool hosted on
   http://reviews.llvm.org/ and its command line interface, Arcanist.

:doc:`HowToSubmitABug`
   Instructions for properly submitting information about any bugs you run into
   in the LLVM system.

:doc:`BugLifeCycle`
   Describes how bugs are reported, triaged and closed.

:doc:`CodingStandards`
  Details the LLVM coding standards and provides useful information on writing
  efficient C++ code.

Development Process
-------------------

Information about LLVM's development process.

.. toctree::
   :hidden:

   Projects
   LLVMBuild
   HowToReleaseLLVM
   Packaging
   ReleaseProcess
   HowToAddABuilder
   ReleaseNotes

:doc:`Projects`
  How-to guide and templates for new projects that *use* the LLVM
  infrastructure.  The templates (directory organization, Makefiles, and test
  tree) allow the project code to be located outside (or inside) the ``llvm/``
  tree, while using LLVM header files and libraries.

:doc:`LLVMBuild`
  Describes the LLVMBuild organization and files used by LLVM to specify
  component descriptions.

:doc:`HowToReleaseLLVM`
  This is a guide to preparing LLVM releases. Most developers can ignore it.

:doc:`ReleaseProcess`
  This is a guide to validate a new release, during the release process. Most developers can ignore it.

:doc:`HowToAddABuilder`
   Instructions for adding new builder to LLVM buildbot master.

:doc:`Packaging`
   Advice on packaging LLVM into a distribution.

:doc:`Release notes for the current release <ReleaseNotes>`
   This describes new features, known bugs, and other limitations.

Mailing Lists
-------------

If you can't find what you need in these docs, try consulting the mailing
lists.

`Developer's List (llvm-dev)`__
  This list is for people who want to be included in technical discussions of
  LLVM. People post to this list when they have questions about writing code
  for or using the LLVM tools. It is relatively low volume.

  .. __: http://lists.llvm.org/mailman/listinfo/llvm-dev

`Commits Archive (llvm-commits)`__
  This list contains all commit messages that are made when LLVM developers
  commit code changes to the repository. It also serves as a forum for
  patch review (i.e. send patches here). It is useful for those who want to
  stay on the bleeding edge of LLVM development. This list is very high
  volume.

  .. __: http://lists.llvm.org/pipermail/llvm-commits/

`Bugs & Patches Archive (llvm-bugs)`__
  This list gets emailed every time a bug is opened and closed. It is
  higher volume than the LLVM-dev list.

  .. __: http://lists.llvm.org/pipermail/llvm-bugs/

`Test Results Archive (llvm-testresults)`__
  A message is automatically sent to this list by every active nightly tester
  when it completes.  As such, this list gets email several times each day,
  making it a high volume list.

  .. __: http://lists.llvm.org/pipermail/llvm-testresults/

`LLVM Announcements List (llvm-announce)`__
  This is a low volume list that provides important announcements regarding
  LLVM.  It gets email about once a month.

  .. __: http://lists.llvm.org/mailman/listinfo/llvm-announce

IRC
---

Users and developers of the LLVM project (including subprojects such as Clang)
can be found in #llvm on `irc.oftc.net <irc://irc.oftc.net/llvm>`_.

This channel has several bots.

* Buildbot reporters

  * llvmbb - Bot for the main LLVM buildbot master.
    http://lab.llvm.org:8011/console
  * smooshlab - Apple's internal buildbot master.

* robot - Bugzilla linker. %bug <number>

* clang-bot - A `geordi <http://www.eelis.net/geordi/>`_ instance running
  near-trunk clang instead of gcc.

Meetups and social events
-------------------------

.. toctree::
   :hidden:

   MeetupGuidelines

Besides developer `meetings and conferences <https://llvm.org/devmtg/>`_,
there are several user groups called
`LLVM Socials <https://www.meetup.com/pro/llvm/>`_. We greatly encourage you to
join one in your city. Or start a new one if there is none:

:doc:`MeetupGuidelines`

Community wide proposals
------------------------

Proposals for massive changes in how the community behaves and how the work flow
can be better.

.. toctree::
   :hidden:

   CodeOfConduct
   Proposals/GitHubMove
   BugpointRedesign
   Proposals/LLVMLibC
   Proposals/TestSuite
   Proposals/VariableNames
   Proposals/VectorizationPlan

:doc:`CodeOfConduct`
   Proposal to adopt a code of conduct on the LLVM social spaces (lists, events,
   IRC, etc).

:doc:`Proposals/GitHubMove`
   Proposal to move from SVN/Git to GitHub.

:doc:`BugpointRedesign`
   Design doc for a redesign of the Bugpoint tool.

:doc:`Proposals/LLVMLibC`
   Proposal to add a libc implementation under the LLVM project.

:doc:`Proposals/TestSuite`
   Proposals for additional benchmarks/programs for llvm's test-suite.

:doc:`Proposals/VariableNames`
   Proposal to change the variable names coding standard.

:doc:`Proposals/VectorizationPlan`
   Proposal to model the process and upgrade the infrastructure of LLVM's Loop Vectorizer.

Indices and tables
==================

* :ref:`genindex`
* :ref:`search`
