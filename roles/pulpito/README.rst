Pulpito
=======

This role is used to configure a node to run pulpito_.

It has been tested on:

- CentOS 7.x
- Debian 8.x (Jessie)
- Ubuntu 14.04 (Trusty)

Dependencies
++++++++++++

Since pulpito_ is only useful as a frontend to paddles_, it requires a paddles_ instance to function. Additonally, you must set ``paddles_address`` in e.g. your secrets repository to the URL of your instance.


.. _pulpito: https://github.com/ceph/pulpito
.. _paddles: https://github.com/ceph/paddles

Variables
+++++++++

``pulpito_repo``: Optionally override the pulpito git repo.

``pulpito_branch``: Optionally override the pulpito repo branch.
For GitHub pull requests the values refs/pull/X/merge or refs/pull/X/head
can be used.

``pulpito_user``: The system account to create and use (Default: pulpito)
