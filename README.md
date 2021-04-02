# Module 18 Homework for James Reeves

# NODE INFORMATION FOR INSTRUCTIONS BELOW FOR ZBANK COIN

## NODE1-
Public address of the key:   0xaCa3fc0420950d2ebF56a1fE1126563247Ac75cf
Path of the secret key file: node1\keystore\UTC--2021-04-02T16-15-43.345795200Z--aca3fc0420950d2ebf56a1fe1126563247ac75cf

enode://8b580a72de3ba0b7ccd5b1c434d7592df9cc0b2d49978a56569208065975ea7d83942916e387ed75989e2201726394c100f35abc262f3478f7b8df7a28cdad57@127.0.0.1:30303

## NODE2-
Public address of the key:   0x8Bb67CBdCc0ae9B7927D05AbF85EAfcEf1c97017
Path of the secret key file: node2\keystore\UTC--2021-04-02T16-16-43.690187000Z--8bb67cbdcc0ae9b7927d05abf85eafcef1c97017

## Block ID - 1234

## Ports -
30303
30304

## Instructions:
Using geth, initialize each node with the new networkname.json. Go to GETH/BlockChain-ToolsHWFinal and enter:

./geth --datadir node1 init zbank.json
./geth --datadir node2 init zbank.json

Now the nodes can be used to begin mining blocks.

Run the nodes in separate terminal windows with the commands:

./geth --datadir node1 --unlock "0xaCa3fc0420950d2ebF56a1fE1126563247Ac75cf" --mine --rpc --allow-insecure-unlock

./geth --datadir node2 --unlock "0x8Bb67CBdCc0ae9B7927D05AbF85EAfcEf1c97017" --mine --port 30304 --bootnodes "enode://8b580a72de3ba0b7ccd5b1c434d7592df9cc0b2d49978a56569208065975ea7d83942916e387ed75989e2201726394c100f35abc262f3478f7b8df7a28cdad57@127.0.0.1:30303" --ipcdisable --allow-insecure-unlock

NOTE: Type your password and hit enter - even if you can't see it visually!

f3ByJ6e7&

Go to MyCrypto and open up the zbank testnet

Open up the wallet with the keycode located in the GETH/BlockChain-ToolsHWFinal folder for node1

Send whatever amount you wish once the wallet is populated to node2 address