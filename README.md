Description
===========

This cookbook will add rackconnect to the sudoers files. This allows RackConnect automation to update software firewall.

Mostly useful if you have other chef cookbooks/recipes that edit/manage sudoers.

More features coming soon.

Requirements
============

You will need the [sudo](http://ckbk.it/sudo) cookbook.

Usage
=====

You NEED to enable (set to true) the `/etc/sudoers.d/` attribute (default is false):

    node['authorization']['sudo']['include_sudoers_d']

Then just include the recipe `rackconnect`.
