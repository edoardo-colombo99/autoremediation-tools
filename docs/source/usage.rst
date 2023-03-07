Usage
=====

.. _installation:

Installation
------------

To start using this project first of all you have to create an ansible project for each customer (tricode)

The project must be named like this(where xxx is the tricode of customer like bsm, wti, weu):

.. code-block:: console

   xxx_project_healthscan_autoremediation_tools

The project must be linked to this out github repository at main branch

.. code-block:: console

   https://github.kyndryl.net/KIIS-Autoremediation/autoremediation-ansible-setup.git


A credential for Github must be used in order to clone the code. The project must look like this:

.. image:: /img/ansaibol-touer.png


After the project creation a jobtemplate "tools" must be created

The JT must be named like this(where xxx is the tricode of customer like bsm, wti, weu):

.. code-block:: console

   xxx_jobtemplate_healthscan_autoremediation_tools

An "Ansible Tower" credential must be selected in order to gain Administrator privilegese to make api requestes, also the inventory must be selected. Without these 2 thinks the playbook execution will fail

The JT must point to "projects.yml"

The JT must look like this:

.. image:: /img/ansaibol-gobtemplate.png
