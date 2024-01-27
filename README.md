# BEVM-Node-Kurulumu
BEVM Testnet Node Kurulumu

Gereksinimler: Nefes alsın yeter

Benim Cihazım: 2 CPU 4 RAM 40 GB SSD (Santiment node kurulu)


SİSTEMİMİZİ GÜNCELLEYELİM

```shell
sudo apt-get update
```

```shell
sudo apt-get upgrade
```

DOCKER KURALIM


Tek tek girip onay veriyoruz

```shell
curl -fsSL https://get.docker.com -o get-docker.sh
```

```shell
sudo sh get-docker.sh
```

Versiyon Kontrolü

```shell
docker -v
```

Hata Yoksa Devam Ediyoruz

```shell
cd /var/lib
```

```shell
mkdir node_bevm_test_storage
```

```shell
sudo docker pull btclayer2/bevm:v0.1.1
```

Ödül alabilmek için NODE_ADINIZ Yazan yere CÜZDAN ADRESİNİZİ girin.

```shell
sudo docker run -d -v /var/lib/node_bevm_test_storage:/root/.local/share/bevm btclayer2/bevm:v0.1.1 bevm "--chain=testnet" "--name=NODE_ADINIZ" "--pruning=archive" --telemetry-url "wss://telemetry.bevm.io/submit 0"
```


Telemetry'de nickinizi aratın. Nickiniz varsa sorun yok. https://telemetry.bevm.io/


BEVM

Discord https://discord.gg/V38ZN6mc
Twitter https://twitter.com/BTClayer2
Telegram https://t.me/+elsWWcz3dbhiNTVl


www.x.com/0xMultijet
