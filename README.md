pyharmony
=========

Python library for connecting to and controlling the Logitech Harmony Link

Protocol
--------

As the harmony protocol is being worked out, notes are in PROTOCOL.md.

Status
------

* Authentication to Logitech's web service working.
* Authentication to harmony device working.
* Sending a simple command to harmony device working.

Further Exploration
-------------------

To capture packets for later viewing and inspection in Wireshark the following command will output raw TCP traffic on an iPhone
  `tcpdump -i en0 -s 0 -v -w > /tmp/yourOutputFile`

TODO
----

* Figure out how to detect when the session token expires so we can get a new
  one.
* Figure out sync protocol.
* Figure out a good way of sending commands based on sync state.
* Is it possible to update device configuration?
