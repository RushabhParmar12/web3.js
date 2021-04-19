
.. include:: include_announcement.rst

===============
Getting Started
===============

The XDC3.js library is a collection of modules which contain specific functionality for the XinFin Network ecosystem.

- The ``XDC3-eth`` is for the ethereum blockchain and smart contracts
- The ``XDC3-shh`` is for the whisper protocol to communicate p2p and broadcast
- The ``XDC3-bzz`` is for the swarm protocol, the decentralized file storage
- The ``XDC3-utils`` contains useful helper functions for Dapp developers.


.. _adding-web3:

Adding XDC3.js
==============

.. index:: npm
.. index:: bower
.. index:: meteor

First you need to get XDC3.js into your project. This can be done using the following methods:

- npm: ``npm install XDC3``
- meteor: ``meteor add XinFin:XDC3``
- pure js: link the ``dist/XDC3.min.js``

After that you need to create a web3 instance and set a provider.
XinFin supported Browsers like XinPay will have a ``XinFinProvider`` or ``XDC3.currentProvider`` available. For  XDC3.js, check ``XDC3.givenProvider``.
If this property is ``null`` you should connect to a remote/local node.

.. code-block:: javascript

    // in node.js use: const Web3 = require('web3');

    const web3 = new XDC(XDC3.givenProvider || "ws://localhost:8546");

That's it! now you can use the ``XDC3`` object.
