Random NFT mint smart contract for Aptos Blockchain. The smart contract is available in mainnet and testnet. For detail information please go to our [docs](https://docs.mokshya.io)

Mainnet contract : 0x25d440284ca6c13afadb0e83ff1bccacbaa75175551111d8b7cb5d2854e708f0

source_address Contract:  0x8d0bcecc1ad9da703b30c8067b76bd954edd95dfe9c5936d638bb65dd393a27e

admin_account : 0xf42c8f5e4c13b796b4c729bb78cc8e5632b00eb4eaba3857d2272af4bb49d4a3 (which is the address that initiates the source address)



1. 部署合约
2. 执行init_candy方法，创建资源账户和指定admin管理地址
3. 用户执行mint操作，mint资源的限制条件都写在资源账户中。
4. 合约更新可以通过更新资源账户地址，通过重新提供参数部署资源合约地址进行执行合约的更新操作

# Quick Installation 

```shell
yarn & cd packages/CLI & yarn & cd ../Candymachine-UI & yarn & ../../
```
# Set up candy machine 

```shell
ts-node packages/CLI/src/index.ts --create_candy 
```

# Add whitelist Users

```shell
ts-node packages/CLI/src/index.ts --create_whitelist 
```

# Mint NFT UI

* copy the resource_account from config.json file.

```shell
cd package/Candymachine-UI & yarn
```

* Add config.json resource_account to the env file in resource_account .

```shell 
npm run dev  
```
