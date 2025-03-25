# Seismic-Devnet-Deploy-and-Transact

Req after doing deploy.sh and transact.sh
Faucet https://faucet-2.seismicdev.net


Explorer
https://explorer-2.seismicdev.net/

## Deploy an encrypted contract

```
curl https://sh.rustup.rs -sSf | sh
```
```
. "$HOME/.cargo/env"
```
```
curl -L \
     -H "Accept: application/vnd.github.v3.raw" \
     "https://api.github.com/repos/SeismicSystems/seismic-foundry/contents/sfoundryup/install?ref=seismic" | bash
```
```
source ~/.bashrc
```
```
sudo apt update && sudo apt install -y build-essential
sudo apt install cargo -y
```
```
sfoundryup 
```
```
git clone --recurse-submodules https://github.com/SeismicSystems/try-devnet.git
cd try-devnet/packages/contract/
```
```
bash script/deploy.sh
```


## **Interact with an encrypted contract**
```
sudo apt install unzip
```
```
curl -fsSL https://bun.sh/install | bash
```
```
cd
cd try-devnet/packages/cli/
```
```
source ~/.bashrc
```
```
bun install
```
```
bash script/transact.sh
```

