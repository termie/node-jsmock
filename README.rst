===========
node-jsmock
===========

This is a quick wrapper around JSMock that adds the exports so that it can be
imported by Node.

See http://jsmock.sourceforge.net for usage.

For a general purpose unit testing framework, see http://github.com/termie/node-unittest

General Usage
=============

::

  var jsmock = require('jsmock');
  var mock = jsmock.MockControl();

  var mockSomething = mock.createMock(Something);

  mockSomething.expects().foo().AndReturn('bar');

  mockSomething.foo();

  mock.verify();

License Bits
============

All the original license stuff applies, these changes are minimal.
