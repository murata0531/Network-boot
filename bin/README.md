# ネットワークの作成
sudo ./setup network --name br0 --address 172.24.0.1/16

# クライアントの起動
sudo ./setup node --network br0

# VMと仮想ネットワークを破棄

TAPの削除
    $ sudo ip tuntap delete tap0 mode tap
ブリッジの削除
    $ sudo ip link delete br0 type bridge