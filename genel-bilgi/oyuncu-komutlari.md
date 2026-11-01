# Oyuncu Komutları

Nimloth’ta çeşitli menülere ulaşmak, karakterinizi düzenlemek ve oyun içindeki işlemleri gerçekleştirmek için komutları kullanabilirsiniz.

Oyun içindeki komut listesine <mark style="color:red;">**Help → Yardım → Komutlar**</mark> yoluyla ulaşabilirsiniz.

<figure><img src="../.gitbook/assets/image (427).png" alt=""><figcaption></figcaption></figure>

## Karakter Düzenleme

| Komut         | Açıklama                                                                            |
| ------------- | ----------------------------------------------------------------------------------- |
| `.stat`       | Strength, Dexterity ve Intelligence değerlerinizi düzenleyebileceğiniz menüyü açar. |
| `.skilldusur` | Seçtiğiniz yeteneği düşürmek için kullanılan menüyü açar.                           |

## Genel Komutlar

| Komut        | Açıklama                                                                               |
| ------------ | -------------------------------------------------------------------------------------- |
| `.where`     | Bulunduğunuz konum ve koordinatlar hakkında bilgi verir.                               |
| `.hungry`    | Karakterinizin açlık durumunu gösterir.                                                |
| `.newplayer` | Yeni oyuncular için hazırlanan başlangıç bilgilendirme ekranını açar.                  |
| `.wiki`      | Hedef seçmenizi ister. Seçtiğiniz eşya veya karakter için tanımlı wiki sayfasını açar. |
| `.top10`     | Farklı alanlardaki oyuncu sıralamalarını görüntüler.                                   |
| `.ailem`     | Üyesi olduğunuz aileyle ilgili bilgileri ve işlemleri görüntüler.                      |
| `.gc mesaj`  | Guild üyelerine mesaj gönderir. Örnek: `.gc Merhaba`                                   |

## Üretim ve Malzeme Takibi

| Komut              | Açıklama                                                                                    |
| ------------------ | ------------------------------------------------------------------------------------------- |
| `.makelast miktar` | Son ürettiğiniz eşyayı belirtilen miktarda tekrar üretmeyi başlatır. Örnek: `.makelast 100` |
| `.ores`            | Çantanızdaki ore miktarlarını görüntüler.                                                   |
| `.ingots`          | Çantanızdaki ingot miktarlarını görüntüler.                                                 |
| `.regs`            | Çantanızdaki büyü malzemelerinin miktarlarını görüntüler.                                   |
| `.potions`         | Çantanızdaki iksir miktarlarını görüntüler.                                                 |

`.makelast` komutunda <mark style="color:red;">**1–1500**</mark> arasında miktar belirleyebilirsiniz. Üretim için gerekli malzemeler, araçlar ve çalışma koşulları sağlanmalıdır. Tekrarlı üretimi <mark style="color:red;">**Tab tuşuyla savaş moduna geçerek**</mark> iptal edebilirsiniz.

### Savaş Komutları

| Komut     | Açıklama                                                                                                                                                                                                                                                               |
| --------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `.stun`   | Yumrukla yapılan saldırılarda kullanılan [<mark style="color:red;">**Stun bonusunu**</mark>](https://nimloth-uo.gitbook.io/wiki/sistemler/bonuslar#stun) açar veya kapatır. En az <mark style="color:red;">**98.0 Wrestling ve 98.0 Tactics**</mark> gerekir.          |
| `.disarm` | Rakibin elindeki ekipmanı çıkarmaya yönelik [<mark style="color:red;">**Disarm bonusunu**</mark>](https://nimloth-uo.gitbook.io/wiki/sistemler/bonuslar#disarm) açar veya kapatır. En az <mark style="color:red;">**80.0 Wrestling ve 80.0 Arms Lore**</mark> gerekir. |

Stun ve Disarm aynı anda açık tutulamaz. Birini etkinleştirdiğinizde diğeri kapanır.

## Canlanma ve Achievement Takibi

| Komut   | Açıklama                                                                                                                                                                                                                                                                   |
| ------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `.res`  | Ölüyken [<mark style="color:red;">**canlanma seçenekleri**</mark>](https://nimloth-uo.gitbook.io/wiki/sistemler/resurrect-options) menüsünü açar. Hayattayken mevcut Resurrection Stone miktarınızı gösterir.                                                              |
| `.achi` | [<mark style="color:red;">**Achievement**</mark>](https://nimloth-uo.gitbook.io/wiki/sistemler/achievement-sistemi) takip penceresini açar. [<mark style="color:red;">**Premium üyelik**</mark>](https://nimloth-uo.gitbook.io/wiki/sistemler/premium-sistemi) gerektirir. |

`.achi` penceresinden takip ettiğiniz başarımları görüntüleyebilir ve takip önerilerine ulaşabilirsiniz. Aynı anda en fazla <mark style="color:red;">**3 başarım**</mark> takip edebilirsiniz.

## Etkinlik Komutları

| Komut       | Açıklama                                                      |
| ----------- | ------------------------------------------------------------- |
| `.etkinlik` | Katılıma açık bir etkinlik varsa katılım işlemini başlatır.   |
| `.bomba`    | Bomberman etkinliğinde bulunduğunuz konuma bomba yerleştirir. |
| `.skor`     | Team Deathmatch etkinliği sırasında skor tablosunu açar.      |

## NPC’lerle Kullanılan Komutlar

Bu komutlar başına nokta konmadan, ilgili NPC’nin yakınında söylenir.

| Komut               | Açıklama                                                                                                                                                  |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `hesap` / `hesabim` | Banker yanında [<mark style="color:red;">**banka hesap sistemi**</mark>](https://nimloth-uo.gitbook.io/wiki/sistemler/banka-hesap-sistemi) menüsünü açar. |
| `gorev`             | Görev veren NPC’lerde Craft, Gatherer, Tamer veya Hunter görev işlemlerine ulaşmanızı sağlar.                                                             |

## Ev Komutları

Ev komutları evin içindeyken, başına nokta konmadan kullanılır. Yapabileceğiniz işlemler evdeki sahiplik, ortaklık veya dostluk yetkinize bağlıdır.

| Komut                     | Açıklama                                                       | Kullanabilenler                |
| ------------------------- | -------------------------------------------------------------- | ------------------------------ |
| `house help` / `komutlar` | Ev komutları yardım ekranını açar.                             | Ev sahibi, ortaklar ve dostlar |
| `res` / `resurrect`       | Evde canlanma işlemini başlatır.                               | Ev sahibi, ortaklar ve dostlar |
| `bank`                    | Bankanızı açma işlemini başlatır.                              | Ev sahibi, ortaklar ve dostlar |
| `I ban thee`              | Seçtiğiniz oyuncuyu evden dışarı çıkarır.                      | Ev sahibi, ortaklar ve dostlar |
| `lock`                    | Seçtiğiniz eşyayı eve sabitler.                                | Ev sahibi ve ortaklar          |
| `release`                 | Seçtiğiniz eşyanın sabitliğini kaldırır.                       | Ev sahibi ve ortaklar          |
| `strongbox`               | Eve size ait bir kişisel kasa yerleştirir.                     | Ev sahibi ve ortaklar          |
| `remove`                  | Size ait kişisel kasayı kaldırmak için hedef seçtirir.         | Ev sahibi ve ortaklar          |
| `secure`                  | Uygun bir eşyayı güvenli hâle getirir.                         | Ev sahibi                      |
| `unsecure`                | Eşyanın güvenli durumunu kaldırır.                             | Ev sahibi                      |
| `item up`                 | Sabit eşyanın yüksekliğini artırır.                            | Ev sahibi ve ortaklar          |
| `item down`               | Sabit eşyanın yüksekliğini azaltır.                            | Ev sahibi ve ortaklar          |
| `flip`                    | Uygun bir sabit eşyanın yönünü değiştirir.                     | Ev sahibi ve ortaklar          |
| `leave` / `leave house`   | Evden ayrılmanızı sağlar. İşlem sırasında hareket edemezsiniz. | Herkes                         |

`leave` komutu <mark style="color:red;">**8 saniye**</mark> sonra sizi evden çıkarır ve <mark style="color:red;">**3 dakikada bir**</mark> kullanılabilir.

Bazı ev komutlarının uzun biçimleri de kullanılabilir:

| Kısa komut  | Uzun biçimi                   |
| ----------- | ----------------------------- |
| `lock`      | `I wish to lock this down`    |
| `release`   | `I wish to release this down` |
| `strongbox` | `I wish to place a strongbox` |
| `remove`    | `I wish to remove this`       |
| `secure`    | `I wish to secure this`       |
| `unsecure`  | `I wish to unsecure this`     |

### Player Vendor Komutları

Bu komutlar player vendorun yakınında, başına nokta konmadan söylenir. Vendor yönetimiyle ilgili işlemleri vendorun sahibi yapabilir.

| Komut              | Açıklama                                                                        |
| ------------------ | ------------------------------------------------------------------------------- |
| `bilgi` / `yardim` | Vendorun yardım ekranını açar.                                                  |
| `durum`            | Vendorun çalışma kasasındaki para ve kalan çalışma süresi hakkında bilgi verir. |
| `kasa`             | Vendorun çalışma kasasına para yatırma işlemini başlatır.                       |
| `fiyat miktar`     | Satılacak eşyaya fiyat belirlemek için kullanılır. Örnek: `fiyat 10000`         |
| `hasilat`          | Satışlardan elde edilen hasılatı tahsil etmenizi sağlar.                        |
| `kontrat`          | Vendorun durumunu ve kaldırma işlemini içeren menüyü açar.                      |
| `lokasyon`         | Vendorun ev içindeki konumunu değiştirmenizi sağlar.                            |
| `buy` / `satin al` | Vendordaki fiyatlandırılmış eşyalardan satın almak için kullanılır.             |
