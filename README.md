node-red-contrib-jsonrpc
==============================

<a href="http://nodered.org" target="_new">Node-RED</a> node for JSON-RPC 2.0 communication. Wraps <a href="https://www.npmjs.com/package/json-rpc2">node-jsonrpc2</a>.

Install
-------

Run the following command in your Node-RED user directory - typically `~/.node-red`

        npm install node-red-contrib-jsonrpc

Example
-----

An example of communicating with ethereum.
```
[{"id":"8b5fb501.4af498","type":"jsonrpc-call","z":"838a7f87.ba911","name":"","method":"eth_sendTransaction","client":"bbdeb946.30bd18","x":330.5,"y":85,"wires":[["b3951.3b65e6b"]]},{"id":"cdef05f.e8692f8","type":"inject","z":"838a7f87.ba911","name":"","topic":"","payload":"{\"from\":\"0x627306090abaB3A6e1400e9345bC60c78a8BEf57\",\"value\":\"0x0de0b6b3a7640000\",\"to\":\"0x05eee23f682718f129719df9d0d0254542c6a10e\"}","payloadType":"json","repeat":"","crontab":"","once":false,"onceDelay":0.1,"x":119.5,"y":61,"wires":[["8b5fb501.4af498"]]},{"id":"b3951.3b65e6b","type":"debug","z":"838a7f87.ba911","name":"","active":true,"tosidebar":true,"console":false,"tostatus":false,"complete":"false","x":520.5,"y":141,"wires":[]},{"id":"bbdeb946.30bd18","type":"jsonrpc-client","z":"","name":"ganache","host":"localhost","port":"7545","connection":"http"}]
```

Acknowledgements
==============================

Uses <a href="https://github.com/pocesar" target="_new">procesar</a>'s fork of the json rpc 2.0 implementation <a href="https://github.com/pocesar/node-jsonrpc2" target="_new">https://github.com/pocesar/node-jsonrpc2</a>.
