# Dymension-Github-PR

## Dymension reposunu  forklayalım 
https://github.com/dymensionxyz/rollapp-registry  adresine gidip burdaki repoyu forklayalım.

## Forkladığımız repoyu sunucumuza çekelim

```
git clone https://github.com/enyaselessar/rollapp-registry
```
* enyaselessar yazan yere github kullanıcı ismini yazalım
```
cd rollapp-registry
```

* Burdaki elessar yazan yerlere kendi rollapp ismimizi yazacağız
```
export ROLLAPP_ID=rollapp adımız
```
*Logo klasörü oluşturalım
```
mkdir -p $ROLLAPP_ID/logos
```
```
cd $ROLLAPP_ID && touch $ROLLAPP_ID.json
```

## Logo klasörünün (/root/rollapp-registry/ elessar_1191427-1/logos/ ) içine istediğimiz bir logo koyalım (svg, png veya jpg formatında)
* Not logo klasörünün içine koyacağımız logonun ismini de rollapp idmiz yazarak değiştirelim.
Örneğin elessar_1191427-1.png
        elessar_1191427-1.svg gibi

## ROLLER CONFİG DOSYASINI EXPORT EDELİM
```
roller config export 
```
* Sunucu üzerinden yukarıdaki kod ile alacağınız çıktıyı parantezler dahil bir yere kopyalayın.
  ![image](https://github.com/enyaselessar/Dymension-Rollapp/assets/108255403/7985678a-9c44-4642-b34a-7e2c1065ae89)
```
Cd
```
```
cd rollapp-registry
```

```
cd rollappadınız

```

```
nano elessar_1191427-1.json
```
* Nano komutunda çıkan yere yukarıda kopyaladığımız bilgileri, Aşağıdaki yerleri bulup ip adresini yazıcaksınız vps'in. sonra ctrl+x y enter dicez kaydedicez. En son hali aşağıdaki gibi olacak.

```
"rpc": "http://sunucu-ipniz:26657"
"rest": "http://sunucu-ipniz:1317"
"rpc": http://sunucu-ipniz:8545
```


![image](https://github.com/enyaselessar/Dymension-Rollapp/assets/108255403/3d2ed5ff-fb69-4fdc-8553-bc78e3372e4c)

#### Sunucumuzdan /root/rollapp-registry/ klasörü içindeki  elessar_1191427-1(sizin kendi oluşturduğunuz isim olacak) dosyayı masaüstüne kaydedin.


* İlk maddede dymension reposunu forklamıştık.Forkladığımız adrese gidip upload files diyerek, masaüstüne kaydettiğimiz klasörü yükleyelim.

![image](https://github.com/enyaselessar/Dymension-Rollapp/assets/108255403/98732b8b-72e3-43b7-bb95-a7ef1e7798b9)
#### Klasörü yükledikten sonra pull request yapalım ve pr linkini kopyalayalım.
![image](https://github.com/enyaselessar/Dymension-Rollapp/assets/108255403/dfaf69cd-f7ce-41b6-8be7-2900f094c3e0)

#### Bu işlemden sonra Discord kanalındaki #list-your-rollapp kanalına aşağıdaki yazıyı gönderin.
```
$pair <RollApp-ID>  ve altına alt mesaj oluşturup, pr oluşturtuğunuz githun linkini yazın
```

https://dymension.xyz/
https://portal.dymension.xyz/rollapp/enyas_1686868-1
