midiServer
==========

MIDI websocket nodeJS server.

Installation
------------

Requires nodeJS and the following modules :
- commander
- midi
- websocket
- http

Running
-------

- To display help: node midiServer.js -h
- To list MIDI inputs/outputs: node midiServer.js -l
- To select inputs/outputs: node midiServer.js -i midiInputNumber -o midiOutputNumber
 
Websocket message syntax
------------------------

[ eventType, note, velocity ]

eventType : 144 = note On event
            128 = note Off event

example : [ 144, 65, 100 ]
