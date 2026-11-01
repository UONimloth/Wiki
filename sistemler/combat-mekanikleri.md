# Combat Mekanikleri

## Combat Mekanikleri

Combat sistemi, Nimloth’ta en üzerinde durulan ve tüm ayrıntıları hesaplanarak tasarlanmış bir yapıdır.

Rastgelelik minimumda tutulmuş, matematiksel doğruluk ve oyuncu becerisi ön planda olacak şekilde dizayn edilmiştir.

Bu sayfa, silah hasar hesaplamasından kritik vuruş mekaniklerine kadar tüm detayları içermektedir.

## Silah Hasarı Hesaplaması

Hasar hesaplama süreci birkaç aşamada gerçekleşir. İlk adım silahın baz hasar değerinin belirlenmesidir.

Örneğin Katana için baz hasar aralığı <mark style="color:red;">**9-13**</mark>’dir.

Örnek bir değer üzerinden ilerleyecek olursak <mark style="color:red;">**10**</mark> üzerinden örnek verebiliriz.

Hasar hesaplamasında kullanılan değişkenler şu şekildedir:

<mark style="color:red;">**Silahın baz hasarı ->**</mark> Örnekte katana için 10 alınacaktır.

<mark style="color:red;">**Combat yeteneği ->**</mark> Katana için Swordsmanship kullaınlacak. Yetenek 100 ise katsayı 1, yetenek 90 ise katsayı 0.9 alınır.

<mark style="color:red;">**Tactics yeteneği ->**</mark> Yetenek 100 ise katsayı 1, yetenek 90 ise katsayı 0.9 alınır.

## İlk Hasar Katsayısı Hesaplama

Oyuncunun <mark style="color:red;">**Swordsmanship yeteneğinin ve Tactics yeteneğinin 100**</mark>, silahın <mark style="color:red;">**Katana ve hasarın 10**</mark> olduğu üzerinden gidersek;

İlk katsayımız: <mark style="color:red;">**10 \* (1 + 1) / 2 = 10**</mark> olacaktır

Bu değer critical hesaplanmadan önceki temel hasardır.

Temel hasar, silahın baz hasarı ile Combat ve Tactics yeteneklerinden elde edilen ortalama katsayının çarpılmasıyla hesaplanır.

## Critical Vuruş Mekaniği

Eğer saldırılan oyuncunun <mark style="color:red;">**armor değeri 25’in altındaysa, critical katsayısı 2**</mark> olarak alınır.

Armor değeri <mark style="color:red;">**25 ve üzerindeyse**</mark> critical şansı şu şekilde belirlenir:

Anatomy / 200 + <-1,1> → 4,6 arası

Armslore / 200 + <-1,1> → 4,6 arası

Toplamdan 18 çıkartılır.

Her iki birlikte değerlendirildiğinde:

10 vuruşta 1 ile 6 vuruşta 1 arası critical tetiklenir.

<mark style="color:red;">**Not: Yetenekler 100(hesaplamada 1000) olarak alınmıştır.**</mark>

## Critical Vuruş Hasar Katsayısı

Kritik vuruşun hasar artışını <mark style="color:red;">**Tactics**</mark> ve <mark style="color:red;">**Lumberjacking**</mark> belirler. Her yeteneğin katkısı ayrı hesaplanır ve temel katsayıya eklenir.

Yalnızca 100 Tactics bulunduğunda kritik hasar katsayısı <mark style="color:red;">**1,2–1,3**</mark>, hem Tactics hem Lumberjacking 100 olduğunda <mark style="color:red;">**1,4–1,6**</mark> arasında olur.

Hedef oyuncunun armor değeri 25’in altındaysa bu hesap yerine doğrudan **2 kat hasar katsayısı** kullanılır.

Örneğin sadece 100 Tactics olduğunu varsayarsak:

Silahın hasarı 10 → 12 - 13 aralığında bir değer olur.

## Magical Silah Katsayısı

Critical hasar hesaplamasının ardından bir sonraki aşama, silahın magical (+) değerine göre hasar çarpanının uygulanmasıdır.

Magical seviye ve hasar katsayıları:

<mark style="color:red;">•</mark> <mark style="color:red;"></mark><mark style="color:red;">**+3 Silahlar için: 1.2**</mark>

<mark style="color:red;">•</mark> <mark style="color:red;"></mark><mark style="color:red;">**+6 Silahlar için: 1.4**</mark>

<mark style="color:red;">•</mark> <mark style="color:red;"></mark><mark style="color:red;">**+9 Silahlar için: 1.6**</mark>

<mark style="color:red;">•</mark> <mark style="color:red;"></mark><mark style="color:red;">**+12 Silahlar için: 1.8**</mark>

<mark style="color:red;">•</mark> <mark style="color:red;"></mark><mark style="color:red;">**+15 Silahlar için: 2.0**</mark>

Örneğimizdeki katananın <mark style="color:red;">**+15**</mark> olduğunu varsayarsak:

Critical gelmediğinde elde edilen hasar: <mark style="color:red;">**10 Baz hasar \* 2.0 dan 20**</mark> olacaktır.

Critical vurduğunda, Critical katsayısından sonra (12-13 arası örneğinde):

• 12 \* 2.0 = 24

• 13 \* 2.0 = 26

Bu durumda sonuç:

Critical olmadan → <mark style="color:red;">**20**</mark>

Critical ile → <mark style="color:red;">**24 - 26**</mark> arası bir hasar değeridir.

## Armor’a Göre Hasar Azaltımı

Son aşamada vurulan hasar hedefin armor değerine göre azaltılır.

Armor ne kadar yüksek ise alınan hasar o kadar azalır.

Azalacak hasarın armora göre oranı 1/10 olarak düzenlenmiştir.

Armor değeri 24 veya altındaysa bu hesaplamadan hasar azaltımı sağlanmaz.

Örneğin rakibin armor değeri 85 ise:

+15 Katana ile Critical vurulmadığında elde edilen 20 hasar → 12’ye düşecektir.

Critical vurulduğunda elde edilen 24-26 hasar → 16-18 aralığına düşecektir.

## Parry Yeteneği ve Kalkan Kullanımı

Kalkan kullanırken Parrying yeteneğiniz <mark style="color:red;">**90.0’ın üzerindeyse**</mark> ek savunma kazanırsınız. Başarılı parry gerçekleştiğinde armor üzerinden hesaplanan hasar azaltımı <mark style="color:red;">**2 katına**</mark> çıkar. Parry gerçekleşmeyen vuruşlarda da bu azaltım <mark style="color:red;">**1,6 kat**</mark> olarak uygulanır.

Örneğin:

Armor değeri 85 olan bir oyuncunu normal şartlarda 8 hasar azaltır.

Parry bonusu devreye girdiğinde azaltılan hasar miktar 8 yerine 16 olur.

Bu sayede oyuncunun aldığı hasar önemli ölçüde düşer ve tank rolündeki karakterlerde kritik öneme sahiptir.

## Reactive Armor Etkisi

Reactive Armor büyüsü aktifken iki farklı mekanizma çalışmaktadır:

### Hasarı Saldırana Yansıtma

Hasar alan oyuncu bir büyü kalkanına sahiptir ve saldıran oyuncuya <mark style="color:red;">**1–2 arası**</mark> hasar geri yansıtılır.

Bu hasar ek bir hesaplamaya tabi değildir ve saf hasar olarak vurulur.

### Alınan Hasarı Azaltma

Reactive Armor’un ikinci ve daha güçlü etkisi, gelen hasarın armor hesaplamasından önce <mark style="color:red;">**%30 oranında**</mark> indirilmesidir.

Örnek olarak saldırılan silahı +15 Katana olarak varsayalım ve Critical vurmadığı hasarı alalım.

Bu durumda armor hesaplaması öncesinde baz hasar miktarımız 20'dir

Reactive Armor etkisi sonrası bu hasar %30 oranında azalacak ve 14 olarak hesaplanacaktır.

Ardından armor defansı devreye girer.

Oyuncunun armor değerinin 53 olduğunu varsayacak olursak 5 hasar armor tarafından bloklanır

Son durumda 14-5 den alınacak hasar 9 olacaktır.

<mark style="color:red;">**Not: Reactive Armor büyüsünün etki süresi, büyüyü atan oyuncunun Magery, Inscription ve Evaluating Intel yeteneklerine göre değişiklik göstermektedir.**</mark>

## Silaha Zehir Sürme

Nimloth dünyasında silahlara zehir sürerek PvP ve PvM’de avantaj elde edebilirsiniz.

Zehir, rakibe her başarılı vuruşta ek hasar verir veya statü etkisi uygular. Ancak bu sistemin bazı kuralları ve gereksinimleri vardır.

### Çift El Silahlar ve Zehir Sürme Şartları

Uygun çift el silahlara zehir sürebilmek için <mark style="color:red;">**Magery en fazla 25.0**</mark><mark style="color:red;">,</mark> <mark style="color:red;"></mark><mark style="color:red;">**Evaluating Intelligence ise 0**</mark> olmalıdır. Bu koşulları sağlamayan bir karakter zehirli çift el silah kuşandığında silahın zehri kaldırılır.

Tek el silahlarda böyle bir kısıtlama yoktur.

### Zehir Seviyeleri ve Gereken Poisoning Yeteneği

Silaha uygulanacak poison seviyesi, oyuncunun Poisoning yeteneği ile orantılıdır.

| Zehir Tipi     | Gerekli Poisoning |
| -------------- | ----------------- |
| Deadly Poison  | 80.0              |
| Greater Poison | 70.0              |
| Poison Potion  | 50.0              |
| Lesser Poison  | 30.0              |

### Magical Silahlara Poison Sürme

Magical silahlara zehir sürebilmek için ekstra olarak Armslore yeteneği gerekmektedir.

| Silah Seviyesi | Gerekli Armslore |
| -------------- | ---------------- |
| +15 Silahlar   | 60.0             |
| +12 Silahlar   | 50.0             |
| +9 Silahlar    | 40.0             |
| +6 Silahlar    | 20.0             |

+3 ve magical olmayan silahlar için ek Armslore gereksinimi bulunmamaktadır.

Magical olmayan silahlara yalnızca <mark style="color:red;">**Lesser Poison**</mark> sürülebilir.

Not: Axe türü ve MF silahlarına(War Axe hariç) zehir sürülemez.

## Oil Cloth Kullanımı

[<mark style="color:red;">**Oil Cloth**</mark>](https://nimloth-uo.gitbook.io/wiki/esyalar/uretimtoplayici/oil-cloth), silahların üzerindeki zehri temizlemek için kullanılan özel bir eşyadır.

Bu eşya sayesinde kendi silahınızdaki zehri silebildiğiniz gibi, başka bir oyuncunun elindeki silahın zehrini de temizleyebilirsiniz.

Oil Cloth,kendi çantanızdaki veya elinizdeki zehirli silahlarda kullanılabilir. Başka oyuncularda ise silahın oyuncunun elinde olması gerekir.

Başarılı temizleme işleminde <mark style="color:red;">**1 Oil Cloth tüketilir**</mark>. Yeni bir temizleme işlemi başlatmak için <mark style="color:red;">**5 saniye**</mark> beklenir. İki saniyelik işlem sırasında hasar alırsanız temizleme iptal olur.

### Kullanım Şartları ve Mekanik

• Oil Cloth, çantanızda olduğunda kullanılabilir.

• Oil Cloth uygulandığında 2 saniyelik bir işlem süresi başlar.

• İşlem tamamlandığında, hedeflenen silahın üzerindeki tüm zehir tamamen temizlenir.

### Kendi Silahınızdaki Zehri Silme

• Elinizde tuttuğunuz silaha Oil Cloth uygularsanız 2 saniye sonra silahın üzerindeki zehir temizlenir.

• Bu işlem için herhangi ek bir gereksinim yoktur.

### Başkalarının Silahındaki Zehri Silme

Oil Cloth aynı zamanda başka bir oyuncunun elindeki silahın üzerindeki zehri silmek için de kullanılabilir.

Bunun için:

• Oil Cloth uygulandığı anda hedef oyuncu 2 kare mesafeden fazla uzakta olmamalı,

• İşlemin tamamlanacağı 2 saniye sonunda da hedef oyuncu görünür durumda ve 2 kare mesafede olmalıdır.

Eğer bu koşullar sağlanırsa, hedef oyuncunun silahındaki zehir başarıyla temizlenir.

Temizleme işlemi başarıyla gerçekleştiğinde, hedef oyuncuya silahındaki zehrin temizlendiğine dair bilgilendirme mesajı gönderilir.
