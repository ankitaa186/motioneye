**motionEye** is a web-based frontend for `motion <https://motion-project.github.io>`_. Check out the `wiki <https://github.com/ccrisan/motioneye/wiki>`_ for more details. Changelog is available on the `releases page <https://github.com/ccrisan/motioneye/releases>`_.


.. image:: https://badges.gitter.im/Join%20Chat.svg
   :alt: Join the chat at https://gitter.im/ccrisan/motioneye
   :target: https://gitter.im/ccrisan/motioneye?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge

You can support the development of motionEye by making a small donation.

.. image:: https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif
   :alt: [paypal]
   :target: https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=ccrisan%40gmail%2ecom&lc=US&item_name=motionEye&no_note=0&currency_code=USD&bn=PP%2dDonationsBF%3abtn_donate_LG%2egif%3aNonHostedGuest

Ankit's custom instructions
===========================

Build motioneye image
---------------------

```docker build --build-arg VCS_REF=$(git rev-parse HEAD) --build-arg BUILD_DATE="2021-01-24T1951" -t ankitaa186/motioneye:master-amd64 -f extra/Dockerfile . ```

Run using docker-compose
------------------------

```docker-compose -f extra\docker-compose.yml -p motioneye up -d```

Tips
----

For Samba share:
1. install cifs tools
2. turn on smb in motioneye config
3. run the container as priviledged
