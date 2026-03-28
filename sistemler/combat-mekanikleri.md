# Combat Mekanikleri

<p>Combat sistemi, Nimloth’ta en üzerinde durulan ve tüm ayrıntıları hesaplanarak tasarlanmış bir yapıdır.</p>
<p>Rastgelelik minimumda tutulmuş, matematiksel doğruluk ve oyuncu becerisi ön planda olacak şekilde dizayn edilmiştir.</p>

<p>Bu sayfa, silah hasar hesaplamasından kritik vuruş mekaniklerine kadar tüm detayları içermektedir.</p>

<h1>Silah Hasarı Hesaplaması</h1>
<p>Hasar hesaplama süreci birkaç aşamada gerçekleşir. İlk adım silahın baz hasar değerinin belirlenmesidir.</p>

<p>Örneğin Katana için baz hasar aralığı <strong style="color: #410000;">9-11</strong>’dir.</p>
<p>Ortalama bir değer üzerinden ilerleyecek olursak <strong style="color: #410000;">10</strong> üzerinden örnek verebiliriz.</p>

<p>Hasar hesaplamasında kullanılan değişkenler şu şekildedir:</p>
<p><strong style="color: #410000;">Silahın baz hasarı -> </strong> Örnekte katana için 10 alınacaktır.</p>
<p><strong style="color: #410000;">Combat yeteneği -> </strong> Katana için Swordsmanship kullaınlacak. Yetenek 100 ise katsayı 1, yetenek 90 ise katsayı 0.9 alınır.</p>
<p><strong style="color: #410000;">Tactics yeteneği -> </strong> Yetenek 100 ise katsayı 1, yetenek 90 ise katsayı 0.9 alınır.</p>

<h1>İlk Hasar Katsayısı Hesaplama</h1>
<p>Oyuncunun <strong style="color: #410000;">Swordsmanship yeteneğinin ve Tactics yeteneğinin 100</strong>, silahın <strong style="color: #410000;">Katana ve hasarın 10</strong> olduğu üzerinden gidersek;</p>
<p>İlk katsayımız: <strong style="color: #410000;">10 * 1 * 1 = 10</strong> olacaktır</p>
<p>Bu değer critical hesaplanmadan önceki temel hasardır.</p>

<h1>Critical Vuruş Mekaniği</h1>
<p>Eğer saldırılan oyuncunun <strong style="color: #410000;">armor değeri 25’in altındaysa, critical katsayısı 2</strong> olarak alınır.</p>

<p>Armor değeri <strong style="color: #410000;">25 ve üzerindeyse</strong> critical şansı şu şekilde belirlenir:</p>
<p>Anatomy / 200 + <-1,1> → 4,6 arası</p>
<p>Armslore / 200  + <-1,1> → 4,6 arası</p>
<p>Toplamdan 18 çıkartılır.</p>

<p>Her iki birlikte değerlendirildiğinde:</p>
<p>10 vuruşta 1 ile 6 vuruşta 1 arası critical tetiklenir.</p>

<p><strong style="color: #410000;">Not: Yetenekler 100(hesaplamada 1000) olarak alınmıştır.</strong></p>

<h1>Critical Vuruş Hasar Katsayısı</h1>
<p><strong style="color: #410000;">Critical vuruş ihtimali denk geldiğinde</strong>, oyuncunun vuracağı critical miktarı şu şekilde hesaplanır:</p>

<p>Tactics / 40 + <-5,5> → 1.2-1.3 arası</p>
<p>Lumberjacking / 40 + <-5,5> → 1.2-1.3 arası</p>
<p>Örneğin sadece 100 Tactics olduğunu varsayarsak:</p>
<p>Silahın hasarı 10 → 12 - 13 aralığında bir değer olur.</p>

<h1>Magical Silah Katsayısı</h1>
<p>Critical hasar hesaplamasının ardından bir sonraki aşama, silahın magical (+) değerine göre hasar çarpanının uygulanmasıdır.</p>
<p>Magical seviye ve hasar katsayıları:</p>
<p>• <strong style="color: #410000;">+3 Silahlar için:	1.2</strong></p>
<p>• <strong style="color: #410000;">+6 Silahlar için: 1.4</strong></p>
<p>• <strong style="color: #410000;">+9 Silahlar için: 1.6</strong></p>
<p>• <strong style="color: #410000;">+12	Silahlar için: 1.8</strong></p>
<p>• <strong style="color: #410000;">+15	Silahlar için: 2.0</strong></p>

<p>Örneğimizdeki katananın <strong style="color: #410000;">+15</strong> olduğunu varsayarsak:</p>
<p>Critical gelmediğinde elde edilen hasar: <strong style="color: #410000;">10 Baz hasar * 2.0 dan 20</strong> olacaktır.</p>

<p>Critical vurduğunda, Critical katsayısından sonra (12-13 arası örneğinde):</p>
<p>• 12 * 2.0 = 24</p>
<p>• 13 * 2.0 = 26</p>

<p>Bu durumda sonuç:</p>

<p>Critical olmadan → <strong style="color: #410000;">20</strong></p>
<p>Critical ile → <strong style="color: #410000;">24 - 26</strong> arası bir hasar değeridir.</p>

<h1>Armor’a Göre Hasar Azaltımı</h1>
<p>Son aşamada vurulan hasar hedefin armor değerine göre azaltılır.</p>
<p>Armor ne kadar yüksek ise alınan hasar o kadar azalır.</p>
<p>Azalacak hasarın armora göre oranı 1/10 olarak düzenlenmiştir.</p>

<p>Örneğin rakibin armor değeri 85 ise:</p>
<p>+15 Katana ile Critical vurulmadığında elde edilen 20 hasar → 12’ye düşecektir.</p>
<p>Critical vurulduğunda elde edilen 24-26 hasar → 16-18 aralığına düşecektir.</p>

<h1>Parry Yeteneği ve Kalkan Kullanımı</h1>
<p>Parry yeteneğiniz bulunuyorsa ve hasar aldığınız sırada kalkan elinizdeyse, gelen hasarı karşılama şansı etkin hale gelir.</p>
<p>Bu durumda bonus aktif olursa oyuncunun defans katsayısı <strong style="color: #410000;">x2</strong> olarak hesaplanır.</p>

<p>Örneğin:</p>
<p>Armor değeri 85 olan bir oyuncunu normal şartlarda 8 hasar azaltır.</p>
<p>Parry bonusu devreye girdiğinde azaltılan hasar miktar 8 yerine 16 olur.</p>
<p>Bu sayede oyuncunun aldığı hasar önemli ölçüde düşer ve tank rolündeki karakterlerde kritik öneme sahiptir.</p>

<h1>Reactive Armor Etkisi</h1>
<p>Reactive Armor büyüsü aktifken iki farklı mekanizma çalışmaktadır:</p>
<h2>Hasarı Saldırana Yansıtma</h2>
<p>Hasar alan oyuncu bir büyü kalkanına sahiptir ve saldıran oyuncuya 2–3 arası hasar geri yansıtılır.</p>
<p>Bu hasar ek bir hesaplamaya tabi değildir ve saf hasar olarak vurulur.</p>

<h2>Alınan Hasarı Azaltma</h2>
<p>Reactive Armor’un ikinci ve daha güçlü etkisi, gelen hasarın armor hesaplamasından önce %30 oranında indirilmesidir.</p>
<p>Örnek olarak saldırılan silahı +15 Katana olarak varsayalım ve Critical vurmadığı hasarı alalım.</p>
<p>Bu durumda armor hesaplaması öncesinde baz hasar miktarımız 20'dir</p>
<p>Reactive Armor etkisi sonrası bu hasar %30 oranında azalacak ve 14 olarak hesaplanacaktır.</p>
<p>Ardından armor defansı devreye girer.</p>
<p>Oyuncunun armor değerinin 53 olduğunu varsayacak olursak 5 hasar armor tarafından bloklanır</p>
<p>Son durumda 14-5 den alınacak hasar 9 olacaktır.</p>
<p>Not: Reactive Armor büyüsünün etki süresi, büyüyü atan oyuncunun Magery, Inscription ve Evaluating Intel yeteneklerine göre değişiklik göstermektedir.</p>

<h1>Silaha Zehir Sürme</h1>
<p>Nimloth dünyasında silahlara zehir sürerek PvP ve PvM’de avantaj elde edebilirsiniz.</p>
<p>Zehir, rakibe her başarılı vuruşta ek hasar verir veya statü etkisi uygular. Ancak bu sistemin bazı kuralları ve gereksinimleri vardır.</p>

<h2>Çift El Silahlar ve Zehir Sürme Şartları</h2>
<p>• Çift el silahlara zehir sürebilmek için oyuncunun <strong style="color: #410000;">Magery yeteneğinin 25’in altında</strong> olması gerekmektedir.</p>
<p>• Tek el silahlarda böyle bir kısıtlama yoktur.</p>

<h2>Zehir Seviyeleri ve Gereken Poisoning Yeteneği</h2>
<p>Silaha uygulanacak poison seviyesi, oyuncunun Poisoning yeteneği ile orantılıdır.</p>
<table style="border-collapse: collapse; width: 100%; max-width: 600px; font-size: 14px;">
  <tr style="background-color: #A09884;">
    <th style="border: 1px solid #410000; color: #410000; padding: 8px; text-align: left;">Zehir Tipi</th>
    <th style="border: 1px solid #410000; color: #410000; padding: 8px; text-align: left;">Gerekli Poisoning</th>
  </tr>
  <tr style="background-color: #A9A08B;">
    <td style="border: 1px solid #410000; padding: 8px;">Deadly Poison</td>
    <td style="border: 1px solid #410000; padding: 8px;">80.0</td>
  </tr>
  <tr style="background-color: #A09884;">
    <td style="border: 1px solid #410000; padding: 8px;">Greater Poison</td>
    <td style="border: 1px solid #410000; padding: 8px;">70.0</td>
  </tr>
  <tr style="background-color: #A9A08B;">
    <td style="border: 1px solid #410000; padding: 8px;">Poison Potion</td>
    <td style="border: 1px solid #410000; padding: 8px;">50.0</td>
  </tr>
  <tr style="background-color: #A09884;">
    <td style="border: 1px solid #410000; padding: 8px;">Lesser Poison</td>
    <td style="border: 1px solid #410000; padding: 8px;">30.0</td>
  </tr>
</table>
<p></p>
<h2>Magical Silahlara Poison Sürme</h2>
<p>Magical silahlara zehir sürebilmek için ekstra olarak Armslore yeteneği gerekmektedir.</p>
<table style="border-collapse: collapse; width: 100%; max-width: 600px; font-size: 14px;">
  <tr style="background-color: #A09884;">
    <th style="border: 1px solid #410000; color: #410000; padding: 8px; text-align: left;">Silah Seviyesi</th>
    <th style="border: 1px solid #410000; color: #410000; padding: 8px; text-align: left;">Gerekli Armslore</th>
  </tr>
  <tr style="background-color: #A9A08B;">
    <td style="border: 1px solid #410000; padding: 8px;">+15 Silahlar</td>
    <td style="border: 1px solid #410000; padding: 8px;">60.0</td>
  </tr>
  <tr style="background-color: #A09884;">
    <td style="border: 1px solid #410000; padding: 8px;">+12 Silahlar</td>
    <td style="border: 1px solid #410000; padding: 8px;">50.0</td>
  </tr>
  <tr style="background-color: #A9A08B;">
    <td style="border: 1px solid #410000; padding: 8px;">+9 Silahlar</td>
    <td style="border: 1px solid #410000; padding: 8px;">40.0</td>
  </tr>
  <tr style="background-color: #A09884;">
    <td style="border: 1px solid #410000; padding: 8px;">+6 Silahlar</td>
    <td style="border: 1px solid #410000; padding: 8px;">30.0</td>
  </tr>
</table>
<p></p>

<p>+3 ve magical olmayan silahlar için ek Armslore gereksinimi bulunmamaktadır.</p>

<p>Not: Axe türü ve MF silahlarına(War Axe hariç) zehir sürülemez.</p>

<h1>Oil Cloth Kullanımı</h1>
<p><a href="https://uo-nimloth.net/wiki/esyalar/oil-cloth" style="color: #410000; font-weight: bold; text-decoration: underline; font-size: inherit;"> Oil Cloth</a>, silahların üzerindeki zehri temizlemek için kullanılan özel bir eşyadır.</p>
<p>Bu eşya sayesinde kendi silahınızdaki zehri silebildiğiniz gibi, başka bir oyuncunun elindeki silahın zehrini de temizleyebilirsiniz.</p>

<h2>Kullanım Şartları ve Mekanik</h2>
<p>• Oil Cloth, çantanızda olduğunda kullanılabilir.</p>
<p>• Oil Cloth uygulandığında 2 saniyelik bir işlem süresi başlar.</p>
<p>• İşlem tamamlandığında, hedeflenen silahın üzerindeki tüm zehir tamamen temizlenir.</p>

<h2>Kendi Silahınızdaki Zehri Silme</h2>
<p>• Elinizde tuttuğunuz silaha Oil Cloth uygularsanız 2 saniye sonra silahın üzerindeki zehir temizlenir.</p>
<p>• Bu işlem için herhangi ek bir gereksinim yoktur.</p>

<h2>Başkalarının Silahındaki Zehri Silme</h2>
<p>Oil Cloth aynı zamanda başka bir oyuncunun elindeki silahın üzerindeki zehri silmek için de kullanılabilir.</p>
<p>Bunun için:</p>
<p>• Oil Cloth uygulandığı anda hedef oyuncu 2 kare mesafeden fazla uzakta olmamalı,</p>
<p>• İşlemin tamamlanacağı 2 saniye sonunda da hedef oyuncu görünür durumda ve 2 kare mesafede olmalıdır.</p>
<p>Eğer bu koşullar sağlanırsa, hedef oyuncunun silahındaki zehir başarıyla temizlenir.</p>
<p>Temizleme işlemi başarıyla gerçekleştiğinde, hedef oyuncuya silahındaki zehrin temizlendiğine dair bilgilendirme mesajı gönderilir.</p>