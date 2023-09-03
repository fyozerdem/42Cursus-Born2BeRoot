# 42Cursus-Born2BeRoot

# Sorular

</div>

<div class="page-body">

Başlangıç:

1- `cd goinfre/fozerdem/born2beroot ` sonrasında
`shasum born2beroot.vdi` yap ve gitclonedan çektiğin id ile
karşılaştır.Bu idnin işlem sornası değişmemesini istiyosan sanal makine
üstünden anlık görüntü almayı unutma.

****Project overview :****

-   Sanal Makine nasıl çalışır?

    Sanal Makineler, donanımdan ayrılmış katmanda bir bilgisayarın sanal
    örneğini çalıştırırlar. Bu işlem sanallaştırma (virtualization)
    tekniği sayesinde mümkündür. Makinenin kaynaklarının sanallaştırılma
    işlemi, VM'leri oluşturan, barındıran ve çalıştıran hipervizör adı
    verilen bir yazılım tarafından gerçekleştirilir.

    Sanallaştırma sayesinde, VM'ler kullanıcılar için sanal bir ortam
    oluşturur. Sanal makineler, bilgisayarın işletim sistemindeki bir
    pencerede işlem olarak çalışır. Kullanıcılar bu ortamlarda
    uygulamalar çalıştırabilir, veri depolayabilir ve herhangi bir
    bilgisayarda yapılabilecek herhangi bir eylemi gerçekleştirebilir.
    Sanal Makineler, işletim sistemini bir yazılım yerine bilgisayarın
    yerel donanımında çalıştıklarına inandırarak çalışır, dolayısıyla
    bir bilgisayarın tüm kabiliyetlerine sahiptir.

<!-- -->

-   İşletim sistemini neden Debian seçtin? Diğer işletim sistemleri
    neler?

<!-- -->

-   Rocky ve Debian arasındaki temel farkları nelerdir?
    -   Rocky Linux daha yeni kurulan (2021) bir işletim sistemi.(CentOS
        klonu olmayı amaçlıyor).Debian ise 1993te kurulmuş.

    <!-- -->

    -   Debian, büyük ve aktif bir topluluğa sahiptir. Kullanıcılar
        arasında geniş bir destek ağı bulunur ve paket deposunda geniş
        bir yazılım yelpazesi bulunur. Rocky Linux'in de kendi topluluğu
        vardır, ancak Debian kadar geniş ve köklü değildir.

    <!-- -->

    -   Debian, kararlı sürümü ve kararsız (testing) sürümü gibi farklı
        sürümleri bulunan bir güncelleme politikasına sahiptir. Kararlı
        sürüm, daha güvenilir ve daha az hata içerirken, testing sürümü
        daha yeni paketleri içerir. Rocky Linux ise, CentOS Stream'e
        dayandığı için sürekli güncellenen bir yapıya sahiptir.Sürekli
        güncellenmesinden dolayı uyum sorunları,test edilmemiş
        güncellemeleriinin yaratçağı sorunlar olabilir.

    <!-- -->

    -   Debian, geniş bir paket deposuna sahiptir ve birçok farklı
        mimariyi destekler. Bu, farklı ihtiyaçlarınıza ve donanımınıza
        uygun paketleri bulmanızı sağlar. Rocky Linux ise CentOS ile
        uyumlu olduğu için, CentOS için geliştirilen uygulamaları ve
        araçları kullanabilirsiniz.

<!-- -->

-   Debian vs CentOS

    1.  Debian apt’dir, CentOS yum.

    2.  CentOS kararlı bir yapıdadır(Az ve Öz güncelleme alıyor). Debian
        daha az kararlı(Çok Güncelleme Alıyor).

    3.  CentOS redhat tarafından lanse edilirken, Debian bireysel lanse
        ediliyor.

    4.  CentOS kendi güvenlik sistemiyle geliyor(Güvenlik Sisteminin
        Adı: Selinux).

    5.  CentOS kurumsal alanda daha çok tercih ediliyor, Debian
        bireysel.

<!-- -->

-   Sanal makinenin amacı nedir?
    -   Uygulamaları bulutta derleme ve dağıtma.

    <!-- -->

    -   Beta sürümleri dahil olmak üzere yeni bir işletim sistemi (OS)
        deneme.

    <!-- -->

    -   Geliştiricilerin geliştirme-test senaryolarını çalıştırmasını
        kolaylaştırmak ve hızlandırmak için yeni bir ortam oluşturma.

    <!-- -->

    -   Mevcut işletim sisteminizi yedekleme.

    <!-- -->

    -   Virüs bulaşmış verilere erişme veya eski bir işletim sistemini
        yükleyerek eski bir uygulamayı çalıştırma.

    <!-- -->

    -   Yazılım veya uygulamaları, başlangıçta amaçlanmadıkları işletim
        sistemlerinde çalıştırma.

<!-- -->

-   Aptitude ile Apt arasındaki fark ve APPArmor'ın nedir?
    -   Diyelim ki bir yazılımı yüklemek istiyorsunuz, ancak yazılımın
        bağımlı olduğu başka paketler de var. Aptitude, bu
        bağımlılıkları otomatik olarak çözebilir ve eksiksiz bir kurulum
        yapabilir.Apt de bu bağımlılıkları elle yapmak zorundasın

    <!-- -->

    -   Aptitude, hem komut satırı tabanlı hem de grafiksel bir
        kullanıcı arayüzü sunar. Bu grafiksel arayüz, paketlerinizi daha
        sezgisel bir şekilde yönetmenize yardımcı olabilir.Apt,
        genellikle komut satırı tabanlıdır. Bu nedenle grafiksel bir
        kullanıcı arayüzüne sahip değildir.

    <!-- -->

    -   Aptitude, paket yükseltme veya kaldırma işlemlerini interaktif
        bir şekilde yönetmenize olanak tanır. Bu, hangi paketlerin
        güncelleneceğini veya kaldırılacağını daha iyi kontrol etmenizi
        sağlar.Apt de bu yönetimi komutlarla yapmak zorundasın

    <!-- -->

    -   AppArmor
        -   AppArmor, Ubuntu 7.10'dan beri Ubuntu'ya varsayılan olarak
            dahil edilen önemli bir güvenlik özelliğidir. Ancak arka
            planda sessizce çalışır, bu nedenle ne olduğunun ve ne
            yaptığının farkında olmayabilirsiniz.

        <!-- -->

        -   AppArmor, bir web tarayıcısı veya sunucu yazılımı gibi
            kötüye kullanılabilecek yazılımları kısıtlamak için
            özellikle yararlıdır.

        <!-- -->

        -   AppArmor, profil adı verilen yapılandırmalar kullanarak
            uygulama davranışlarını kısıtlayabilir. Bu profiller,
            uygulamaların belirli dosyalara erişimini kontrol edebilir,
            ağ bağlantılarını düzenleyebilir ve diğer güvenlik
            önlemlerini uygulayabilir. Bu şekilde, AppArmor
            uygulamaların zararlı etkilerini sınırlayarak sistemin
            güvenliğini artırabilir.

<!-- -->

-   Ekranda 10 dkda bir script gelicek onu kontrol detaylarını sonraki
    sorularda sorulcak.

------------------------------------------------------------------------

****Simple setup:****

-   UFW service nedir kontol et

    `systemctl status ufw`

    -   UFW (uncomplicated firewall), Linux'ta güvenlik duvarı
        kurallarını yönetmek için kullanılan bir araçtır.

    <!-- -->

    -   Güvenlik duvarını hızlı bir şekilde etkinleştirme veya devre
        dışı bırakma seçeneği sunar.

    <!-- -->

    -   Gelen ve giden trafiği kontrol etmek için temel güvenlik
        politikaları oluşturmanıza olanak tanır.

    <!-- -->

    -   Sadece gereken portlara erişim sağlayarak saldırırlardan korur.

    <!-- -->

    -   Zararlı yazılımların sisteme sızmasından korur.

    <!-- -->

    -   Yalnızca belirli IP adreslerinden gelen erişimlere izin vererek
        güvenliği artırabilirsiniz.

    disable -\> `systemctl disable ufw`

    inactive → `systemctl stop ufw`

    -   enable vs stop

        -   `systemctl stop`: Bu komut, belirtilen hizmeti **anında
            durdurur**. Hizmetin çalışması durdurulur ve mevcut işlemler
            sonlandırılır. Hizmet, sistem yeniden başlatılmadığı sürece
            otomatik olarak başlamaz.

        <!-- -->

        -   `systemctl disable`: Bu komut, belirtilen hizmetin **sistem
            başlangıcında otomatik olarak başlamasını engeller**.
            Hizmetin çalışması durdurulmaz, sadece sistem yeniden
            başlatıldığında otomatik olarak başlamaz. Hizmeti manuel
            olarak başlatmak veya durdurmak hala mümkündür.

        Özetle, `systemctl stop` komutu hizmeti anında durdururken,
        `systemctl disable` komutu hizmetin otomatik başlamasını sistem
        başlangıcında engeller.

<!-- -->

-   SSH servise nedir kontol et

    `systemctl status ssh`

    disable için → `systemctl disable ssh` → enable için
    `systemctl enable ssh`

    inactive için → `systemctl stop ssh` → active için
    `systemctl start ssh`

    -   SSH (Secure Shell), güvenli bir uzaktan erişim protokolüdür.

    <!-- -->

    -   SSH’nin çalışması, iki uzak sistemin kimlik doğrulamasına ve
        aralarında geçen verilerin şifrelenmesine izin vermek için bir
        istemci-sunucu modelinden faydalanmaktır.

<!-- -->

-   debian mı rocky mi kontrol et

    `cat etc/os-release` → debianın versyonunu gösterir

    <figure>
    <img width="496" alt="Ekran_Resmi_2023-08-14_OS_2 11 15" src="https://github.com/fyozerdem/42Cursus-Born2BeRoot/assets/138295010/f92b5686-bbb7-4727-931b-40cc8c5f7fdc">
    </figure>

------------------------------------------------------------------------

****User :****

-   öğrencinin sudo ve user42 grubuna ait olup olmadığına bakın.

    `grep -w sudo etc/group` or `getent group sudo`

    `grep -w user42 etc/group` or `getent group user42`

    <figure>
    <img width="325" alt="Ekran_Resmi_2023-08-14_OS_3 02 46" src="https://github.com/fyozerdem/42Cursus-Born2BeRoot/assets/138295010/27f565db-c7f3-4350-98cc-a72496273339">
    </figure>

<!-- -->

-   Yeni kullanıcı oluştur,şifre kurallarına uygun bir şifre belirle.

    `sudo adduser kullanıcı`

    `grep -w kullanıcı etc/group` or `getent group kullanıcı` ***→***
    kullanıcı nerde görüyom

<!-- -->

-   Konuda istenen kuralları sanal makinesinde nasıl oluşturduğunu
    açıkla.

    `sudo vim /etc/login.defs` **→ PASS_MAX_DAYS 30,PASS_MIN_DAYS
    2,PASS_WARN_AGE 7**

    `sudo vim /etc/pam.d/common-password` **→ şifre için gerekli
    şeylerin olduğu dosya**

    -   Güçlü bir şifre politikası oluşturmak için aşağıdaki
        gereksinimlere uymalısınız:

        → `sudo vim /etc/login.defs` **bu dosyada işlemler sürcek**

        1.  Şifreniz her 30 günde bir süresi dolmalıdır.
             <!-- -->
                  PASS_MAX_DAYS 30
             <!-- -->

        <!-- -->

        2.  Bir şifrenin değiştirilmeden önce izin verilen minimum gün
            sayısı 2 olarak ayarlanacaktır.
             <!-- -->
                  PASS_MIN_DAYS 2
             <!-- -->
        <!-- -->

        3.  Kullanıcı, şifresinin süresi dolmadan 7 gün önce bir uyarı
            ile bilgilendirilmelidir.
            <!-- -->
                   PASS_WARN_AGE 7
             <!-- -->
            

        <!-- -->
         
        4.  Şifreniz en az 10 karakter uzunluğunda olmalıdır. Bir büyük
            harf, bir küçük harf ve bir rakam içermelidir. Ayrıca, üç
            ardışık aynı karakteri içermemelidir.

            `sudo vim /etc/pam.d/common-password`

            → `ucredit=-1 `**→ En az bir büyük harf içermeli**

            → `lcredit=-1 `**→ En az bir küçük harf içermeli**

            → `dcredit=-1` **→ En az bir sayı içermeli**

            →` ``maxrepeat=3`**→ En fazla 3 ardışık aynı karakter içerebilir.**

            →`minlen=10` **→ Şifre minimum uzunluğunu 10 karakter**

            →`usercheck=1`**→ Şifre, kullanıcının adını içermemelidir.**
        <!-- -->

        6.  Aşağıdaki kural kök (root) şifresi için geçerli değildir:
            Şifre, önceki şifrenin parçası olmayan en az 7 karakter
            içermelidir. 

            →` ``difok=7` **→** önceki şifrenin parçası olmayan en az 7 karakter

        <!-- -->

        7.  Tabii ki, kök (root) şifreniz de bu politikaya uymalıdır. 
           
            →`enforce_for_root `**→ Tüm bu şifre politikasını **root **kullanıcısı üzerinde uygulanır.**

        <figure>
        ![Untitled](https://github.com/fyozerdem/42Cursus-Born2BeRoot/assets/138295010/bb278635-eefb-451b-a39c-fb9d1799bc3e)

        </figure>

        `sha512` → Bu modül, kullanıcıların parola doğrulama işlemlerini
        kontrol etmek ve yönlendirmek için kullanılır. `sha512` ise bir
        şifreleme algoritmasıdır ve parolaların güvenli bir şekilde
        saklanmasını sağlar.

        SHA-512 (Secure Hash Algorithm 512) ise güvenli bir karma
        algoritmasıdır ve parolaların özetlerini (hash) oluşturmak için
        kullanılır. Karma algoritmaları, veriyi belirli bir uzunlukta
        sabit bir dizeye dönüştüren ve tek yönlü olan matematiksel
        işlemlerdir.

        `obscure `→ pam_unix.so obscure"ifadesi, bu PAM modülünün parola
        politikalarını veya parola karmaşıklığını artıran ve belirli bir
        güvenlik seviyesini sağlayan ayarları

    <!-- -->

    -   Eğer fozerdem üsründe şifre uygulancaksa :
        `sudo chage --mindays 2 fozerdem`

<!-- -->

-   "evaluating" adında bir grup oluştur

    `sudo addgroup evoluating`

    `grep -w evoluating etc/group` → ` evoluating` groupu var mı kontrol et

<!-- -->

-   bu grubu bu kullanıcıya atamasını isteyin

    `adduser kullanıcı evoluating ` or
    `sudo usermod -aG evaluating your_new_username`

<!-- -->

-   bu kullanıcının "evaluating" grubuna ait olup olmadığını kontrol
    edin.

    `grep -w kullanıcı etc/group` or `getent group evaluating`

    `groups kullanıcı` → kullanıcıların bağlı olduğu grupları gösterir

    <figure>
    <img
    src="Sorular%20167ee0641edc429fb2420d028dc41017/Ekran_Resmi_2023-08-14_OS_8.16.24.png"
    style="width:1134px" />
    </figure>

<!-- -->

-   silmek için

    `sudo groupdel gorupname` → grup silmek için

    `sudo deluser kullanıcı` → user desilmek için

<!-- -->

-   değerlendirilen öğrenciden bu şifre politikasının
    avantajlarını,uygulamanın avantajlarını ve dezavantajlarını
    açıklamasını isteyin.

    [https://www.passwordmonster.com](https://www.passwordmonster.com/)

    Parolaların kırılma hızı çok artıyo.Şifrelenmesi için özel şifreleme
    sistemleri kullanıyoruz.Hesap paylaşımı azalır çünkü güçlü
    parolaları insanlar paylaşmak istemez

    Hatırlaması zor,kullanıcı memnuniyetsiz

------------------------------------------------------------------------

****Hostname and partitions:****

-   hostname login42 olmalı kontol et

    `hostnamectl`

<!-- -->

-   hostaname adını evocu adıyla değiştir , rebbot et

    `hostnamectl set-hostname server1`

    `vim etc/hosts` → girip adını değiştiriyoruz

    `reboot`

<!-- -->

-   makineyi tekrar original hostname e çevir

    `hostnamectl set-hostname fozerdem42`

<!-- -->

-   sanal makinenin bölmelerini nasıl görüntüleyebileceğini sorun.

    `lsblk`

    <figure>
    <img
    src="Sorular%20167ee0641edc429fb2420d028dc41017/Ekran_Resmi_2023-08-24_OS_6.23.04.png"
    style="width:1648px" />
    </figure>

<!-- -->

-   LVM'nin nasıl çalıştığına ve konunun ne hakkında olduğuna dair kısa
    bir açıklama yapmalıdır.

    -   Geleneksel bir disk yönetimi modelinde, işletim sistemi önce
        kullanılabilir sürücüleri arar ve ardından bu aygıtlarda hangi
        birimlerin kullanılabilir olduğunu kontrol eder.

    <!-- -->

    -   LVM ise sürücüler ve birimler tek bir sürücü birkaç disk ve
        birim içerecek şekilde ele alınabilir.Disk alanı bu şekilde ele
        alınırsa işletim sistemi tarafından aralarında hiçbir fark
        göremeyecek ve birim yöneticisi işletim sistemine yanlızca
        yapılandırdığınız birim gruplarını , diskleri ve bölümleri
        gösterecektir.Bu veri içeren birimleri yönetmek için çok güçlü
        bir sistemdir.Fiziksel bölümlere ayılmış mantıksal birimler
        oluşturmaya izin verir ve bu tür birimler işletim sisteminde
        veri içeren geleneksek aygıtlar olark ortaya çıkar

    <!-- -->

    -   Bu yöneticinin ana faydaaları her şeyden öncee herhangi bri
        sayıda fiziksel birim üzerinde bir grup mantıksal birim
        oluşturabilmek ve mantıksal birimlerin kolayca ve anında yeniden
        boyutlandırılabilmesidir.

    <!-- -->

    -   Ayrıca LVM kopyalama ve ikizleme seçenekleri destekler

    <figure>
    <img
    src="Sorular%20167ee0641edc429fb2420d028dc41017/Ekran_Resmi_2023-08-14_OS_6.27.33.png"
    style="width:2672px" />
    </figure>

<!-- -->

-   `Hard lsblk `
    -   Başlıkların açıklaması
        -   `NAME`: Aygıtın adı veya kimliği.

        <!-- -->

        -   `MAJ:MIN`: Aygıtın ana ve alt numarası.

        <!-- -->

        -   `RM`: Aygıtın taşınabilirliği (1: taşınabilir, 0:
            taşınabilir değil). 1 → Bu genellikle harici diskler, USB
            bellekler veya kart okuyucular gibi taşınabilir aygıtlar
            için kullanılır. 0→ tipik olarak dahili sabit diskler veya
            ROM aygıtları gibi aygıtların taşınabilir olmadığı anlamına
            gelir.

        <!-- -->

        -   `SIZE`: Aygıtın boyutu.

        <!-- -->

        -   `RO`: Aygıtın salt okunur olup olmadığı (1: salt okunur, 0:
            salt okunur değil). 1 → aygıt salt okunurdur, yani üzerine
            yazma veya değişiklik yapmak mümkün değildir. 0→ aygıt
            yazılabilir veya değiştirilebilir demektir.

        <!-- -->

        -   `TYPE`: Aygıtın türü (örneğin disk, bölüm, ROM vb.). <span
            class="mark highlight-yellow_background">disk</span> → bir
            disk aygıtını temsil eder. Örneğin, `sda` bir disk
            aygıtıdır. <span
            class="mark highlight-yellow_background">part </span>→ bir
            disk bölümünü temsil eder. <span
            class="mark highlight-yellow_background">rom </span>→ Bu,
            bir ROM (Salt Okunur Bellek) aygıtını temsil eder.
            Örneğin, `sr0` bir ROM aygıtıdır ve genellikle bir CD/DVD
            sürücüsünü ifade eder. <span
            class="mark highlight-yellow_background">crypt</span> →Bu,
            şifrelenmiş bir bölümü temsil eder.

        <!-- -->

        -   `MOUNTPOINTS`: Bölümün bağlı olduğu nokta (örneğin dosya
            sistemi tarafından kullanılan nokta).

    <!-- -->

    -   Linux Dosya Sistemi yapısı : /boot,/home …

        `/boot`:

        -   Başlatma süreci için gerekli olan dosyaları içerir, örneğin
            çekirdek dosyası (kernel) ve başlatma yükleyici (bootloader)
            dosyaları.

        <!-- -->

        -   Örnek: `/boot/vmlinuz`, `/boot/grub`

        `/home`:

        -   Kullanıcıların kişisel dizinlerini içerir.

        <!-- -->

        -   Her kullanıcı kendi dizini altında çalışabilir.

        <!-- -->

        -   Örnek: `/home/user1`, `/home/user2`

        `/tmp`:

        -   Sistemde geçici dosya yaratma ve ortak kullanım alanı.

        <!-- -->

        -   Geçici dosyaların saklandığı dizindir.

        <!-- -->

        -   Önyükleme sırasında temizlenir.

        <!-- -->

        -   Örnek: `/tmp/tempfile`

        `/var`: Değişken verilerin (`variable data`) bulunduğu dizin.

        -   Değişen verileri ve günlük (log) dosyalarını içerir.

        <!-- -->

        -   Örnek: `/var/log`, `/var/spool`, `/var/www`

        `/srv` :

        -   Linux sistemlerinde servislerin verilerini saklamak amacıyla
            kullanılan bir dizindir.

        <!-- -->

        -   sistem dizinlerinden ayrı bir bölge olarak servis verilerini
            saklar.

        <!-- -->

        -   Örnek olarak, bir web sunucusunun veri dosyalarını
            `/srv/www` altında saklamak yaygın bir kullanım şeklidir.

        `swap` :

        -   RAM belleğinin tükendiği durumlarda sistem performansını
            düşürmeden işlemlere devam etmektir. Bellek tükenirse,
            kullanılmayan veya az kullanılan veriler swap alanına
            taşınabilir. Bu sayede daha fazla bellek benzeri alan
            sağlanır ve sistem çökmesi önlenir.

    <!-- -->

    -   `sr0`

        ROM aygıtını (CD/DVD sürücüsü gibi) temsil eder.

------------------------------------------------------------------------

**Sudo**

-   Sanal makinede "sudo" programının düzgün bir şekilde yüklendiğini
    kontrol edin.

    `dpkg -l | grep sudo`

<!-- -->

-   Değerlendirilen öğrenci, yeni kullanıcınızı "sudo" grubuna atamayı
    göstermelidir.

    `adduser yeni sudo`

<!-- -->

-   sudo'nun değerini ve işleyişini kendi seçtikleri örneklerle
    açıklamalıdır. İkinci bir adımda ise, konu tarafından getirilen
    kuralların uygulanışını size göstermelidir
    -   `sudo visudo`

    <!-- -->

    -   Sudo değeri ve işleyişi
        -   Sistem önce kullanıcının yetkilendirilip
            yetkilendirilmediğini kontrol eder.

        <!-- -->

        -   Hangi kullanıcıların hangi komutları ve hangi kullanıcıların
            hangi yetkilerle çalıştırabileceğini tanımlar.

        <!-- -->

        -   Kullanıcının `sudo` yetkilerine sahip olduğunu belirlerse,
            kullanıcıya kendi parolasını girmesi istenir.
            -   `{{kullanıcı_adı}} ALL=(ALL) ALL`
                -   İlk "ALL" (komut): Bu, `{{kullanıcı_adı}}` adlı
                    kullanıcının izin verileceği şeyi gösteriyor.

                <!-- -->

                -   İkinci "ALL" (kullanıcı): Bu, `{{kullanıcı_adı}}`
                    kullanıcısının herhangi bir kullanıcının <span
                    class="mark highlight-yellow">kimliği altında
                    </span>(<span class="mark highlight-yellow">herhangi
                    bir kullanıcı adıyla</span>) komut
                    çalıştırabilmesine izin verildiğini belirtir.

                <!-- -->

                -   Üçüncü "ALL"(Host): Bu, `{{kullanıcı_adı}}`
                    kullanıcısının herhangi bir host (sunucu) üzerinde
                    tüm <span class="mark highlight-yellow">komut
                    çalıştırabilmesine</span> izin verildiğini belirtir.

                <!-- -->

                -   Terminal Oturumu Türü Kısıtlaması Yok: Bu girişte
                    belirli bir terminal oturumu türüne dair bir
                    kısıtlama bulunmaz.

            <!-- -->

            -   `{{kullanıcı_adı}} ALL=`<span
                class="mark highlight-yellow">`(ALL : ALL)`</span>` ALL`

                <span class="mark highlight-yellow">ALL : ALL
                </span>daki 2. ALL hangi terminal üzerinde çalışmasına
                izin verdiğini belirtiyor.Yani kullanıcısının herhangi
                bir terminal oturumu türüyle (örneğin, terminal
                penceresi veya uzaktan erişim) komut çalıştırabilmesine
                izin verildiğini belirtir.

            <!-- -->

            -   `{{kullanıcı_adı}} ALL=(root : /dev/tty1) /bin/ls"`

                Bu ifade, "{{kullanıcı_adı}}" kullanıcısına sadece
                "root" kimliğiyle ve "/dev/tty1" terminalinden "/bin/ls"
                komutunu çalıştırma izni verir. Bu şekilde,
                yetkilendirmeyi daha spesifik hale getirebilirsiniz.

        <!-- -->

        -   `sudo`, çalıştırılan komutları izler ve günlüğe kaydeder.

    <!-- -->

    -   `fozerdem ALL=(ALL) NOPASSWD: /usr/local/bin/monitoring.sh `→
        NOPASSWD:" ifadesi, sudo komutlarının çalıştırılmasında parola
        gerekliliğini kaldırır. Yani,
        "[monitoring.sh](http://monitoring.sh/)" betiği sudo ile
        çalıştırıldığında, parola girmeden çalıştırılabilir.<span
        class="mark highlight-yellow"> cron 10dkda bir şifre istemesin
        diye bunu yapıyoruz otomatik çalışsın diye </span>
        -   Sudo grubunuz için güçlü bir yapılandırma oluşturmak için
            aşağıdaki gereksinimlere uymanız gerekmektedir:
            1.  Sudo kullanarak kimlik doğrulama, yanlış bir şifre
                girilmesi durumunda 3 denemeye sınırlanmalıdır. <span
                class="mark highlight-yellow">**Defaults
                passwd_tries=3**</span>

            <!-- -->

            2.  Sudo kullanılırken yanlış şifre nedeniyle bir hata
                oluşursa, isteğe bağlı olarak özel bir ileti
                görüntülenmelidir. <span
                class="mark highlight-yellow">**Defaults
                badpass_message=”Hatali Sifre Girdiniz! Lutfen Tekrar
                Giriniz.”**</span>

            <!-- -->

            3.  Sudo kullanılarak gerçekleştirilen her işlem, girdileri
                ve çıktılarıyla birlikte arşivlenmelidir. Günlük
                dosyası, /var/log/sudo/ klasöründe saklanmalıdır.

                Önce `sudo mkdir /var/log/sudo` **ile dosya oluştur**
                `sudo visudo` **içine** <span
                class="mark highlight-yellow">**Defaults
                logfile=”/var/log/sudo/sudo.log”**</span>

            <!-- -->

            4.  Güvenlik nedenleriyle TTY modu etkinleştirilmelidir.
                <span class="mark highlight-yellow">**Defaults
                requiretty**</span>

            -   tty

                **Pts ve tty arasındaki fark nedir?**

                **tty** normal bir terminal cihazıdır (örneğin
                sunucunuzdaki konsol).

                **pts**, sanal/taklit (uzak) terminal bağımlısıdır (bir
                xterm veya **ssh** bağlantısı).

                `Who `

                <figure>
                <img
                src="Sorular%20167ee0641edc429fb2420d028dc41017/Ekran_Resmi_2023-08-14_OS_8.14.39.png"
                style="width:656px" />
                </figure>

            1.  Güvenlik nedenleriyle sudo tarafından kullanılabilecek
                yollar sınırlanmalıdır. Örnek:
                /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/snap/bin
                <span class="mark highlight-yellow">**Defaults
                secure_path=”/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/snap/bin”**</span>

        <!-- -->

        -   <span
            class="mark highlight-yellow">`Defaults`</span>` log_input,log_output`

            "log_input" seçeneği, sudo komutunun kullanıcı tarafından
            girilen komutları günlüğe kaydetmesini sağlar. Bu,
            kullanıcının hangi komutları çalıştırdığını izlemek için
            yararlı olabilir.

            "log_output" seçeneği, sudo komutunun çalıştırılan komutun
            çıktısını günlüğe kaydetmesini sağlar. Bu, komutun çıktısını
            takip etmek ve olası hataları veya sorunları tespit etmek
            için kullanışlı olabilir.

        <!-- -->

        -   `defaults mail_badpass`

            Bu kural, sudoers dosyasında isteğe bağlı olarak eklenen bir
            ayar olup, yanlış parola girişlerinin izlenmesini ve
            güvenlik olaylarına hızlı bir şekilde müdahale edilmesini
            sağlamak için kullanılabilir.

        <!-- -->

        -   `defaults env_reset`

            sudo komutunun güvenli bir şekilde kullanılmasını teşvik
            etmek ve beklenmedik güvenlik açıklarını önlemek için yaygın
            olarak kullanılan bir uygulamadır.

        <!-- -->

        -   `defaults use_pty`,

            sudo komutunun bir PTY kullanarak çalışmasını sağlar,
            böylece komutlar etkileşimli bir terminal benzeri ortamda
            yürütülebilir.

<!-- -->

-   "/var/log/sudo/" klasörünün varlığını ve en az bir dosyasının
    bulunduğunu doğrulayın.

    `cat /var/log/sudo/sudo.log`

<!-- -->

-   Bu klasördeki dosyaların içeriğini kontrol edin. Bu dosyalarda sudo
    ile kullanılan komutların geçmişini görmelisiniz. Son olarak, sudo
    aracılığıyla bir komut çalıştırmayı deneyin.

    <figure>
    <img
    src="Sorular%20167ee0641edc429fb2420d028dc41017/Ekran_Resmi_2023-08-14_OS_7.24.57.png"
    style="width:1868px" />
    </figure>

    su - fozerdem

    sudo systemctl status ufw

<!-- -->

-   "/var/log/sudo/" klasöründeki dosyaların güncellendiğini gözlemleyin

------------------------------------------------------------------------

**UFW**

-   UFW" (veya "Firewalld" eğer Rocky Linux ise) programının düzgün bir
    şekilde yüklendiğini kontrol edin.

    `dpkg -l | grep ufw`

<!-- -->

-   UFW (veya Firewalld)'nin düzgün çalıştığını kontrol edin.
    `service ufw status`

    `systemctl status ufw`

<!-- -->

-   UFW deki aktif rullaara bakın port 4242 olmalı

    `sudo ufw status `

    <figure>
    <img
    src="Sorular%20167ee0641edc429fb2420d028dc41017/Ekran_Resmi_2023-08-14_OS_7.33.40.png"
    style="width:1282px" />
    </figure>

<!-- -->

-   8080 portuna izin verin check edin

    `sudo ufw allow 8080`

    `ufw status`

    ayaralr \>ağ\>gelişmiş\>b.noktası yönlendirme \> portları 8080 yap

<!-- -->

-   sonrada bu kuralı silin

    `ufw status numbered`

    <figure>
    <img
    src="Sorular%20167ee0641edc429fb2420d028dc41017/Ekran_Resmi_2023-08-14_OS_7.36.59.png"
    style="width:1476px" />
    </figure>

    `ufw delete 2 `

    `ufw status numbered`

    `ufw delete 3`

    `ufw status`

<!-- -->

-   disable

    disable -\> `systemctl disable ufw`

<!-- -->

-   inactive

    inactive → `systemctl stop ufw`

------------------------------------------------------------------------

SSH

-   sshı kontrol et inmiş mi ve çalışıyo mu

    `systemctl status ssh`

    `dpkg -l | grep ssh`

<!-- -->

-   SSH ın ne olduğunu ve AVANTAJLARI

    SSH (Secure Shell), güvenli bir uzaktan erişim protokolüdür. SSH, ağ
    üzerinden güvenli ve şifreli bir şekilde başka bir bilgisayara
    erişim sağlar. Genellikle sunuculara uzaktan bağlanmak, dosya
    transferi yapmak veya uzaktan komut çalıştırmak için kullanılır.

    SSH'nin Temel Avantajları:

    1.  **Şifreli İletişim:** SSH, iletişimi şifreleyerek verilerin
        güvenli bir şekilde aktarılmasını sağlar. Bu, hassas bilgilerin
        ağ üzerinde aktarılması sırasında güvenlik risklerini azaltır.

    <!-- -->

    2.  **Kimlik Doğrulama:** SSH, kullanıcıların ve sunucuların
        birbirlerini kimlik doğrulayarak bağlantı kurmasına olanak
        tanır. Bu, yetkisiz erişimi önlemeye yardımcı olur.

    <!-- -->

    3.  **Açık Ağlar İçin Güvenlik:** SSH, genellikle açık ağlarda
        (örneğin, internet üzerinden) güvenli bir şekilde bağlantı
        kurmak için kullanılır. Şifreli bağlantı, verilerin izinsiz
        erişimden korunmasını sağlar.

    <!-- -->

    4.  **Uzaktan Yönetim:** SSH, uzaktan sunucu veya cihaz yönetimini
        kolaylaştırır. Uzaktan komut çalıştırma ve dosya transferi gibi
        işlemler bu sayede gerçekleştirilebilir.

    <!-- -->

    5.  **Tünel Oluşturma:** SSH, verileri güvenli bir tünel üzerinden
        iletmek için kullanılabilir. Örneğin, VPN benzeri güvenli
        bağlantılar oluşturulabilir.

    <!-- -->

    6.  **Çoklu Platform Desteği:** SSH, farklı işletim sistemlerinde ve
        cihazlarda kullanılabilir. Bu, çeşitli platformlar arasında
        güvenli iletişimi sağlar.

    <!-- -->

    7.  **Anahtar Tabanlı Kimlik Doğrulama:** SSH, parola tabanlı kimlik
        doğrulama yerine anahtar tabanlı kimlik doğrulama da sağlar. Bu
        daha güvenli bir kimlik doğrulama yöntemidir.

<!-- -->

-   SSH ın sadece 4242 portunu kullandığını göster

    aklına gelmezse `find -name sshd_config` ile uzantısını bulabilirsin

    `sudo vim /etc/ssh/sshd_config` → port 4242

    -   **PermitRootLogin no**

        TERMİNALDE root@127.0.0.1 ile ağlanamıyoruz bunun sayesinde

        Sistem yöneticisinin düzenli bir kullanıcı hesabı ile giriş
        yapması ve ardından komutlarını sudo gibi izin verilen
        yetkilendirme mekanizmalarını kullanarak çalıştırması gerektiği
        anlamına gelir. Bu şekilde, hem güvenlik sağlanmış olur hem de
        her işlem için ayrı ayrı kimlik doğrulama yapılmasına olanak
        tanınır.

    `sudo systemctl restart ssh`

<!-- -->

-   <span class="mark highlight-default">Yeni oluşturulan kullanıcıyla
    SSH kullanarak oturum açmada size yardımcı olmalıdır. Bunun için
    anahtar veya basit bir şifre kullanabilirsiniz. Bu, değerlendirilen
    öğrenciye bağlı olacaktır. Tabii ki, konuda belirtildiği gibi "root"
    kullanıcısıyla SSH kullanamayacağınızdan emin olmalısınız.</span>

    yeni oluşturulan kullanıcyla terminalden bağlanma →
    `ssh kullanici@127.0.0.1 -p 4242` sıkıntı çıkarsa →
    `ssh-keygen -R '[127.0.0.1]:4242'`

<!-- -->

-   disable

    `systemctl disable ssh` → enable için `systemctl enable ssh`

<!-- -->

-   inactive

    `systemctl stop ssh` → active için `systemctl start ssh`

------------------------------------------------------------------------

CRON

-   Betik hangi işlevleri yerine getiriyor, hangi komutları içeriyor ve
    hangi sonuçları üretiyor gibi sorulara cevap vermelisiniz.

    1.  `sudo apt install -y net-tools`

    <!-- -->

    2.  `cd ``/usr/local/bin/`

    <!-- -->

    3.  `vim ``monitoring.sh`

    <!-- -->

    4.  İçine aşağğıdakileri yazıcaz Detaylı açıklıyorum:

    \#!/bin/bash → Bu satır, Bash kabuğunu kullanarak betiğin
    çalıştırılmasını sağlar.

    -   `arc=$(uname -a) ` \# Sistem mimarisini ve diğer bilgileri alır.

        `uname` → yazınca sadece işletim sistemini veriyo Linux yazıyo
        ama `uname -a` diyince komple mimariyi veriyor.

        <figure>
        <img
        src="Sorular%20167ee0641edc429fb2420d028dc41017/Ekran_Resmi_2023-08-11_OS_5.33.43.png"
        style="width:2176px" />
        </figure>

        **Linux**: İşletim sistemi çekirdek türünü gösterir.

        server1 → hostname

        • **6.1.0-10-amd64**: Çekirdek versiyonunu gösterir. Bu durumda,
        çekirdek versiyonu "6.1.0-10-amd64" olarak belirtilmiştir.

        **\#1 SMP PREEMPT_DYNAMIC**: Çekirdek yapılandırmasını ifade
        eder.

        Debian : İşletim sistemi

        **x86_64**: Sistem mimarisini ifade eder.

        **GNU/Linux**: İşletim sistemi adını belirtir.

    <!-- -->

    -   `pcpu=$(grep "physical id" /proc/cpuinfo | sort | uniq | wc -l) `\#
        Fiziksel CPU sayısını belirler.

        1.  `grep "physical id" /proc/cpuinfo`: Bu komut, /proc/cpuinfo
            dosyasını okur ve “physical id” ifadesini içeren satırları
            ayıklar. Bu satırlar, her bir fiziksel işlemciye ait
            bilgileri içerir.

        <!-- -->

        2.  `sort`: Ayıklanan satırları sıralar. Bu, aynı fiziksel
            işlemciye ait bilgilerin bir arada olmasını sağlar

        <!-- -->

        3.  `uniq`: Ardışık aynı satırları filtreler ve yalnızca
            benzersiz satırları bırakır. Bu, aynı fiziksel işlemciye ait
            bilgilerin yinelenmemesini sağlar.

        <!-- -->

        4.  `wc -l`: Bu komut, gelen satır sayısını hesaplar. Bu, toplam
            fiziksel işlemci sayısını verir.

        Sonuç olarak, bu komut dizisi size sisteminizde bulunan toplam
        fiziksel işlemci sayısını verir. Örneğin, eğer sonuç “2” ise,
        sisteminizde iki fiziksel işlemci bulunduğunu gösterir.

        <figure>
        <img
        src="Sorular%20167ee0641edc429fb2420d028dc41017/Ekran_Resmi_2023-08-11_OS_5.37.30.png"
        style="width:886px" />
        </figure>

        physical id : 0 physical id : 0 physical id : 1 physical id : 1

        Bu şekildede çıktı olabailir bu durumda 2 fiziksel kimlik vardır
        0 ve 1 bunların kimlik numarasıdır.

    <!-- -->

    -   `vcpu=$(grep "^processor" /proc/cpuinfo | wc -l) `\# Sanal CPU
        (çekirdek) sayısını belirler.

        processor kelimesinin satırın başında yer aldığı yerleri bulur
        ve satırları toplar.

    <!-- -->

    -   `fram=$(free --mega | grep Mem: | awk '{print $2}')` \# Toplam
        RAM miktarını MB cinsinden alır.

        1.  `free --mega`: Bu komut, sistemin mevcut bellek kullanımını
            ve diğer bellek istatistiklerini görüntüler. -m baytları
            <span class="mark highlight-yellow">memibaytlara ,</span>
            —mega → megabaytlara dönüştürür.

        <!-- -->

        2.  `grep Mem`:: free —mega komutunun çıktısını alır ve “Mem:”
            ifadesini içeren satırı ayıklar. Bu satır, toplam bellek
            (RAM) hakkında bilgi içerir.

        <!-- -->

        3.  `awk '{print $2}'`: grep komutunun çıktısını alır ve
            satırdaki ikinci alanı (bellek miktarını) yazdırır.

        Sonuç olarak, bu komut dizisi size sistemdeki toplam bellek
        miktarını megabayt cinsinden verir. Örneğin, eğer sonuç “8192”
        ise, sisteminizde toplam 8192 megabayt (8 gigabayt) bellek
        olduğunu gösterir.

        <figure>
        <img
        src="Sorular%20167ee0641edc429fb2420d028dc41017/Ekran_Resmi_2023-08-11_OS_5.40.25.png"
        style="width:1186px" />
        </figure>

        Burdaki swap Mem: i aşan durumlarda swap alanında kullanılan
        şeyleri içerir.

    <!-- -->

    -   `uram=$(free --mega | grep Mem: | awk '{print $3}') `\#
        Kullanılan RAM miktarını MB cinsinden alır.

    <!-- -->

    -   `pram=$(free | grep Mem: | awk '{printf("%.2f"), $3/$2*100}') `\#
        Kullanılan RAM yüzdesini hesaplar.

        free → bayt cinsinden

        `awk '{printf("%.2f"), $3/$2*100}'`: Seçilen satırı AWK
        aracılığıyla işler. Bu kısım, <span
        class="mark highlight-yellow">kullanılan belleği toplam belleğe
        bölerek bellek kullanım yüzdesini hesaplar.</span> Ardından
        `printf("%.2f")` kullanılarak yüzdeyi ondalık noktası ile iki
        basamak hassasiyetle görüntüler.

    <!-- -->

    -   `fdisk=$(df -Bg | grep '^/dev/' | grep -v '/boot$' | awk '{ft += $2} END {print ft}')`
        \# Toplam disk alanını GB cinsinden hesaplar.
        1.  `df -Bg`: Bu komut, dosya sistemi kullanımını gösterir. `B`
            seçeneği, boyutları belirli bir birimde görüntülememizi
            sağlar. `g` ise gigabayt cinsinden görüntülememizi sağlar.
            Bu komutun çıktısı, dosya sistemleri hakkında bilgi içeren
            satırları içerir.

        <!-- -->

        2.  `grep '^/dev/'`: `df` çıktısını işlerken, sadece `/dev/` ile
            başlayan disklerin bilgilerini seçer. Bu, fiziksel disklerin
            listesini almanın bir yoludur.

        <!-- -->

        3.  `grep -v '/boot$'`: Önceki adımda seçilen satırlardan,
            `/boot` ile bitenleri hariç tutar. Bu genellikle önyükleme
            bölümüdür ve sistem dosyalarını içerir.

        <!-- -->

        4.  `awk '{ft += $2} END {print ft}'`: Bu adım, seçilen
            satırlardan sütun 2'yi (dosya sistemi boyutu) alır ve
            bunları toplam disk boyutunu temsil eden bir değişkene
            (`ft`) ekler. `END` bölümünde ise toplam disk boyutunu
            yazdırır.

            <figure>
            <img
            src="Sorular%20167ee0641edc429fb2420d028dc41017/Ekran_Resmi_2023-08-11_OS_6.20.56.png"
            style="width:1182px" />
            </figure>

            10+3+3+5+3+4 = 28 2.sütünu topluyo yazdırıyor

    <!-- -->

    -   `udisk=$(df -Bm | grep '^/dev/' | grep -v '/boot$' | awk '{ut += $3} END {print ut}') `\#
        Kullanılan disk alanını MB cinsinden hesaplar.

        `df -Bm`: Bu komut, dosya sistemi kullanımını gösterir. `-B`
        seçeneği, boyutları belirli bir birimde (MB) görüntülememizi
        sağlar. `-m` ise megabayt cinsinden görüntülememizi sağlar. Bu
        komutun çıktısı, dosya sistemleri hakkında bilgi içeren
        satırları içerir.

        <figure>
        <img
        src="Sorular%20167ee0641edc429fb2420d028dc41017/Ekran_Resmi_2023-08-11_OS_6.22.42.png"
        style="width:1030px" />
        </figure>

        3.sutünü toplar yazdırır ekrana 1224

    <!-- -->

    -   `pdisk=$(df -Bm | grep '^/dev/' | grep -v '/boot$' | awk '{ut += $3} {ft+= $2} END {printf("%d"), ut/ft*100}') `\#
        Kullanılan disk alanının yüzdesini hesaplar.

        üçüncü sutün(kullanılan)toplamı /ikinci sütün(toplam boyut
        ft)toplamı \*100

    <!-- -->

    -   `cpul=$(top -bn1 | grep '^%Cpu' | cut -c 9- | xargs | awk '{printf("%.1f%%"), $1 + $3}')`
        \# CPU kullanım yüzdesini hesaplar.

        <figure>
        <img
        src="Sorular%20167ee0641edc429fb2420d028dc41017/Ekran_Resmi_2023-08-11_OS_6.31.24.png"
        style="width:1298px" />
        </figure>

        1.  `top -bn1`: Bu komut, bir kez çalıştırılan `top` komutunu
            kullanarak sistemdeki işlem ve kaynak kullanımı
            istatistiklerini görüntüler. `bn1` seçeneği, `top` komutunun
            toplamda bir kez çalıştırılmasını ve çıkışın hemen
            gösterilmesini sağlar.

        <!-- -->

        2.  `grep '^%Cpu'`: `top` çıktısını işlerken, sadece `%Cpu` ile
            başlayan satırları seçer. Bu satır, CPU kullanım
            istatistiklerini içerir.

        <!-- -->

        3.  `cut -c 9-`: Seçilen satırın 9. karakterden sonraki bölümünü
            alır. Bu, CPU kullanım yüzdesini içeren veriyi elde etmenizi
            sağlar.

        <!-- -->

        4.  `xargs`: Önceki komuttan gelen veriyi alır ve boşlukları
            çıkararak tek bir veri parçasına dönüştürür.

        <!-- -->

        5.  `awk '{printf("%.1f%%"), $1 + $3}'`: `awk` aracılığıyla
            işlenir. Bu adım, `$1` ve `$3` ifadelerini alır, bunları
            toplar ve sonucu ondalık noktasıyla birlikte yüzde
            sembolüyle birlikte yazdırır.

    <!-- -->

    -   `lb=$(who -b | awk '$1 == "sistem" {print $3 " " $4}') `\# Son
        yeniden başlatma tarihini ve saati alır.

        `who -b`: Bu komut, sistemin en son yeniden başlatıldığı tarihi
        ve saatini gösterir. Bu komutun çıktısı, sistemin yeniden
        başlatıldığı tarih ve saati içeren bir satırı içerir.

        <div class="indented">

        <figure>
        <img
        src="Sorular%20167ee0641edc429fb2420d028dc41017/Ekran_Resmi_2023-08-11_OS_6.55.33.png"
        style="width:830px" />
        </figure>

        </div>

    <!-- -->

    -   `lvmt=$(lsblk -o TYPE | grep "lvm" | wc -l)` \# LVM bölümlerinin
        sayısını belirler.

        <figure>
        <img
        src="Sorular%20167ee0641edc429fb2420d028dc41017/Ekran_Resmi_2023-08-11_OS_7.05.17.png"
        style="width:612px" />
        </figure>

        `lsblk -o TYPE`: Bu komut, disk bölümlerini listeler ve yalnızca
        "TYPE" sütununu görüntüler. "TYPE" sütunu, bölüm türünü
        belirtir.

    <!-- -->

    -   `lvmu=$(if [ $lvmt -eq 0 ]; then echo no; else echo yes; fi) `\#
        LVM kullanılıp kullanılmadığını belirler.

        Eğer lvm sayısı 0 sa no döndür 0 değilse yes döndür `fi` if
        ifadesinin sonunu belirtir.

    <!-- -->

    -   `ctcp=$(cat /proc/net/tcp | wc -l | awk '{print $1-1}') `\# TCP
        bağlantı sayısını belirler.

        <figure>
        <img
        src="Sorular%20167ee0641edc429fb2420d028dc41017/Ekran_Resmi_2023-08-11_OS_7.14.06.png"
        style="width:1844px" />
        </figure>

    <!-- -->

    -   `ulog=$(users | wc -w) `\# Anlık oturum açmış kullanıcı sayısını
        belirler.
        1.  `users`: Bu komut, anlık olarak oturum açmış kullanıcıları
            görüntüler.

        <!-- -->

        2.  `wc -w`: `wc` komutu, verilen metin veya dosyanın satır,
            kelime ve karakter sayısını sayar. `w` seçeneği, sadece
            kelime sayısını döndürmesini sağlar. Bu komut dizisi,
            `users` komutunun çıktısındaki kelime sayısını yani oturum
            açmış kullanıcı sayısını verir.

            <figure>
            <img
            src="Sorular%20167ee0641edc429fb2420d028dc41017/Ekran_Resmi_2023-08-11_OS_7.21.45.png"
            style="width:286px" />
            </figure>

    <!-- -->

    -   `mac=$(ip link show | awk '$1 == "link/ether" {print $2}') `\#
        Sistem MAC adresini alır.

        1.  `ip link show`: Bu komut, ağ arabirimlerinin (network
            interfaces) durumunu ve özelliklerini görüntüler. Bu çıktı,
            ağ arabirimlerinin farklı özelliklerini içeren satırları
            içerir.

        <!-- -->

        2.  `awk '$1 == "link/ether" {print $2}'`: Bu adım, `awk`
            komutunu kullanarak çıktıdaki satırları işler. `$1` ifadesi,
            her satırdaki ilk sütunu temsil eder. Bu komut, sadece
            "link/ether" ifadesini içeren satırları seçer, yani fiziksel
            MAC adreslerini içeren satırları.

        <!-- -->

        3.  `{print $2}`: Seçilen satırlardan ikinci sütunu yani MAC
            adresini alarak ekrana basar.

        <figure>
        <img
        src="Sorular%20167ee0641edc429fb2420d028dc41017/Ekran_Resmi_2023-08-11_OS_7.17.17.png"
        style="width:1672px" />
        </figure>

    <!-- -->

    -   `ip=$(hostname -I)` \#ip adresini yazdırır.

        sistemdeki ağ arabirimlerinin IP adreslerini döndürür

    <!-- -->

    -   `cmds=$(journalctl _COMM=sudo | grep COMMAND | wc -l)` \# Sudo
        komutlarının sayısını belirler.

        \_COMM =sudo kısmı sudo\[123\] olanları getirir systemd\[123\]
        falanda olabiliyo biz sudoları istiyoruz bide COMMAND olanlar
        sadece sudo komutu kullanmak demek diğerleri bilgi o yüzden
        onuda ayıklıyoruz

        <figure>
        <img
        src="Sorular%20167ee0641edc429fb2420d028dc41017/Ekran_Resmi_2023-08-11_OS_7.18.52.png"
        style="width:2018px" />
        </figure>

        `journalctl` aracılığıyla sistem günlüğünü incelemeyi sağlar.

        command içerenlerin sayısı döner

    <figure>
    <img
    src="Sorular%20167ee0641edc429fb2420d028dc41017/Ekran_Resmi_2023-08-24_OS_6.43.08.png"
    style="width:2374px" />
    </figure>

    \- Tcp bağlanan yer sayısını tutuyo diğer yerden bağlanınca artıyo.

<!-- -->

-   Öğrencinin hazırladığı betiği sunucu başladıktan sonra her 10
    dakikada bir çalışacak şekilde nasıl planlayacağınızı anlamalısınız.
    Bu işlemi gerçekleştirmek için "cron" kullanmanız gerekecek.

    `crontab -e`

    \# Example of job definition: \# .---------------- minute (0 - 59)
    \# \| .------------- hour (0 - 23) \# \| \| .---------- day of month
    (1 - 31) \# \| \| \| .------- month (1 - 12) OR jan,feb,mar,apr ...
    \#\| \| \| \| .----dayofweek(0-6)(Sunday=0or7) \#\|\|\|\|\| \# 10\*
    \* \* \* user-name command to be executed

    ` */10 * * * *` at <span class="mark highlight-yellow">every 10th
    minute</span> 21:10, 21:20,21:30 ,..

    `10 * * * *` at <span class="mark highlight-yellow">minute 10
    </span>21:10, 22:10,23:10 ,..

<!-- -->

-   Betiğin doğru şekilde çalıştığını doğruladıktan sonra, öğrencinin
    betiği her dakika çalışacak şekilde nasıl ayarlayacağını
    anlamalısınız.

    `*/1 * * * * ` olarak değiştir

<!-- -->

-   Sunucu başladığında betiğin otomatik olarak çalışmasını durdurmak,
    ancak betiği kendisini değiştirmeden yapmanız gerekmektedir. Bu,
    "cron" zamanlama ve betiğin yönetimiyle ilgili bir gerekliliktir.

    systemctl status cron ile hangi saaatlerde çalıştığını göerbilriiz

    <figure>
    <img
    src="Sorular%20167ee0641edc429fb2420d028dc41017/Ekran_Resmi_2023-08-14_OS_9.12.10.png"
    style="width:2220px" />
    </figure>

    `systemctl stop cron` → inactive

    `sudo cronstop`

    `sudo cronstop`

<!-- -->

-   Sunucu yeniden başlatıldığında, betiğin hala aynı yerde bulunduğunu,
    haklarının değişmediğini ve değiştirilmediğini kontrol etmeniz
    gerekecektir.

------------------------------------------------------------------------

-   Detaylar:
    -   udp dosyası silme `ss -tunlp`

        -   `ss -tunlp` kod açıklaması

            `ss -tunlp` komutu, sistemdeki TCP ve UDP bağlantılarını ve
            dinleyen portları listelemek için kullanılan bir komuttur.
            İşletim sistemine bağlı olarak, `ss` komutu genellikle
            `netstat` komutunun yerine kullanılır.

            -   `t` seçeneği, sadece TCP bağlantılarını listelemek için
                kullanılır.

            <!-- -->

            -   `u` seçeneği, sadece UDP bağlantılarını listelemek için
                kullanılır.

            <!-- -->

            -   `n` seçeneği, IP adreslerini ve port numaralarını
                sayısal formatta gösterir.

            <!-- -->

            -   `l` seçeneği, sadece dinleme (listening) portlarını
                listeler.

            <!-- -->

            -   `p` seçeneği, bağlantıya veya dinleyen porta ait işlem
                PID değerini ve program adını gösterir.

        <figure>
        <img
        src="Sorular%20167ee0641edc429fb2420d028dc41017/Ekran_Resmi_2023-08-24_OS_2.40.00.png"
        style="width:2394px" />
        </figure>

        `kill -9 563` ile udp silindi Ama geri geliyor

        <figure>
        <img
        src="Sorular%20167ee0641edc429fb2420d028dc41017/Ekran_Resmi_2023-08-24_OS_2.40.32.png"
        style="width:2392px" />
        </figure>

        →

        -   `State` (Durum): Bağlantının veya dinleyen portun durumu.
            Örneğin, "LISTEN" (dinleme), "ESTABLISHED" (kurulmuş),
            "CLOSE_WAIT" (kapanmayı bekliyor) gibi durumlar
            olabilir.`UNCONN` durumu, bir UDP bağlantısının henüz veri
            alışverişi yapmadığını veya kapatıldığını gösterir.

        <!-- -->

        -   `Recv-Q` (Alma Sırası): Bağlantı üzerinden alınmayı bekleyen
            veri miktarı.

        <!-- -->

        -   `Send-Q` (Gönderme Sırası): Bağlantı üzerinden gönderilmeyi
            bekleyen veri miktarı.

        <!-- -->

        -   `Local Address` (Yerel Adres): Bağlantının veya dinleyen
            portun yerel IP adresi ve port numarası.

        <!-- -->

        -   `Foreign Address` (Uzak Adres): Bağlantının veya dinleyen
            portun uzak IP adresi ve port numarası.

        <!-- -->

        -   `Process` (PID/Program Adı): Bağlantıya veya dinleyen porta
            ait işlem PID değeri ve program adı.

    <!-- -->

    -   Sudo neden inactive gözüküyor → arkaplanda maskeli çalışıyor.
        Sadece komutu kullandığın anda active oluyo ve sonrasında arka
        planda inactive olarak çalışıyor.

        -   change passwd

            Change password of account ( your_username).

            the command **passwd username** (where **username** is the
            name of the user whose password you want to change).

            `passwd zmahmoud`

        <!-- -->

        -   cron
            -   `sudo ``crontab -e `**→ editlemeye açıyo**

            <!-- -->

            -   `sudo ``crontab -l `**→ ekrana cronu yazdırıyor**

            <!-- -->

            -   `sudo ``crontab -u username -e` **→ istenilen user ile
                cron açıyor.**

        <!-- -->

        -   `groups username` : username in bağlı olduğu grupları
            gösterir.

        <!-- -->

        -   `gpasswd -a username groupname`  : username i groupname
            eekliyo. / `adduser username groupname` aynı işlevi yapıyor

        <!-- -->

        -   `gpasswd -d username groupname` : username i groupname den
            çıkarıyor / `deluser username groupname` aynı işevi yapar.

        <!-- -->

        -   `id -g` : shows a user’s main group ID.

        <!-- -->

        -   `id -g fozerdem` → fozerdemin group idsini gösterir.

        <!-- -->

        -   `getent group` = `cat etc/group` → ikiside tüm groupları
            gösteriyor

        <!-- -->

        -   `getent passwd` = `cat etc/passwd` → ikiside tüm userları
            gösteriyor

        <!-- -->

        -   `cut -d: -f1 /etc/group | tr '\n' ' ‘` → sadece group
            adlarını gösterir

        <!-- -->

        -   `etc/passwd` içinde kullanıcı bilgileri var `etc/group ` ta
            group bilgileri

        <!-- -->

        -   `etc/ passwd `içeriği → <span
            class="mark highlight-default">username:password:userID:groupID:geçerliAd:evKlasörü:komutShellgete</span>

        <!-- -->

        -   `usermod -aG sudo fozerdem` bunla `adduser fozerdem sudo`
            buda aynı şey

        <!-- -->

        -   `users` : giriş yapılan tüm kullanıcıları gösterir.

        <!-- -->

        -   `id -u fozerdem ` → kullanıcı idsini gösterir

        <!-- -->

        -   `userdel -r` :kullanıcı ve bağlı tüm dosyalarını siler.

        <!-- -->

        -   `chage -l  fozerdem`

            <figure>
            <img
            src="Sorular%20167ee0641edc429fb2420d028dc41017/Ekran_Resmi_2023-08-24_OO_10.14.54.png"
            style="width:1970px" />
            </figure>

        ------------------------------------------------------------------------

        <figure>
        <img
        src="Sorular%20167ee0641edc429fb2420d028dc41017/Ekran_Resmi_2023-08-24_OS_12.01.17.png"
        style="width:2382px" />
        </figure>

        üstteki scripti `bash /usr/local/bin/monitroing.sh` yazarsak
        direkt ekrana yazıyor

        ------------------------------------------------------------------------

        → dosya oluştur içine 1 2 3 4 5 6 7 8 9 yaz ve bunun bir
        sütununu ekrana yazdır

        → `awk ‘{printf(”%d”, $1)}’ deneme.txt`
        or` awk '{print $1}' deneme.txt`

        → satır yazdırmak için → `head -n 1 deneme.txt`

        ------------------------------------------------------------------------

        `export a=ls` → a ya ls komutu atıyosun environment

        `$a` → yazınca ls komutu çalışıyor.

------------------------------------------------------------------------

</div>
