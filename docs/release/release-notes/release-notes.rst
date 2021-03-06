.. This work is licensed under a
.. Creative Commons Attribution 4.0 International License.
.. http://creativecommons.org/licenses/by/4.0
.. (c) 2015-2017 AT&T Intellectual Property, Inc

======================================================================
OPNFV Copper Release Notes
======================================================================

This document provides the release notes for the Danube Release of Copper.

.. contents::
   :depth: 3
   :local:


Version History
---------------

+--------------------+--------------------+--------------------+--------------------+
| **Date**           | **Ver.**           | **Author**         | **Comment**        |
|                    |                    |                    |                    |
+--------------------+--------------------+--------------------+--------------------+
| 2017 Feb 7         | 1.0                | Bryan Sullivan     |                    |
|                    |                    |                    |                    |
+--------------------+--------------------+--------------------+--------------------+

Important Notes
---------------


Summary
-------

The Danube release of OPNFV Copper is based on OpenStack Newton.

Release Data
------------

Copper Release 1 Scope
^^^^^^^^^^^^^^^^^^^^^^
OPNFV Brahmaputra was the initial OPNFV release for Copper, and achieved the
goals:

  * Add the OpenStack Congress service to OPNFV, through at least one installer
    project, through post-install configuration.
  * Provide basis tests scripts and tools to exercise the Congress service

Copper Release 2 Scope
^^^^^^^^^^^^^^^^^^^^^^
OPNFV Colorado includes the additional features:
  * Congress support in the the OPNFV CI/CD pipeline for the JOID and Apex
    installers, through the following projects being upstreamed to OpenStack:

    * For JOID, a JuJu Charm for Congress
    * For Apex, a Puppet Module for Congress

  * Congress use case tests integrated into Functest and as manual tests
  * Further enhancements of Congress test tools

Copper Release 3 Scope
^^^^^^^^^^^^^^^^^^^^^^
OPNFV Danube includes the additional features:
  * Manual tests

    * Network Bridging test to detect when a VM is connected to 2 networks with different security levels and then pause that VM

  * Further enhancements of Congress test scripts

Version Change
^^^^^^^^^^^^^^

Module Version Changes
~~~~~~~~~~~~~~~~~~~~~~
- Openstack has changed from Mitaka to Newton

Known Limitations, Issues and Workarounds
-----------------------------------------

The following features have not been verified as of this release:

  * HA deployment: Congress should be installed in OPNFV deployments in a
    non-HA mode, including in HA deployment scenarios. Basic HA support has been
    implemented for Congress (see http://docs.openstack.org/developer/congress/index.html), but
    this feature has not yet been verified on the OPNFV platform.

  * Horizon plugin: The Congress OpenStack Dashboard plugin (a "Policy tab") has not been
    deployed in OPNFV as of this release. Installing the needed Congress Dashboard plugin
    files on the OpenStack Dashboard host is a future work item.

