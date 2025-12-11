<p align="center">
  <img height="100" height="auto" src="https://github.com/user-attachments/assets/f08682f1-9c97-458e-a18f-96ecdaa78da6"">
</p>

# Push Testnet

Official documentation:
>- [Validator setup instructions](https://push.org/docs/chain/node-and-system-tools/running-push-validator)

Explorer:
>- [Explorer](https://donut.push.network/)

### Minimum Hardware Requirements
 - 4x CPUs; the faster clock speed the better
 - 8GB RAM
 - 100GB of storage (SSD or NVME)

### Recommended Hardware Requirements 
 - 8x CPUs; the faster clock speed the better
 - 16GB RAM
 - 1TB+ of storage (SSD or NVME)

 - Ubuntu 22.04

Устанавливаем ноду:

```
sudo apt update & sudo apt upgrade -y
```

```
sudo apt install curl iptables build-essential git wget lz4 jq make gcc nano automake autoconf tmux htop nvme-cli pkg-config libssl-dev libleveldb-dev tar clang bsdmainutils ncdu unzip libleveldb-dev git-all protobuf-compiler screen libgbm1 ca-certificates gnupg -y
```

```
curl -fsSL https://get.push.network/node/install.sh | bash
```

Пишем Y.

<img width="497" height="124" alt="Termius_khqVeuysaK" src="https://github.com/user-attachments/assets/48099a3f-c2bb-4c59-be79-6c2ab7a1ebf3" />

Придумываем имя валидатора на английском.

<img width="520" height="217" alt="Termius_RWZ3lTp75L" src="https://github.com/user-attachments/assets/09d30af1-0ab4-4e12-8ddf-c10f12880739" />

Вписываем имя ключа: validator-key.

<img width="579" height="34" alt="Termius_Fkmgsul2pL" src="https://github.com/user-attachments/assets/22b6c839-1075-439d-b9dd-a49735dfa202" />

Пишем 5.

<img width="390" height="37" alt="Termius_ESA3Bj9J8u" src="https://github.com/user-attachments/assets/9d982baa-53bf-4e70-8e1a-2521456ed9b4" />

Сохраняем фразу кошелька где написано "Recovery Mnemonic Phrase" и адреса кошельков в поле "Account Info". Далее запрашиваем тестовые токены на EVM адрес через кран - https://faucet.push.org/ Запросить придется 2 раза с промежутком в 6ч, так как нам потребуется больше 1 токена. После того как нужное кол-во токенов есть на кошельке, в терминале нажимаем - Enter.

<img width="617" height="471" alt="Termius_9mUIKI8ng7" src="https://github.com/user-attachments/assets/b0b04d9e-e30a-4e05-be99-e6b54902aa76" />

Вписываем 1.5 или больше.

<img width="693" height="878" alt="Termius_iqzFVmwZLz" src="https://github.com/user-attachments/assets/ff583f43-9ccb-43bc-861e-474aa3a8df0c" />

Нажимаем Enter.

Закрыть Dashboard - CTRL + C

```
source ~/.bashrc
```

Полезные команды:

Cтатус узла:

```
push-validator status
```

Открыть Dashboard:

```
push-validator dashboard
```

