NOVA Project Documentation
==========================

Welcome to the documentation for the NOVA project! NOVA is designed to bring advanced visualizations to the neutron group at SNS (Spallation Neutron Source) at ORNL (Oak Ridge National Laboratory). It leverages a combination of Python libraries and a web framework to create powerful and interactive tools for data analysis and exploration.

This documentation provides an overview of the different components of the NOVA project.  For detailed information, please refer to the specific documentation for each library.

Project Libraries
-----------------

The NOVA project is built around the following core libraries:

*   :ref:`nova-galaxy`
*   :ref:`nova-trame`
*   :ref:`nova-mvvm`

.. _nova-galaxy:

nova-galaxy: Pythonic Galaxy Tool Automation
--------------------------------------------

``nova-galaxy`` is a Python library designed to simplify and streamline interaction with Galaxy servers for tool execution and data management. It provides an intuitive and Pythonic way to automate Galaxy workflows, manage data, and integrate Galaxy tools into your Python applications.

It allows users to easily manage Galaxy datasets and tools from python scripts. This means that users can automate complex data processing pipelines directly from Python.

For detailed information, please refer to the `nova-galaxy documentation <https://nova-application-development.readthedocs.io/projects/nova-galaxy/en/latest/>`_.

.. _nova-trame:

nova-trame: Interactive Application Development
-----------------------------------------------

``nova-trame`` is a UI package that uses the Trame framework to simplify the creation of interactive web applications for the NOVA project.  It provides a set of pre-built components and layouts that streamline the application development process.

``nova-trame`` aims to make it easy to build powerful interactive user interfaces in pure python. These web based applications are designed to be easy to share and deploy.

For detailed information, please refer to the `nova-trame documentation <https://nova-application-development.readthedocs.io/projects/nova-trame/en/stable/>`_.

.. _nova-mvvm:

nova-mvvm: MVVM Bindings for Python
-----------------------------------

``nova-mvvm`` is a Python library that helps with the implementation of Model-View-ViewModel (MVVM) architectural pattern for GUI applications.  It provides a framework for connecting view components with underlying data models. This library supports several UI frameworks including PyQt and Trame.

By providing a structured way to manage data binding it aims to significantly reduce the boilerplate required to create MVVM style applications.

For detailed information, please refer to the `nova-mvvm documentation <https://nova-application-development.readthedocs.io/projects/mvvm-lib/en/latest/>`_.

Getting Started
---------------

If you are new to developing NOVA applications, then we recommend you walk through the `NOVA Tutorial <https://nova.ornl.gov/tutorial/>`_. This will guide you through setting up your development environment and introduce you to working with the above NOVA libraries.
