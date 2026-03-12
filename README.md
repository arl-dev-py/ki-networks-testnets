# KI Networks Testnets

Configurations and instructions for connecting to **testnet** networks KI Network (Cosmos SDK).

## Quick connection

1. Clone repository
git clone https://github.com/arl-dev-py/ki-networks-testnets.git
cd ki-networks-testnets

2. Download genesis files
# Main testnet
curl -o testnet-1/genesis.json https://rpc.testnet-1.ki.network/genesis
curl -o testnet-1/addrbook.json https://rpc.testnet-1.ki.network/addrbook.json

# All testnets
./download-all.sh

3. Run node
# Install KI binary
curl -sSfL https://raw.githubusercontent.com/KiFoundation/ki-node/main/install.sh | bash
export PATH=$PATH:~/.ki/bin

# Initialize
kid init "MyNode" --chain-id testnet-1

# Start
kid start


---

# KI Networks Testnets

Конфигурации и инструкции для подключения к **testnet** сетям KI Network (Cosmos SDK).

## Быстрое подключение

1. Клонировать репозиторий
git clone https://github.com/arl-dev-py/ki-networks-testnets.git
cd ki-networks-testnets

2. Скачать genesis файлы
# Основной testnet
curl -o testnet-1/genesis.json https://rpc.testnet-1.ki.network/genesis
curl -o testnet-1/addrbook.json https://rpc.testnet-1.ki.network/addrbook.json

# Все testnets
./download-all.sh

3. Запустить ноду
# Установить KI binary
curl -sSfL https://raw.githubusercontent.com/KiFoundation/ki-node/main/install.sh | bash
export PATH=$PATH:~/.ki/bin

# Инициализация
kid init "MyNode" --chain-id testnet-1

# Запуск
kid start

