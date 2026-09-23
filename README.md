# Cep Langırtı

Telefonda oynanan langırt (kicker) oyunu. Tek bir `index.html` dosyasından oluşur; kurulum, kütüphane ya da derleme adımı yoktur.

## Nasıl oynanır

İki mod var: **Bilgisayara karşı** (mavi takım sensin, kırmızıyı bilgisayar oynar) ve **2 kişi** (aynı telefonda arkadaşınla). Seçtiğin gol sayısına (3, 5 ya da 7) ilk ulaşan maçı kazanır.

| Kontrol | Ne yapar |
| --- | --- |
| **▲ / ▼** (sol başparmak) | Aktif çubuğu (pirinç renkte parlayan çubuk) yukarı / aşağı kaydırır. Parmağını kaldırmadan ▲ ile ▼ arasında kaydırabilirsin. |
| **ŞUT** (sağ başparmak), dokun | Aktif çubuğun adamları hızlıca döner ve topa vurur. |
| **ŞUT**, basılı tut | Adamlar geriye yatar ve güç toplar (tuşun çevresindeki halka dolar). Bıraktığında daha sert vurur. |
| Vururken ▲/▼ | Kayan çubuk sürtünmeyle topa yan hız verir, top çapraz gider. |
| Ayağın kenarıyla vurmak | Ayak yuvarlak olduğu için top açılı seker. |
| Topuk | Top adamının arkasında kaldıysa ŞUT'a basılı tut: adam geriye yatarken topu arkaya iter. |
| **SÜPER** (ŞUT'un üstünde) | Göstergen dolunca süper şutu hazırlar; bir sonraki vuruşun süper şut olur (aşağıya bak). |

### Aktif çubuk

İsteğe bağlı bir özelliktir ve açık gelir. Menüdeki **Aktif çubuk** anahtarından ya da moladaki **Aktif çubuk** düğmesinden kapatabilirsin; seçimin hatırlanır.

- **Açık:** Yalnızca topa en yakın çubuk kayar ve vurur (ayrıntılar aşağıda).
- **Kapalı:** Bütün çubukların birlikte kayar ve birlikte vurur. Her çubuk kendi yol aralığının aynı oranında kayar, böylece çubuklar birbirinden kopmaz. Maç ortasında kapatırsan çubuklar yumuşakça aynı hizaya gelir. Bu modda kaleci zaten elinle birlikte hareket ettiği için otomatik kaleci devre dışıdır.
- 2 kişilik modda ayar iki oyuncuya da uygulanır. Bilgisayar her zaman aktif çubukla oynar.

Açıkken her an yalnızca bir çubuğunu kontrol edersin: topa en yakın ve topu önüne alabilecek çubuğu. Top başka bir çubuğun bölgesine geçince kontrol de kendiliğinden o çubuğa geçer. Diğer çubukların, bıraktığın yerde kalır.

- Top adamlarının arkasındaysa arkadaki çubuk için ek mesafe sayılır. Bu yüzden kontrol, topu ileri vurabilecek çubukta kalır.
- Top hızla kendi kalene geliyorsa kontrol, topun henüz geçmediği ilk çubuğa verilir.
- Kendi pasın ya da şutun ileri giderken kontrol, topun varacağı sıradaki çubuğuna geçer. Böylece o çubuğu top gelmeden hizalayabilirsin.
- Kontrol yalnızca güç toplarken ve vuruşun topa değebildiği kısa anda kilitli kalır. Adamlar topun üstüne kalkar kalkmaz kontrol sıradaki çubuğa geçebilir; vuran çubuk kendi kendine dikey konuma döner.
- Yeni çubuk açıkça daha uygunsa kontrol hemen geçer. Top iki çubuğun tam ortasında duruyorsa, titremesin diye kısa bir süre (0,06 sn) beklenir.
- Top yavaşlarken kontrolün iki çubuk arasında gidip gelmemesi için hız eşiklerinin açılma ve kapanma değerleri farklıdır: ileri pas 700 mm/s'de başlar, 350 mm/s'de biter.
- Bilgisayar da aynı kuralla oynar: o da aynı anda tek çubuğunu yönetir.

### Otomatik kaleci

Kontrol başka bir çubuktayken kalecin topu kendiliğinden izler. Böylece sert bir şutta kontrol kaleciye geçtiğinde kaleci boş kalenin kenarında beklemiyor olur. Yardım bilerek sınırlı tutuldu:

- Topu 0,25 saniye gecikmeyle görür, topun gideceği yeri tahmin etmez.
- Senin el hızının %45'iyle kayar.
- Kale ağzının dışına çıkmaz. Topu yalnızca kısmen izler: top şut menzilindeyken yaklaşık üçte iki oranında, uzaktayken daha az. Bu yüzden köşeler açık kalır.
- Kontrol kaleciye geçtiği anda kaleciyi yine sen oynarsın.

Açık gelir; kapatmak için menüdeki **Otomatik kaleci** anahtarını ya da moladaki **Oto kaleci** düğmesini kullan. Yalnızca aktif çubuk açıkken çalışır. Seçimin hatırlanır. Bilgisayara karşı modda yalnızca senin takımına, 2 kişilik modda iki takıma da uygulanır.

### Süper şut

Her takımın bir süper şut göstergesi vardır. Gösterge top oyundayken 40 saniyede dolar; gol yiyen takımın göstergesine ayrıca %30 eklenir.

- **Hazırlama:** Gösterge dolunca **SÜPER** tuşu turuncu parlar ve skor tabelasında takımın yanındaki şimşek yanar. Tuşa basınca süper şut hazırlanır: ŞUT tuşu da turuncu çerçeve alır. Dolmadan basarsan bir şey olmaz.
- **Ateşleme:** Hazırlanan süper, bir sonraki gerçek ileri vuruşunda ateşlenir. Topuk itişi ya da yana giden vuruş onu harcamaz. Kullanınca gösterge sıfırlanır.
- **Etkisi:** Top normal şutun yaklaşık 1,5 katı hızla (en az 3,8 m/s) kaymadan gider. Rakibin defans, orta saha ve forvet adamlarının içinden geçer; geçtiği adamlar bir anlığına soluklaşır. Turuncu iz ve parıltı bırakır, gol olursa "Süper gol!" yazar.
- **Sınırları:** Kaleci süper şutu durdurabilir; kaleci dokunduğu an süper biter. Duvardan sekebilir. Hızı 1,5 m/s'nin altına düşünce ya da 1,6 saniye sonra normal topa döner.
- **Bilgisayar:** Aynı göstergeyle oynar ve süperini forvetiyle vururken kullanır. İki kişilik modda iki oyuncunun da ayrı göstergesi ve SÜPER tuşu vardır.

Menüdeki **Süper şut** anahtarıyla kapatılabilir; açık gelir ve seçimin hatırlanır. Kapalıyken tuşlar ve göstergeler gizlenir.

Simülasyonda gösterge 40 saniyede dolarken gollerin yaklaşık %30'u süper şuttan geldi. 22 saniyelik dolumla bu oran yarıyı geçiyordu ve oyun göstergeye bağlı kalıyordu.

### 2 kişi (aynı telefon)

Telefonu yatay olarak ikinizin arasına koyun. Mavi oyuncu sol uçta, kırmızı oyuncu sağ uçta oturur; herkesin kalesi kendi tarafındadır.

- Her uçta o oyuncuya ait bir tuş sütunu vardır: ▲, ŞUT ve ▼. Tuşlar takım renginde, ŞUT yazısı da o oyuncuya dönüktür.
- Tuşlar ekranın kenarı boyunca dizildiği için, telefonu ister karşılıklı ister yan yana tutun, basılan ok çubuğun kaydığı yönü gösterir.
- İki oyuncu aynı anda basabilir; ekran birden fazla parmağı ayrı ayrı izler.
- İki taraf da "topa en yakın çubuk" kuralıyla oynar; her takımın aktif çubuğu kendi renginde parlar.
- Otomatik kaleci açıksa iki takıma birden uygulanır.

Klavyeyle 2 kişi oynamak için mavi `W S` ve `Boşluk` (ya da `F`), kırmızı `↑ ↓` ve `Enter` (ya da `L`) tuşlarını kullanır. Süper şut mavi için `E`, kırmızı için `O` ya da sağ `Shift`.

Bilgisayara karşı modda klavyeyle de oynanır: `↑ ↓` ya da `W S` aktif çubuğu kaydırır, `Boşluk` şut çeker, `E` ya da `Q` süper şutu hazırlar. İki modda da `P` ya da `Esc` molaya alır.

Oyun yatay ekran için tasarlandı. Telefon dik tutulursa sahne kendiliğinden 90° döner; telefonu yan çevirmen yeterli.

## Telefonda açmak

- **GitHub Pages:** Depo ayarlarında *Settings → Pages* bölümünden bu dalı ve kök klasörü (`/`) seç. Verilen adresi telefonda aç.
- **Yerel ağ:** Bilgisayarda depo klasöründe `npx http-server -p 8080` çalıştır, telefondan aynı Wi-Fi üzerinden `http://<bilgisayarın-IP-adresi>:8080` adresini aç.
- Tarayıcı menüsünden **Ana ekrana ekle** dersen oyun, `manifest.webmanifest` sayesinde tam ekran ve yatay açılır.

## Top fiziği

Bütün hesaplar gerçek masa ölçüleriyle, milimetre ve saniye cinsinden yapılır: 120 × 68 cm saha, 35 mm top, 20,5 cm kale ağzı, 15 cm çubuk aralığı. Çubuk düzeni gerçek masadaki gibidir: kaleci (1), defans (2), forvet (3) ve orta saha (5).

- **Kayma → yuvarlanma:** Vurulan top önce masada kayar. Sürtünme, topun dönüşünü doğrusal hızına eşitleyene kadar onu yavaşlatır, sonra top yuvarlanır. Dolu küre modeli kullanılır; kayma, doğrusal hızın 3,5 katı hızla söner. Bu yüzden duvardan kafa kafaya dönen top, önceki dönüşü ona ters çalıştığı için belirgin şekilde yavaşlar.
- **Yuvarlanma direnci ve hava sürtünmesi:** Top yuvarlanırken sabit bir yavaşlama ile hızla orantılı küçük bir sürtünme etki eder.
- **Vuruş:** Çubuk dönüş ekseni etrafında döner. Ayağın topa değdiği noktadaki hız `v = L · ω · cos θ` ile hesaplanır. Çarpışma, çarpma katsayılı ve sürtünmeli bir impuls olarak çözülür; bu da çubuğun kayma hızının topa yan hız olarak geçmesini sağlar. Kavisli ayak topu biraz üstten yakaladığı için topa bir miktar üst dönüş de verir.
- **Kalkan adamlar:** Adamlar yaklaşık 56°'den fazla döndüğünde ayaklar topun üstünden geçer ve çarpışma olmaz. Kendi pasın arkadan gelip adamlarından birine çarpacaksa o çubuk kalkar ve top altından geçer. Gerçek oyuncular da bunu içgüdüsel olarak yapar. Adamlar topun üstüne inerse top tuzağa düşer.
- **Duvarlar ve direkler:** Ahşap duvarlar ve yuvarlak kale direkleri farklı çarpma katsayılarına sahiptir.
- **Eğimli kenarlar:** Kenar rampaları ile köşe eğimleri, duran topu tekrar adamların erişebileceği yere yuvarlar.
- **Ölü top:** Hiçbir adamın ulaşamayacağı yerde duran top, kurala uygun biçimde orta sahadaki servis deliğinden yeniden oyuna girer.
- **Adım aralığı:** Fizik saniyede 480 sabit adımla hesaplanır. Böylece en sert şut bile bir adımda adamın içinden geçip gitmez.

## Bilgisayar rakip

Üç seviye vardır: **Acemi**, **Kulüp** ve **Usta**. Seviyeler şu değerlerde ayrışır:

- tepki süresi (topu 0,09–0,28 saniye gecikmeyle "görür")
- el hızı
- nişan hatası
- topun gideceği yeri önceden tahmin etme
- şut gücü
- açılı şut deneme sıklığı

Rakip, aktif çubuğunu topun o çubuğun hizasından geçeceği noktaya getirir. Top ayağının önündeyken kaleye doğru nişan alıp vurur. Arkaya düşen topu defans ya da forvetiyle topuk pasıyla kurtarır.

## Dosyalar

- `index.html`: oyunun tamamı (HTML, CSS, JavaScript; sesler Web Audio ile üretilir)
- `manifest.webmanifest`, `icon.svg`: ana ekrana eklemek için
