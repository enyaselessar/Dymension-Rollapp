# Dymension-Rollapp

# Dymension
![1500x500](https://user-images.githubusercontent.com/91562185/234884978-f1a6b9f1-5939-422c-af5d-ca66a9feb758.jpg)

## Sistem Gereksinimleri
| Bileşenler | Minimum Gereksinimler | 
| ------------ | ------------ |
| CPU |	4|
| RAM	| 8+ GB |
| Storage	| 500 GB SSD |


*PORTLAR
 -  Öncelikle 26657, 1317 ve 8545 portlarının açık olması lazım.
 -  RollApp RPC Endpoint (varsayılan 26657)
 -  Rest Endpoint (varsayılan 1317)
 -  JSON RPC Endpoint (varsayılan 8545. Yalnızca EVM RollApps ile ilgilidir)


*KURULUMU YAPALIM
```
sudo apt update && sudo apt upgrade -y
```

```
sudo apt install curl tar wget clang pkg-config libssl-dev jq build-essential bsdmainutils git make ncdu gcc git jq chrony liblz4-tool -y
```

```
curl -L https://dymensionxyz.github.io/roller/install.sh | bash
```

```
roller config init --interactive
```
*bu komuttan sonra gelen sorulara

1)	Enter your RollApp ID:   örn: elessar_3448-1
2)	Specify your RollApp denom: örn: ENY
3)	How many tokens do you wish to mint for Genesis? Token adedini belirleyin örn: 1000000000000000  (bu kısmı fazla belirleyebilirsiniz)
4)	Diğer soruda celestia veya avail seçebilirsiniz.

*Fotoğrafdaki adresleri kaydedin ve discorddan DYM olanlar için DYM faucettan, Celestia için Celestia faucettan token talep edin

![image](https://github.com/enyaselessar/Dymension-Rollapp/assets/108255403/c5a1d420-99b7-433d-a8fc-eb44f2e02ed7)


REGISTER YAPALIM
```
roller tx register
```

![image](https://github.com/enyaselessar/Dymension-Rollapp/assets/108255403/3d653d01-c69e-447c-9f11-2822636646ad)

*Yeni screen açıp, roller run komutunu girelim ve kanal bulmasını bekleyelim
```
Screen -S roller
```
```
roller run 
```

![image](https://github.com/enyaselessar/Dymension-Rollapp/assets/108255403/ae2b2911-110e-474f-b884-cc667fe14bdf)



* Kanal bulduktan sonra ctrl a+d ile screenden çıkıp bu komutu girelim, bu komut oluşturduğumuz kendi tokenımızı dymension discordda görünmesini ve ordan insanların  bizim tokenımızı talep edebilmesini sağlayacak.Transfer 10-20 dk sürebilir.

```
roller tx fund-faucet 
```

* DYM faucet kanalında aşağıdaki komutla, oluşturduğumuz token balansını kontrol ediyoruz.Balans görüyorsak ok.(Adresi değiştirmeyin, sadece rollapp id kendi rollapp adınızı yazın)
```
$balances dym1g8sf7w4cz5gtupa6y62h3q6a4gjv37pgefnpt5 <rollapp-id>
```

* Daha sonra aşağıdaki formatta kendi tokenımızı talep ediyoruz.
```
$request <user-address> <rollapp-id>
```

* Keylerimizi export edip,saklayalım
```
roller keys export hub_sequencer
```
```
roller keys export rollapp_sequencer
```
```
roller keys export my_celes_key
```
