# Aleph-Zero-Dogrulama
Aleph-Zero-Dogrulama
https://twitter.com/uguryukselx10/status/1555790824088240128
```
Kurulum aşamasını Uğur paylaşmış zaten oraya girmiyorum  
```
https://validators.alephzero.org/   yaptığımız başvurunun kabul edilmesi için 3 tane şart var. 


 Hesap ayarı ( Cüzdan adınızla node adınız aynı olsun) 
 https://test.azero.dev/#/accounts  siteye gidiyoruz ve node ile ilişkilendirmek istediğimiz hesabın sağ tarafındaki üç noktaya basıp set on-chain identity diyoruz.Sizde burada hesap görünmezse eğer polkadot cüzdanınıza girip hangi hesabınızı kullanmak istiyorsanız onun sağ tarafındaki üç noktaya tıklayıp her zincirde kullanıma izin ver diyerek siteyi yenileyin.  Gelen ekranda bizden twitter, mail, isim  gibi bilgiler istiyor. Girdiğiniz bilgiler profilinizde görünecek. İsim yazmak yeterli diğerleri size kalmış ben doldurdum.  
![a1](https://user-images.githubusercontent.com/107887745/199969132-71d6ba8c-39ef-4498-8576-3b86f828c4e6.jpg)

 

1 - Düğüm doğrulama
![a2](https://user-images.githubusercontent.com/107887745/199969231-cf1ef079-1861-4c63-b134-8b59f21ec171.jpg)

 

İşaretli yere tıkladığınızda cüzdan adresini kopyalayabilirsiniz. 

https://faucet.test.azero.dev/   musluktan token alalım. 

Network kısmından staking sayfasına geliyoruz ve işaretlediğim accounts sekmesine tıklıyoruz. 
![a3](https://user-images.githubusercontent.com/107887745/199969458-4a61a859-b106-439a-b43e-337b5db89fa8.png)


 

En sağdaki Stash tuşuna tıklayıp gelen sayfada aldığımız tokenleri bond işlemi yapalım. Fee için token ayırmayı unutmayın yoksa otomatik olarak maksimum miktarı seçiyor. En az 25k adet test azero tokeni  bond etmeniz gerekiyor yoksa hata alırsınız. 


 Node kurduğumuz sunucumuza giriş yapalım. 
Gireceğimiz komuttan sonra bir çıktı verecek o çıktıyı not almayı unutmayın. 

curl -H "Content-Type: application/json" -d '{"id":1, "jsonrpc":"2.0", "method": "author_rotateKeys"}' http://127.0.0.1:9933

 




 https://test.azero.dev/#/staking/actions 
 ![a4](https://user-images.githubusercontent.com/107887745/199969538-06737bd3-328d-4155-8ffa-6ff1a82c7058.png)

Tekrardan sitemize dönüyoruz az önce bond işlemi yaptığımız  network-staking- accounts sayfasında sağ tarafta Session Key e tıklayalım.   
Açılan sayfada bizden 0x le başlayan bir key istiyor. Az önce girdiğimiz komut sonrası aldığımız çıktıdaki 0x le başlayan şifreyi buraya giriyoruz ve onaylıyoruz. 
 İşlem onaylandıktan sonra yine aynı sayfada işaretli olan validate tuşuna basıyoruz ve istediğimiz komisyon oranını yazarak onaylıyoruz. 
 ![a5](https://user-images.githubusercontent.com/107887745/199969713-4cad5d36-e208-4595-bedd-3ccf5a0a7bb6.png)


Bu işlemden sonra; 

https://test.azero.dev/#/staking

https://telemetry.azero.dev/#list/0x05d5279c52c484cc80396535a316add7d47b1c5b9e0398dd1f584149341460c5

İki sitede de adınızı göreceksiniz. 



Uyku sersemi bond işleminde eksik yapmışım.  Ben 24 k bond ettim ama sizin yapmanız gereken 25k. Fotoğraflara bakıp böyle yapan olursa hata alacaktır. Şu şekilde çözülür; validate tuşunun sağ tarafındaki üç noktaya tıklayın ve en üstteki bond more funds seçeneği ile 25k ya tamamlarsanız eğer validate işlemini de rahatlıkla yaparsınız. 
