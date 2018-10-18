ansible-mailgun
===============

[![Build Status](https://travis-ci.org/pulse-mind/ansible-mailgun.svg?branch=master)](https://travis-ci.org/pulse-mind/ansible-mailgun)

This role configures postfix to use [Mailgun](http://mailgun.com) for outgoing
email on Linux servers.

Requirements
------------

Ansible 2.7 is strongly recommended, but Ansible 2.4 should work (unless
you're on Fedora, then you need 1.9 for sure for `dnf` support).

Role Variables
--------------

The variables for this role are found within `defaults/main.yml` and include
the following:

* _mailgun_username_ - your Mailgun SMTP username
* _mailgun_password_ - your Mailgun SMTP password

**Please note:** This is your SMTP username/password combination, not the
credentials you use to access the Mailgun dashboard on the website. The SMTP
credentials should be different for each domain you host and they're found
here:

    https://mailgun.com/app/domains/{your-domain-name}

Dependencies
------------

This role has no dependencies.

License
-------

Apache 2.0

Author Information
------------------

Original Author : [Major Hayden](http://majorhayden.com)
