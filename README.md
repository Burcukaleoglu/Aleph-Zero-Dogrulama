# Aleph-Zero-Dogrulama
Aleph-Zero-Dogrulam
https://twitter.com/uguryukselx10/status/1555790824088240128

Kurulum aşamasını Uğur paylaşmış zaten oraya girmiyorum.  

https://validators.alephzero.org/   yaptığımız başvurunun kabul edilmesi için 3 tane şart var. 


 Hesap ayarı ( Cüzdan adınızla node adınız aynı olsun) 
 https://test.azero.dev/#/accounts  siteye gidiyoruz ve node ile ilişkilendirmek istediğimiz hesabın sağ tarafındaki üç noktaya basıp set on-chain identity diyoruz.Sizde burada hesap görünmezse eğer polkadot cüzdanınıza girip hangi hesabınızı kullanmak istiyorsanız onun sağ tarafındaki üç noktaya tıklayıp her zincirde kullanıma izin ver diyerek siteyi yenileyin.  Gelen ekranda bizden twitter, mail, isim  gibi bilgiler istiyor. Girdiğiniz bilgiler profilinizde görünecek. İsim yazmak yeterli diğerleri size kalmış ben doldurdum.  

 

Düğüm doğrulama

 

İşaretli yere tıkladığınızda cüzdan adresini kopyalayabilirsiniz. 

https://faucet.test.azero.dev/   musluktan token alalım. 

Network kısmından staking sayfasına geliyoruz ve işaretlediğim accounts sekmesine tıklıyoruz. 


 

En sağdaki Stash tuşuna tıklayıp gelen sayfada aldığımız tokenleri bond işlemi yapalım. Fee için token ayırmayı unutmayın yoksa otomatik olarak maksimum miktarı seçiyor. En az 25k adet test azero tokeni  bond etmeniz gerekiyor yoksa hata alırsınız. 


 Node kurduğumuz sunucumuza giriş yapalım. 
Gireceğimiz komuttan sonra bir çıktı verecek o çıktıyı not almayı unutmayın. 

curl -H "Content-Type: application/json" -d '{"id":1, "jsonrpc":"2.0", "method": "author_rotateKeys"}' http://127.0.0.1:9933

 




 https://test.azero.dev/#/staking/actions 
 
Tekrardan sitemize dönüyoruz az önce bond işlemi yaptığımız  network-staking- accounts sayfasında sağ tarafta Session Key e tıklayalım.   
Açılan sayfada bizden 0x le başlayan bir key istiyor. Az önce girdiğimiz komut sonrası aldığımız çıktıdaki 0x le başlayan şifreyi buraya giriyoruz ve onaylıyoruz. 
 İşlem onaylandıktan sonra yine aynı sayfada işaretli olan validate tuşuna basıyoruz ve istediğimiz komisyon oranını yazarak onaylıyoruz. 
 

Bu işlemden sonra; 

https://test.azero.dev/#/staking

https://telemetry.azero.dev/#list/0x05d5279c52c484cc80396535a316add7d47b1c5b9e0398dd1f584149341460c5

İki sitede de adınızı göreceksiniz. 



Uyku sersemi bond işleminde eksik yapmışım.  Ben 24 k bond ettim ama sizin yapmanız gereken 25k. Fotoğraflara bakıp böyle yapan olursa hata alacaktır. Şu şekilde çözülür; validate tuşunun sağ tarafındaki üç noktaya tıklayın ve en üstteki bond more funds seçeneği ile 25k ya tamamlarsanız eğer validate işlemini de rahatlıkla yaparsınız. 
