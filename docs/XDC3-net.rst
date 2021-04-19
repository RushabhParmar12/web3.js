.. _net:

.. include:: include_announcement.rst

========
xdc3.*.net
========


The ``xdc3-net`` package allows you to interact with the Ethereum nodes network properties.


.. code-block:: javascript

    import xdc3 from 'xdc3';
    import {Net} from 'xdc3-net';

    // "Personal.providers.givenProvider" will be set if in an Ethereum supported browser.
    const net = new Net(xdc3.givenProvider || 'ws://some.local-or-remote.node:8546', options);


    // or using the xdc3 umbrella package
    const xdc3 = new xdc3(xdc3.givenProvider || 'ws://some.local-or-remote.node:8546', options);

    // -> xdc3.eth.net
    // -> xdc3.bzz.net
    // -> xdc3.shh.net



------------------------------------------------------------------------------


.. include:: include_package-net.rst


------------------------------------------------------------------------------
