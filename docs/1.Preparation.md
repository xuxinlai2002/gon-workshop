# 1.Gon's Preparation

## Overview

If you want to participate in GoN activities and get Points, you need to make the following preparations


### Preparation

#### 1. Registration of Gon
Registration is available through the link  [Gon Register](https://docs.google.com/forms/d/e/1FAIpQLSfIhkXzOUTNu5R2cueCSt-_0Dic4MdsF193I9GSx64YTqNyWw/viewform)


#### 2. Install CLIs for gon chains (command-line interface) 

+ [IRISnet](https://www.irisnet.org/docs/get-started/install.html)
```sh
git clone https://github.com/irisnet/irishub
cd irishub
git checkout feature/gon
make install
iris version # 1.4.1-gon-testnet
```

+ [Uptick](https://docs.uptick.network/quickstart/installation.html)
```sh
git clone https://github.com/UptickNetwork/uptick.git
cd uptick
make install
uptickd version # v0.2.6
```

+ [Stargaze](https://docs.stargaze.zone/nodes-and-validators/getting-setup)
```sh
git clone https://github.com/public-awesome/stargaze
cd stargaze
git fetch
git checkout 8.0.0-rc.1
make install
starsd version # 8.0.0-rc.1
```

+ [Juno](https://docs.junonetwork.io/validators/getting-setup)

```sh
git clone https://github.com/CosmosContracts/juno
cd juno
git fetch
git checkout v10.0.0
make install
junod version # v10.0.0
```


+ [OmniFlix](https://github.com/omniflix/omniflixhub#installation)
```sh
git clone https://github.com/Omniflix/omniflixhub.git
cd omniflixhub
git checkout v0.9.0-gon-rc5
make install
omniflixhubd version # 0.9.0-gon-rc5
```

#### 3. Setup Chains Configartion

+ IRISNet
```sh
# config
iris config chain-id gon-irishub-1
iris config node http://34.80.93.133:26657
iris config output json
iris config broadcast-mode block
# show and check config
iris config
```

+ Uptick
```sh
# config
uptickd config chain-id uptickd_7000-2
uptickd config node http://52.220.252.160:26657
uptickd config output json
uptickd config broadcast-mode block
# show and check config
uptickd config
```

+ Stargaze
```sh
# config
starsd config chain-id elgafar-1
starsd config node https://rpc.elgafar-1.stargaze-apis.com:443
starsd config output json
starsd config broadcast-mode block
# show and check config
starsd config
```

+ Juno
```sh
# config
junod config chain-id uni-6
junod config node https://rpc.uni.junonetwork.io:443
junod config output json
junod config broadcast-mode block
# show and check config
junod config
```

+ Omniflix
```sh
# config
omniflixhubd config chain-id osmo-test-4
omniflixhubd config node https://rpc.testnet.osmosis.zone:443
omniflixhubd config output json
omniflixhubd config broadcast-mode block
# show and check config
omniflixhubd config
```

#### 4. Create Wallets (Keyrings)

+ IRISNet
```sh
iris keys add <keyName> # key name 
```

+ Uptick
```sh
uptickd keys add <keyName> #  key name 
```

+ Stargaze
```sh
starsd keys add <keyName> #  key name 
```

+ Juno
```sh
Junod keys add <keyName> #  key name 
```

+ Omniflix
```sh
omniflixhubd keys add <keyName> #  key name 
```

#### 5. Get Test Coin From Faucet

+ [multi-chain faucet website](https://faucet.ping.pub/)
+ Discord

| #  | Testnets | Faucet Link |
| ------------- | ------------- |  ------------- |
| 1  | IRISnet  | https://discord.gg/r3U7AR9bhe |
| 2  | Uptick   | https://discord.gg/7NRNv5wB |
| 3  | Stargaze   |  https://discord.gg/stargaze |
| 4  | Juno   |  https://discord.gg/juno |
| 5  | OmniFlix   | https://discord.gg/k586GjYT |


#### 6. Get IBC Channel Info
| #  | aSide | bSize |
| ------------- | ------------- |  ------------- |
| 1  | uptick (channel-3)   |  iris("channel-17) |
| 2  | uptick (channel-4)   |  iris("channel-19)|
| 3  | uptick (channel-5)   |  OmniFlix("channel-41) |
| 4  | uptick (channel-6)   |  Stargaze("channel-203) |
| 5  | uptick (channel-7)   |  Juno("channel-86) |

+ [more](https://github.com/game-of-nfts/gon-testnets/#Appendix)

