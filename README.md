Email Verify
======================

Copyright: Daniel Bonniot <bonniot@users.sourceforge.net>


This module provides advanced email address checking. It does this by checking
that an email address actually exists when it is provided.

The module does this in two ways:

1. Checks if the domain/host part of the address exists
1. Tries to validate the full email address by sending a HELO/MAIL FROM/RCPT TO
   chain of commands to the SMTP servers for the found host.

Some hosts will not reveal if an email address is valid ("catch-all policy")
while others might refuse the check entirely.  When in doubt, the module will
play it safe and accept some potentially invalid addresses rather than to refuse
potentially valid ones.



Installation <!-- This section is required. -->
------------

- Install this module using the official Backdrop CMS instructions at
  https://docs.backdropcms.org/documentation/extend-with-modules.

- Visit the configuration page under Administration > Configuration > System >
  Email Verification (admin/config/system/email_verify) and enter the required
  information.

- You must check the "Enabled" box and then save configuration. Email checking
  will be activated for user account verification immediately.

- Any additional steps.


Issues <!-- This section is required. -->
------

Bugs and feature requests should be reported in [the Issue Queue](https://github.com/backdrop-contrib/email_verify/issues).

* When reporting issues, it would be most helpful you can provide a detailed
  SMTP conversation to illustrate what is happening. The conversation should be
  from the machine hosting your site (as opposed to a local installation).

Current Maintainers <!-- This section is required. -->
-------------------

- [Jen Lampton](https://github.com/jenlampton).
- [Jason Flatt](https://github.com/oadaeh).
<!-- You may also wish to add: -->
- Seeking additional maintainers.

Credits <!-- This section is required. -->
-------

- Ported to Backdrop CMS by [Jen Lampton](https://github.com/jenlampton).
- Originally written for Drupal by [Daniel Bonniot](mailto:bonniot@users.sourceforge.net).

License <!-- This section is required. -->
-------

This project is GPL v2 software.
See the LICENSE.txt file in this directory for complete text.

<!-- If your project includes other libraries that are licensed in a way that is
compatible with GPL v2, you can list that here too, for example: `Foo library is
licensed under the MIT license.` -->

