========
rdp
========

Formula to enable Windows Remote Desktop and configure the terminal service.

.. note::

    See the full `Salt Formulas installation and usage instructions
    <http://docs.saltstack.com/en/latest/topics/development/conventions/formulas.html>`_.

Status
======

* This formula has been tested on salt-minion 2015.5.8, running under Windows Server 2008r2 SP1 and Windows Server 2012r2.

Available states
================

.. contents::
    :local:

``rdp``
----------
Meta-state which includes the following states, in order::

    rdp.rdp
    rdp.registry
    rdp.service

``rdp.rdp``
----------
Toggles access to Windows Remote Desktop connections. Settings are configurable via the pillar.

``rdp.registry``
----------
Toggles Network Level Authentication and sets the ingress TCP port number for RDP. Settings are configurable via the pillar.

``rdp.service``
-----------
Ensures the TermService and UmRdpService services are running.

Defaults
========

See ``rdp/defaults.yml``.

