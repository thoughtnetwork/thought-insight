
Create thought.conf in ~/.thoughtcore

```
server=1
addnode=phi.thought.live
txindex=1
addressindex=1
timestampindex=1
spentindex=1
zmqpubrawtx=tcp://127.0.0.1:28332
zmqpubrawtxlock=tcp://127.0.0.1:28332
zmqpubhashblock=tcp://127.0.0.1:28332
rpcallowip=127.0.0.1
rpcuser=thought
rpcpassword=local321
```

Run ./thoughtd binary


Edit dashcore-node.json

```
"servicesConfig": {
    "dashd": {
      "connect": [
        {
          "rpchost": "127.0.0.1",
          "rpcport": "10617",
          "rpcuser": "thought",
          "rpcpassword": "local321",
          "zmqpubrawtx": "tcp://127.0.0.1:28332"
        }
      ]
    }
  }
```

Packages
------------
thoughtcore-lib - https://phab.thought.live/diffusion/45/

thoughtcore-node - https://phab.thought.live/diffusion/46/ 

thoughtd-rpc - https://phab.thought.live/diffusion/47/

insight-api - https://phab.thought.live/diffusion/49/

insight-ui - https://phab.thought.live/diffusion/50/
