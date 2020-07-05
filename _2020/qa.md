---
layout: lecture
title: "Soru & Cevap"
date: 2019-01-30
ready: true
video:
  aspect: 56.25
  id: Wz50FvGG6xU
---

Son dersimizde, öğrencilerin yönelttiği soruları cevapladık:

- [İşletim Sistemleri ile ilgili olan process, sanal bellek, interrupt, bellek yönetimi gibi konuları öğrenmeyle ilgili tavsiyeleriniz nelerdir?](#isletim-sistemleri-ile-ilgili-olan-process-sanal-bellek-interrupt-bellek-yonetimi-gibi-konulari-ogrenmeyle-ilgili-tavsiyeleriniz-nelerdir)
- [Öncelikli olarak öğrenilmesi gerektiğini düşündüğünüz araçlardan bazıları nelerdir?](#oncelikli-olarak-ogrenilmesi-gerektigini-dusundugunuz-araclardan-bazilari-nelerdir)
- [Bash scriptlerini, Python'u veya diğer dilleri hangi durumlarda kullanabilirim?](#bash-scriptlerini-pythonu-veya-diger-dilleri-hangi-durumlarda-kullanabilirim")
- [`source script.sh` ve `./script.sh` arasındaki fark nedir?](#source-script-sh-ve-script-sh-arasindaki-fark-nedir)
- [Farklı paketlerin ve araçların depolandığı yerler nelerdir ve nasıl görebiliriz? `/bin` ve `/lib` gibi dizinlerin aralarındaki farklar nelerdir?](#farkli-paketlerin-ve-araclarin-depolandigi-yerler-nelerdir-ve-nasıl-gorebiliriz)
- [Python paketlerini `apt-get install` ile mi yoksa `pip install` ile mi kurmalıyım?](#python-paketlerini-apt-get-install-ile-mi-yoksa-pip-install-ile-mi-kurmaliyim)
- [Kodumun performansını iyileştirmek için kullanabileceğim en iyi ve en kolay **profiling** araçları nelerdir?](#kodumun-performansini-iyilestirmek-icin-kullanabilecegim-en-iyi-ve-en-kolay-profilling-araçları-nelerdir)
- [Hangi tarayıcı eklentilerini kullanıyorsunuz?](#hangi-tarayici-eklentilerini-kullaniyorsunuz)
- [Diğer faydalı **data wrangling** araçları nelerdir?](#diger-faydali-data-wrangling-araclari-nelerdir)
- [Docker ve Sanal Makine arasındaki fark nedir?](#docker-ve-sanal-makine-arasindaki-fark-nedir)
- [İşletim sistemlerinin avantajları ve dezavantajları nelerdir ve aralarında nasıl seçim (örneğin amaçlarımıza en uygun Linux dağıtımını seçmek) yapabiliriz?](#isletim-sistemlerinin-avantajlari-ve-dezavantajlari-nelerdir-ve-aralarinda-nasil-secim-yapabiliriz)
- [Vim vs Emacs?](#vim-vs-emacs)
- [Makine Öğrenimi uygulamaları için ipuçları ve püf noktalar nelerdir?](#makine-ögrenimi-uygulamalari-icin-ipuclari-ve-puf-noktalar-nelerdir)
- [Başka Vim ipuçları?](#baska-vim-ipuclari)
- [2FA nedir ve neden kullanmalıyım?](#2fa-nedir-ve-neden-kullanmalıyım)
- [Web tarayıcıları arasındaki farklar hakkında yorumunuz nedir?](#web-tarayicilari-arasindaki-farklar-hakkinda-yorumunuz-nedir)

<h2 id="isletim-sistemleri-ile-ilgili-olan-process-sanal-bellek-interrupt-
bellek-yonetimi-gibi-konulari-ogrenmeyle-ilgili-tavsiyeleriniz-nelerdir">
İşletim Sistemleri ile ilgili olan process (işlem), sanal bellek, interrupt
(kesme), bellek yönetimi gibi konuları öğrenmeyle ilgili tavsiyeleriniz
nelerdir?
</h2>

Öncelikle, oldukça düşük seviye konular olduğundan tüm bunlara gerçekten
aşina olmanız gerekip gerekmediği meçhuldür. Kernelde değişiklik yapmak
veya kerneli **implement etmek** gibi daha düşük seviyeli kodlar yazmaya
başlarsanız önemli olacaktır. Aksi halde, diğer derslerde kısaca ele
alınacak olan işlemler (process) ve sinyaller hariç, çoğu konuyla ilişkisi
yoktur.

Bu konu hakkında bilgi edinmek için bazı iyi kaynaklar:

- [MIT's 6.828 class](https://pdos.csail.mit.edu/6.828/) - İşletim Sistemi
Mühendisliği lisansüstü dersi. Sınıf materyalleri herkese açıktır.
- Modern Operating Systems (4th ed) - Andrew S. Tanenbaum kitabı bahsedilen
kavramların çoğuna iyi bir genel bakış sağlar.
- The Design and Implementation of the FreeBSD Operating System - FreeBSD
işletim sistemi hakkında güzel bir kaynak (bunun Linux olmadığını unutmayın). 
- Ve insanların çoğunlukla öğretim amaçlı olmak üzere çeşitli dillerde
adım adım kernel **implement ettiği** [Rust ile işletim sistemi yazmak](https://os.phil-opp.com/) 
gibi bir takım kılavuzlar. 

<h2 id="oncelikli-olarak-ogrenilmesi-gerektigini-dusundugunuz-araclardan-
bazilari-nelerdir">
Öncelikli olarak öğrenilmesi gerektiğini düşündüğünüz araçlardan bazıları
nelerdir?
</h2>

Öncelik vermeye değer bazı konular:

- Fareyi daha az, klavyeyi daha fazla kullanmayı öğrenin. Bu klavye
kısayolları ve arayüz değiştirme gibi çeşitli yöntemlerle olabilir.
- Editörünüzü iyi öğrenin. Bir programcı olarak zamanınızın çoğu dosyaları
düzenlemekle geçer, bu nedenle bu beceriye sahip olmak gerçekten işe yarar.
- İş akışınızdaki tekrarlayan görevleri otomatikleştirmeyi ve basitleştirmeyi
öğrenin, çünkü çok büyük bir zaman tasarruf sağlar.
- Git gibi versiyon kontrol araçlarını ve modern yazılım projelerinde
başkalarıyla çalışabilmek için Github ile birlikte nasıl kullanılacakları
konusunda bilgi edinin.

<h2 id="bash-scriptlerini-pythonu-veya-diger-dilleri-hangi-durumlarda-
kullanabilirim">
Bash scriptlerini, Python'u veya diğer dilleri hangi durumlarda
kullanabilirim?
</h2>

Bash scriptleri, yalnızca belirli komut dizilerini çalıştırmak istediğiniz
kısa ve tek seferlik basit scriptler için kullanışlıdır. bash, daha büyük
programlarda veya scriptlerde çalışmayı zorlaştıran bir dizi garipliğe
sahiptir:

- bash'te basit bir kullanım durumunu hatasız yazmak kolaydır, ancak tüm 
olası girdileri doğru bir şekilde elde etmek gerçekten zor olabilir.
Örneğin, script argümanlarında bulunan boşluklar bash scriptleri için
sayısız hataya yol açar.
- bash, kodun yeniden kullanılmasına uygun değildir, bu nedenle daha önce
yazmış olduğunuz programların bileşenlerini yeniden kullanmak zor olabilir.
Daha net söyleyecek olursak, bash'de yazılım kütüphanesi kavramı yoktur.
- bash, belirli değerleri ifade etmek için `$?` veya `$@` gibi birçok
sihirli stringe dayanırken, diğer diller onları açıkca belirtir. Örneğin
sırasıyla `exitCode` ve `sys.args` gibi.

Bu nedenle, daha büyük ve/veya karmaşık scriptler için Python ve Ruby gibi
daha olgun script dillerini kullanmanızı öneririz. İnsanların bu dillerde
sık karşılaşılan sorunları çözmek için daha önce yazmış oldukları sayısız
kütüphane bulabilirsiniz. Bir dilde size lazım olan işlevleri yerine getiren
bir kütüphane bulursanız, genellikle yapılacak en iyi şey bu dili kullanmaktır.

<h2 id="source-script-sh-ve-script-sh-arasindaki-fark-nedir">
<code>source script.sh</code> ve <code>./script.sh</code> arasındaki fark
nedir?
</h2>

Her iki durumda da `script.sh` dosyası bir bash oturumunda okunacak ve
yürütülecektir. Aralarındaki fark oturumun (session) komutları çalıştırma
şeklindedir. `source` için komutlar geçerli bash oturumunuzda yürütülür
ve bu nedenle geçerli ortam üzerinde yapılan dizin değiştirme veya fonksiyon
tanımlama gibi değişiklikler, `source` komutunun yürütülmesi tamamlandığında
geçerli oturumda devam edecektir. Script `./script.sh` şeklinde
çalıştırıldığında, geçerli bash oturumunuz `script.sh` dosyasındaki
komutları çalıştırmak için yeni bir bash örneği (**instance of bash**)
başlatır. Bu nedenle, `script.sh` dizinleri değiştirirse, yeni bash örneği
dizinleri değiştirir, ancak script tamamlanıp kontrol ana bash oturumuna
geçtiğinde üst oturum aynı konumda kalır. Benzer şekilde, `script.sh`,
terminalinizde erişmek istediğiniz bir fonksiyonu tanımlıyorsa, geçerli
bash oturumunuzda kullanmak için `source` etmeniz gerekir. Aksi takdirde
çalıştırdığınızda yeni bash işlemi (process), geçerli shell'iniz yerine
fonksiyon tanımını gerçekleştiren işlem olacaktır.

<h2 id="farkli-paketlerin-ve-araclarin-depolandigi-yerler-nelerdir-ve-
nasıl-gorebiliriz">
Farklı paketlerin ve araçların depolandığı yerler nelerdir ve nasıl
görebiliriz? `/bin` ve `/lib` gibi dizinlerin aralarındaki farklar nelerdir?
</h2>

Terminalinizde yürüttüğünüz programlara bakacak olursak, tümü `PATH` ortam
değişkeninde listelenen dizinlerde bulunur. Shell'inizin belirli bir programı
nereden çalıştırdığını görmek için `which` komutunu (ya da `type` komutunu)
kullanabilirsiniz. Genelde, belirli dosya türlerinin nerede olduğuna dair
bazı kurallar bulunur. İşte konuştuklarımızdan bazıları, daha kapsamlı bir
listei için [Dosya Sistemi Hiyerarşi Standardı](https://en.wikipedia.org/wiki/Filesystem_Hierarchy_Standard)
'na bakabilirsiniz.  

- `/bin` - Önemli program dosyaları
- `/sbin` - Root izni gerektiren önemli program dosyaları
- `/dev` - Donanım aygıtlarının arabirim dosyaları
- `/etc` - Sistem yapılandırma dosyaları
- `/home` - Kullanıcılara ayrılmış ev dizinleri
- `/lib` - Kütüphane dosyaları
- `/opt` - Üçüncü parti programların dosyaları
- `/sys` - Sistemin bilgi ve konfigürasyon dosyaları ([ilk derste](/2020/course-shell/) bahsi geçti)
- `/tmp` - Sistem yeniden başlatılınca silinen geçici dosyalar (keza `/var/tmp`)
- `/usr/` - Tüm kullanıcıların paylaştığı dosyalar
  + `/usr/bin` - Program dosyaları
  + `/usr/sbin` - Root izni gerektiren program dosyaları
  + `/usr/local/bin` - Kullanıcı tarafından derlenen programların dosyaları
- `/var` - Log (günlük) ve Cache (önbellek) dosyaları gibi sürekli değişen verileri barındıran dosyalar

<h2 id="python-paketlerini-apt-get-install-ile-mi-yoksa-pip-install-ile-mi-kurmaliyim">
Python paketlerini <code>apt-get install</code> ile mi yoksa <code>pip install</code>
ile mi kurmalıyım?
</h2>

Bu sorunun genel geçer bir cevabı yok. Aslında daha çok yazılım yüklemek
için sisteminizin paket yöneticisini mi yoksa dilin paket yöneticisini mi
kullanmanız gerektiğiyle ilgilidir. Dikkate alınması gereken birkaç şey:

- Yaygın paketler her ikisinde de bulunabilir, ancak daha az popüler olan
veya yeni oluşturulmuş olan paketler sistem paket yöneticinizde bulunmayabilir.
Bu durumda, dile özgü aracı kullanmak daha iyi bir seçimdir.
- Benzer şekilde, dile özgü paket yöneticileri genellikle sistem paket
yöneticilerinden daha güncel sürümlere sahiptir.
- Sistem paket yöneticinizi kullanırken, kütüphaneler sistem genelinde
kurulacaktır. Bu, geliştirme amacıyla bir kitaplığın farklı sürümlerine
ihtiyacınız varsa sistem paket yöneticisinin yeterli olamayabileceği anlamına
gelir. Bu senaryo için, çoğu programlama dili bir tür yalıtılmış sanal
ortam sağlar. Böylelikle kütüphanelerin farklı sürümlerini çakışmalara
neden olmadan yükleyebilirsiniz. Python için virtualenv, Ruby için RVM
örneklerindeki gibi.
- İşletim sistemine ve donanım mimarisine bağlı olarak, bu paketlerin
bazıları binary dosyalar ile gelebilir ve derlenmesi gerekebilir. Örneğin,
Raspberry Pi gibi ARM mimarili bilgisayarlarda, binary dosyalar halinde
geliyor ve sonrasında derlenmeleri gerekiyorsa, sistem paket yöneticisini
kullanmak dile özgü olandan daha iyi olabilir. Bu büyük ölçüde sizin
sisteminize bağlıdır.

Hata ayıklaması çakışmalara yol açabileceğinden, her ikisini birden değil,
sadece birini kullanmaya çalışmalısınız.Tavsiyemiz, mümkün olduğu kadar
dile özgü paket yöneticisini izole ortamlar ile kullanarak global ortamları
kirletmemeniz. 

<h2 id="kodumun-performansini-iyilestirmek-icin-kullanabilecegim-en-iyi-ve
-en-kolay-profilling-araçları-nelerdir">
Kodumun performansını iyileştirmek için kullanabileceğim en iyi ve en kolay
<b>profiling</b> araçları nelerdir?
</h2>

**profilling** amacıyla kullanmak oldukça kullanışlı olan en kolay araç
[süre ölçerek yazdırmadır](/2020/debugging-profiling/#timing).
Kodunuzun farklı bölümleri arasında geçen süreyi manuel olarak hesaplarsınız.
Bunu defalarca yaparak, kodunuz üzerinde etkili bir binary arama yapabilir
ve en uzun süren kod parçasını bulabilirsiniz. 

Daha gelişmiş araçlar için, Valgrind'in [Callgrind](http://valgrind.org/docs/manual/cl-manual.html)
aracı, programınızı çalıştırmanıza, tüm çağrı yığınlarının (call stack) ve
diğer şeylerin ne kadar sürdüğünü ölçmenize olanak tanır. Sonrasında,
programınızın kaynak kodunun satır başına harcadığı süreyi içeren ek açıklamalı
bir versiyonunu oluşturur. Ancak, programınızın büyüklüğüne göre yavaş
çalışır ve iş parçacıklarını (thread) desteklemez. Diğer durumlar için,
[`perf`](http://www.brendangregg.com/perf.html) aracı ve dile özgü diğer
**sampling profiler**ları yararlı verileri oldukça hızlı bir şekilde üretebilir.
[Flamegraphs](http://www.brendangregg.com/flamegraphs.html), bahsedilen
**sampling profiler** çıktısı için iyi bir görselleştirme aracıdır. Ayrıca,
üzerinde çalıştığınız programlama dili veya programlama görevi için özel araçlar
kullanmaya çalışmalısınız. Örneğin, web geliştirme için, Chrome ve Firefox'taki
dahili geliştirici araçlarının fantastik **profiler**ları vardır.

Bazen kodunuzun yavaş kısmı, sisteminizin disk okuması veya paket iletimi
gibi bir olay bekleme aşaması olabilir.
**In those cases, it is worth checking that back-of-the-envelope calculations about the theoretical speed in terms of hardware capabilities do not deviate from the actual readings**. Sistem çağrılarındaki
bekleme sürelerini analiz etmek için özelleşmiş araçlar da vardır. Bunlar,
kullanıcı programlarının çekirdek izlemesini gerçekleştiren
[eBPF](http://www.brendangregg.com/blog/2019-01-01/learn-ebpf-tracing.html)
gibi araçları içerir. Özellikle bu tür düşük seviye **profiling** yapmanız
gerekiyorsa [`bpftrace`](https://github.com/iovisor/bpftrace) aracı göz atmaya değerdir.


<h2 id="hangi-tarayici-eklentilerini-kullaniyorsunuz">
Hangi tarayıcı eklentilerini kullanıyorsunuz?
</h2>

Çoğunlukla güvenlik ve kullanılabilirlikle sağlayan favorilerimizden bazıları:

- [uBlock Origin](https://github.com/gorhill/uBlock) - Yalnızca reklamları
durdurmakla kalmayan, aynı zamanda bir sayfayla her türlü üçüncü şahıs
etkileşimine girmeyi deneyebileceğiniz
[geniş yelpazeye sahip](https://github.com/gorhill/uBlock/wiki/Blocking-mode)
bir engelleyicidir. Buna satır içi scriptler ve diğer kaynak yükleme türleri
de dahil. Bazı ayarları özel olarak yapılandırmak için zaman harcamak
istiyorsanız, [medium mode](https://github.com/gorhill/uBlock/wiki/Blocking-mode:-medium-mode)
ve hatta [hard mode](https://github.com/gorhill/uBlock/wiki/Blocking-mode:-hard-mode)
geçebilirsiniz. Bunlar, ayarlar üzerinde uğraşmadıkça bazı sitelerin
çalışmamasına yol açar, ancak çevrimiçi güvenliğinizi önemli ölçüde arttırır.
Aksi takdirde, [easy mode](https://github.com/gorhill/uBlock/wiki/Blocking-mode:-easy-mode)
zaten çoğu reklamı ve izlenmeyi engelleyen iyi bir varsayılandır.
- [Stylus](https://github.com/openstyles/stylus/) - Stylish fork'u (Stylish
kullanmayın, [kullanıcıların göz atma geçmişini gizlice kaydettiği](https://www.theregister.co.uk/2018/07/05/browsers_pull_stylish_but_invasive_browser_extension/)
ortaya çıktı),websitelere özel CSS stil sayfaları eklemenize izin verir.
Stylus ile web sitelerinin görünümünü kolayca değiştirebilir ve
özelleştirebilirsiniz. Örneğin kenar çubuğunu kaldırabilir, arka plan
rengini, metin boyutunu veya yazı tipi tercihini değiştirebilirsiniz. Bu,
sık ziyaret ettiğiniz web sitelerini daha okunaklı yapmak için harikadır.
Ayrıca, Stylus diğer kullanıcılar tarafından yazılan ve
[userstyles.org](https://userstyles.org/)'da yayınlanan stilleri bulabilir.
Çoğu yaygın web sitesinde örneğin bir veya birkaç karanlık tema stil sayfası
bulunur. 
- Tam Sayfa Ekran Yakalama - Firefox ve 
[Chrome eklentisi](https://chrome.google.com/webstore/detail/full-page-screen-capture/fdpohaocaechififmbbbbbknoalclacl?hl=en)
vardır. Web sitenin tam ekran görüntüsünü alır, genellikle referans amaçlı
çıktı alırken iyidir.
- [Multi Account Containers](https://addons.mozilla.org/en-US/firefox/addon/multi-account-containers/) 
\- çerezleri "konteyner" olarak ayırmanıza olanak tanır. Böylece internette
farklı kimliklerle dolaşmanızı ve web sitelerin kendi aralarında bilgi
paylaşmasını engeller.
- Şifre Yöneticisi Entegrasyonu - Çoğu şifre yöneticisinin, kimlik bilgilerini
sitelere girmeyi daha güvenli hale getiren tarayıcı uzantıları vardır.
Kullanıcı adı ve şifrenizi basitçe kopyalayıp yapıştırmayla karşılaştırıldığında,
bu araçlar önce web sitesi alan adının giriş için listelenen alan adıyla
eşleşip eşleşmediğini kontrol ederek kimlik bilgilerini çalmak için popüler
web sitelerini taklit eden kimlik avı saldırılarını önler.

<h2 id="diger-faydali-data-wrangling-araclari-nelerdir">
Diğer faydalı data wrangling araçları nelerdir?
</h2>

**Data wrangling** dersi sırasında yer verme fırsatımızın olmadığı araçlardan
bazıları, sırasıyla JSON ve HTML verileri için özel ayrıştırıcılar olan `jq`
ve `pup`'tır. Perl programlama dili, daha gelişmiş **data wrangling pipelines**
için bir diğer güzel araçtır. Başka bir püf nokta, boşluklu metni sütunlar
halinde düzgünce hizalanmış bir metne dönüştürmek için kullanılan `column -t`
komutudur.

Daha genel olarak alışılmadık diğer veri düzenleme araçları ise vim ve
Python'dur. Bazı karmaşık ve çok satırlı dönüşümler için, vim makroları
kullanımı oldukça kolay değerli bir araç olabilir. Bir dizi eylemi
kaydedebilir ve bunları istediğiniz kadar tekrarlayabilirsiniz, örneğin
editörler hakkındaki [ders notunda](/2020/editors/#macros) (ve geçen yılki
[videoda](/2019/editors/)) XML formatlı bir dosyayı sadece vim makroları
kullanılarak JSON'a dönüştürme örneği mevcut.

[pandas](https://pandas.pydata.org/) Python kütüphanesi genellikle
CSV'lerde sunulan tablo verileri için harika bir araçtır. Sadece gruplandırma,
birleştirme veya filtreleme gibi karmaşık işlemleri tanımlamayı kolaylaştırmakla
kalmaz, aynı zamanda verilerinizin farklı özelliklerinin grafiklerini çizmeyi
de oldukça kolaylaştırır. Ayrıca XLS, HTML veya LaTeX gibi birçok tablo
formatında dışa aktarmayı destekler. Alternatif olarak R programlama dili
(tartışmasız [kötü](http://arrgh.tim-smith.us/) bir programlama dili),
veriler üzerindeki istatistikleri hesaplamak için birçok işlevselliğe
sahiptir ve pipeline'ınızın son adımı olarak oldukça yararlı olabilir.
[ggplot2](https://ggplot2.tidyverse.org/), R'de harika bir çizim kütüphanesidir. 

<h2 id="docker-ve-sanal-makine-arasindaki-fark-nedir">
Docker ve Sanal Makine arasındaki fark nedir?
</h2>

Docker, konteyner olarak adlandırılan daha kapsamlı bir konsepte dayanmaktadır.
Konteynerler ve sanal makineler arasındaki temel fark, sanal makinelerin
çekirdek ana makine ile aynı olsa bile, çekirdek de dahil olmak üzere tüm
OS yığınını yürütmesidir. VM'lerin aksine konteynerler, çekirdeğin başka
bir örneğini çalıştırmaktan kaçınır ve bunun yerine çekirdeği ana bilgisayarla
paylaşırlar. Linux'ta bu, LXC adı verilen mekanizma ile elde edilir ve kendi
donanımında çalıştığını düşünen bir programı döndürmek için bir dizi yalıtım
mekanizmasından yararlanır, ama  aslında donanımı ve çekirdeği ana bilgisayarla
paylaşır. Böylece konteynerler tam yükteki VM'den daha düşük ek yüke sahiptir.
Diğer taraftan bakarsak, konteynerler daa zayıf bir yalıtıma sahiptir ve
yalnızca ana bilgisayar aynı çekirdekte koşuyorsa çalışır. Örneğin, Docker'ı
macOS'ta çalıştırıyorsanız, Docker'ın ilk Linux çekirdeğini almak için bir
Linux sanal makinesini döndürmesi gerekir ve bu nedenle ek yük hala önemlidir.
Son olarak Docker, konteynerlerin özel bir implementasyonudur ve yazılım
dağıtımı için uyarlanmıştır. Bu nedenle, bazı tuhaflıkları vardır; örneğin,
Docker konteynerleri varsayılan olarak yeniden başlatmalar arasında herhangi
bir depolama biçiminde kalamaz.

<h2 id="isletim-sistemlerinin-avantajlari-ve-dezavantajlari-nelerdir-ve-aralarinda-nasil-secim-yapabiliriz">
İşletim sistemlerinin avantajları ve dezavantajları nelerdir ve aralarında
nasıl seçim (örneğin amaçlarımıza en uygun Linux dağıtımını seçmek) yapabiliriz?
</h2>

Linux dağıtımları, çok sayıda dağıtım olmasına rağmen, çoğu kullanım
durumunda aynı şekilde davranacaklardır. 
Linux ve UNIX özelliklerinin ve çalışma biçimlerinin çoğu herhangi bir
dağıtımda öğrenilebilir. 
Dağıtımlar arasındaki temel fark, paket güncellemeleriyle nasıl başa
çıktıklarıdır. 
Arc Linux gibi bazı dağıtımlar, her şeyin en son versiyona sahip oldukları
ve çok sıkı bozulabildiği sallantılı bir güncelleme politikası izlerler.
Öte yandan Debian, CentOS gibi bazı dağıtımlar ve Ubuntu'nun LTS sürümleri
depolarındaki güncellemeleri yayınlarken çok daha tutucu olduğundan, yeni
özelliklerden ödün vermek pahasına kararlı durumlarını korurlar.
Hem masaüstü bilgisayarlar hem de sunucularla kolay ve kararlı bir deneyim
için önerimiz Debian veya Ubuntu kullanmaktır.

Mac OS, Windows ve Linux arasındaki orta noktadır ve güzel bir arayüze sahiptir.
Ancak MacOS, Linux'dan ziyade BSD tabanlıdır. Bu nedenle sistemin ve komutların
bazı kısımları farklıdır. Göz atmaya değer bir alternatif ise FreeBSD'dir.
Bazı programlar FreeBSD'de çalışmayacak olsa da, BSD ekosistemi Linux'tan
daha az dallara ayrılmış ve daha iyi belgelenmiştir. 
Windows'u ise Windows uygulamaları geliştirmek ve oyun oynamak için en iyi
sürücü desteği gibi akıl çelici özelliklerine ihtiyacımız olmayacaksa tavsiye
etmiyoruz. 

Dual boot sistemler için, en iyi çalışan implementasyonun macOS’in bootcamp'i
olduğunu ve özellikle disk şifreleme gibi diğer özelliklerle birleştirirseniz,
diğer tüm kombinasyonların uzun vadede sorun yaratabileceğini düşünüyoruz.

<h2 id="vim-vs-emacs">
Vim vs Emacs?
</h2>

Üçümüz de birincil editörümüz olarak Vim kullanıyoruz ancak Emacs da iyi
bir alternatif. Hangisinin sizin için daha iyi olduğunu görmek için denemeye
değer. Emacs, vim'in **modal editing** özelliğini barındırmaz. Fakat bu,
[Evil](https://github.com/emacs-evil/evil) ve
[Doom Emacs](https://github.com/hlissner/doom-emacs) eklentileri aracılığıyla 
etkinleştirilebilir. 
Emacs kullanmanın bir avantajı, bu uzantıların Vim'in varsayılan script
dili vimscript'ten daha iyi bir script dili olan Lisp'te uygulanabilinmesidir.

<h2 id="makine-ögrenimi-uygulamalari-icin-ipuclari-ve-puf-noktalar-nelerdir">
Makine Öğrenimi uygulamaları için ipuçları ve püf noktalar nelerdir?
</h2>

Buradaki bazı dersler ve düşünceler Makine Öğrenimi uygulamalarına doğrudan
uygulanabilir. 
Birçok bilim dalında olduğu gibi, ML'de sıklıkla bir dizi deney yaparsınız
ve neyin işe yarayıp neyin işe yaramadığını kontrol etmek istersiniz. 
Bu deneylerde kolayca ve hızlı bir şekilde arama yapmak ve sonuçları anlamlı
bir şekilde toplamak için shell araçlarını kullanabilirsiniz. Bu, verilen
zaman diliminde  veya belirli bir veriseti kullanan tüm deneylerin alt
seçimi anlamına gelebilir. Deneyler sonucunda ulaşılan parametreleri saklamak
için basit bir JSON dosyası kullanmak, bu sınıfta ele aldığımız araçlarla
inanılmaz derecede kolay olabilir. Son olarak, GPU görevlerinizi gönderdiğiniz
bir tür kümeyle çalışmıyorsanız, zihinsel enerjinizi de tüketen oldukça zaman
alıcı bir görev olabileceğinden, bu süreci nasıl otomatikleştireceğinizi
araştırmalısınız.

<h2 id="baska-vim-ipuclari">
Başka Vim ipuçları?
</h2>

Birkaç ipucu daha: 

- Eklentiler - Aceleye etmeden eklenti mağazasını keşfedin. Bazı vim
eksiklerini gideren veya mevcut vim iş akışlarıyla uyumlu yeni işlevler
ekleyen birçok harika eklenti vardır. Bunun için en iyi kaynaklar
[VimAwesome](https://vimawesome.com/) ve diğer programcıların **dotfile**'larıdır.
- İşaretler - Vim'de, bazı `X` harfleri için `m<X>` yaparak işaret
oluşturabilirsiniz. Daha sonra`'<X>` kullanarak o işarete geri dönebilirsiniz.
Bu, bir dosyadaki ve hatta dosyalar arasındaki belirli konumlara hızlı
şekilde gitmenizi sağlar.
- Gezinme - `Ctrl+O` ve `Ctrl+I` son gittiğiniz konumlarda sizi sırasıyla
ileri ve geri hareket ettirir.
- **Undo Tree**- Vim, değişiklikleri takip etmek için oldukça süslü bir
mekanizmaya sahiptir. Diğer editörlerin aksine, vim değişiklik ağacı saklar.
Böylece geri alıp farklı değişiklik yapsanız bile **undo tree**de gezinerek
orjinal durumuna geri dönebilirsiniz. [gundo.vim](https://github.com/sjl/gundo.vim)
ve [undotree](https://github.com/mbbill/undotree) gibi bazı eklentiler bu
ağacı grafiksel yolla gösterir. 
- Zamana Göre Geri Alma - `:earlier` ve `:later` komutları, her seferinde
bir değişiklik yerine zamanı referans  alarak dosyalarda gezinmenizi sağlar.
- [Persistent undo](https://vim.fandom.com/wiki/Using_undo_branches#Persistent_undo)
vim'de gömülü (built-in) olarak gelen ve varsayılan olarak devre dışı olan
harika bir özelliktir. **It persists undo history between vim invocations**.
`.vimrc` dosyanızda `undofile` ve `undodir` ayarlayarak, dosya başına
değişiklik geçmişini depolar.
- **Leader Key** - Leader key, genellikle özel komutlar için yapılandırılmak
üzere kullanıcıya bırakılan özel bir anahtardır. Desen(pattern) genellikle
bu tuşa (genelde space) ve ardından belirli bir komutu yürütmek için başka
bir tuşa basıp bırakmaktır. Eklentiler de kendi işlevlerini eklemek için
bu anahtarı kullanırlar; örneğin, UndoTree eklentisi geri alma ağacını
açmak için `<Leader> U` kullanır. 
- **Advanced Text Objects - Text objects like searches can also be composed with vim commands. E.g. `d/<pattern>` will delete to the next match of said pattern or `cgn` will change the next occurrence of the last searched string.**

<h2 id="2fa-nedir-ve-neden-kullanmalıyım">
2FA nedir ve neden kullanmalıyım?
</h2>

İki Aşamalı Doğrulama (2FA), hesaplarınıza şifrelerin yanı sıra ekstra bir
koruma katmanı ekler. Giriş yapmak için sadece parola bilmek yetmez, aynı
zamanda bazı cihazlara erişiminizin olduğunu bir şekilde "kanıtlamanız"
gerekir. En basit şekilde, SMS 2FA ile ilgili 
[bilinen bazı sorunlar](https://www.kaspersky.com/blog/2fa-practical-guide/24219/) 
olmasına rağmen, telefonunuza bir SMS gönderilerek yapılabilir.
Desteklediğimiz daha iyi bir alternatif, [YubiKey](https://www.yubico.com/)
gibi  [U2F](https://en.wikipedia.org/wiki/Universal_2nd_Factor) çözümü
kullanmaktır.

<h2 id="web-tarayicilari-arasindaki-farklar-hakkinda-yorumunuz-nedir">
Web tarayıcıları arasındaki farklar hakkında yorumunuz nedir?
</h2>

2020 yılı itibariyle tarayıcıların şu anki manzarası, aynı motoru (Blink)
kullandıklarından dolayı çoğunun Chrome'a ​​benziyor olduğudur. Bu, Blink
tabanlı Microsoft Edge'in ve Blink'e benzer bir motor olan WebKit tabanlı 
Safari'nin, sadece Chrome'un kötü versiyonları oldukları anlamına gelir.
Chrome, hem performans hem de kullanılabilirlik açısından oldukça iyi bir
tarayıcıdır. Alternatif isteyecek olursanız bizim önerimiz Firefox'tur.
Chrome ile hemen hemen her açıdan yarışabilir ve gizlilik konusunda mükemmeldir.
[Flow](https://www.ekioh.com/flow-browser/) isimli bir diğer tarayıcı,
henüz kullanıma hazır olmamakla birlikte, var olanlardan daha hızlı olacağını
iddia ettiği yeni bir render motoru uyguluyor.