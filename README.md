# INTUcoin
sudo apt-get install build-essential libboost-all-dev 

git clone https://github.com/intucoin/INTUcoin.git

cd INTUcoin 

mkdir build && cd build

cmake ..

make

./intucoind --rpc-bind-ip 0.0.0.0  --enable-blockexplorer --enable-cors '*'

./simplewallet --wallet-file your_pool_wallet --password your_password --rpc-bind-ip 127.0.0.1 --rpc-bind-port 8082
