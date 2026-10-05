## LİNUX TEMELLERİ
Linux açık kaynak kodlu, UNIX tabanlı, Linux çekirdeğine dayalı, herkesin indirip kullanabileceği hatta aslında herkesin kendi versiyonlarını ve dağıtımlarını çıkarabileceği, ücretsiz bir işletim sistemidir.
Ayrıca Android işletim sistemi de Linux çekirdeği üzerinde çalışmaktadır. Bu nedenle mobil cihazlarda da kullanıyoruz.

- > Çekirdek (Kernel): Donanım (işlemci, bellek) ile yazılım süreçlerini yöneten sistemin merkezidir.

- >Kabuk (Shell): Kullanıcının komutları sisteme iletmesini sağlayan arayüzdür.

- >Dağıtımlar (Distro): Linux çekirdeğinin masaüstü, paket yöneticisi ve uygulamalarla birleştirilmiş halidir (Ubuntu, Debian, Fedora, Arch Linux gibi).

# Linux Tarihçesi ve Amacı

Linux, 1991 yılında ismi ilk geliştiricisi olan Linus Torvalds adlı bir Fin üniversite öğrencisi tarafından, daha eski işletim sistemlerinden birisi olan UNIX’in mimarisine ve POSIX standartlarına uygun bir şekilde sıfırdan yazılmaya başlanmıştır. Linux Vakfı çatısı altında geliştirilen bir yazılım projesidir.

Linux’tan önce, 1984 yılında ise yine aynı prensiplere dayanarak bir işletim sistemini özgür yazılım projesi olarak geliştirmek isteyen Richard Stallman, GNU Projesi adı verdiği işletim sistemi geliştirme projesi araçları hazır ama çekirdek yazılımı eksikti. 1992 yılında Linus Torvalds geliştirdiği çekirdek yazılımı ile katkıcının desteğini alabilmek adına özgür yazılım olan GNU Genel Kamu Lisansı ile yayınlama kararı aldı. Böylelikle bu iki ayrı proje birbirinin eksik kalan yanlarını tamamlamış oldu ve tam bir işletim sistemi olarak sunulabilir hale geldi. Ardından 1994 yılında GNU bülteninde “Özgür UNIX Benzeri” olarak duyuruldu. 1995 yılında ise ticari alanda da kullanılmaya başlandı.

Bu olay Linux için en önemli kırılma noktası oldu. Sonrasında dünya genelinden pek çok gönüllü uzmanın katkısını almayı başardı.

#Neden Tercih Edilmeli?

2000’li yıllardan sonra internetin gerek evlere gerek işletmelere kadar yaygınlaşmasıyla geniş internet alt yapısına ve farklı özellikteki ağ cihazlarına olan ihtiyaç artış gösterdi. Burada da Linux’un sınırsızca özelleştirilebiliyor olması ve ücretsiz sunulması üreticiler tarafından fazlasıyla tercih edilmesine neden oldu.

Bunun yanında güvenlik açısından baktığımızda; virüslere, kötü amaçlı yazılımlara ve çökmelere karşı koruma sağlayan çeşitli güvenlik seçeneklerini desteklemesinin bize artısı var.

Açık kaynaklı bir sistem olduğu için kaynak koduna erişim ile lisansa uygun olarak inceleyebilir değiştirebilir bu değişiklikleri yayınlayabilirsiniz. Linux’un neredeyse bütün popüler programlama dillerini destekliyor olması da bize yarar sağlar.

## Temel Linux Terminal Komutları

# Dosya ve Dizin Gezinme Komutları

- pwd (Print Working Directory): Şu anda hangi klasörde (dizinde) olduğunuzu gösterir.

- ls (List): Bulunduğunuz dizindeki dosya ve klasörleri listeler.

- cd (Change Directory): Dizin değiştirmenizi sağlar.

- cd /klasor_adi: Belirtilen klasöre geçer.

- cd ..: Bir üst dizine çıkar.

- cd ~ veya sadece cd: Kullanıcının ana dizinine (Home) döner.

# Dosya ve Klasör Yönetimi

- mkdir (Make Directory): Yeni bir klasör oluşturur.

- touch: Boş bir dosya oluşturur veya var olan dosyanın erişim zamanını günceller.

- rm (Remove): Dosya veya klasör siler.

- rm dosya.txt: Dosyayı siler.

- rm -r klasor_adi: Klasörü ve içindekileri özyinelemeli (recursive) olarak siler.

- rm -rf klasor_adi: Uyarı vermeden zorla siler (dikkatli kullanılmalıdır).

- cp (Copy): Dosya veya klasör kopyalar.

- cp -r kaynak_klasor hedef_klasor: Klasör kopyalamak için -r parametresi kullanılır.

- mv (Move): Dosya veya klasörleri taşır ya da adını değiştirir.

# Dosya İçeriği ve Metin Görüntüleme

- cat (Concatenate): Dosya içeriğini terminal ekranına yazdırır.

- nano / vim: Terminal tabanlı metin düzenleyicileridir. Dosya düzenlemek için kullanılır.

- head ve tail: Dosyanın başındaki veya sonundaki satırları gösterir.

- tail -f log.txt: Dosyaya eklenen yeni satırları canlı olarak takip eder.

- grep: Dosyalar içinde belirli bir metni arar.

# Sistem, Kullanıcı ve İzin Yönetimi

- sudo (Superuser Do): Komutları sistem yöneticisi (root) yetkileriyle çalıştırmayı sağlar.

- chmod: Dosya veya klasör erişim izinlerini değiştirir.

- chown: Dosyanın sahibini veya grubunu değiştirir.

- whoami: Şu anda oturum açmış olan kullanıcı adını gösterir.


# Sistem Bilgisi ve Ağ Komutları

- top / htop: Çalışan süreçleri (process) ve sistem kaynak kullanımını (CPU, RAM) canlı olarak listeler.

- df -h: Disk alan kullanımını insan tarafından okunabilir biçimde (GB, MB) gösterir.

- free -h: Kullanılabilir ve kullanılan RAM miktarını gösterir.

- ping: Bir sunucuya ağ bağlantısını ve yanıt süresini test eder.

- ip a / ifconfig: Ağ arayüzlerini ve IP adreslerini görüntüler.

# Pratik ve Yardımcı Komutlar
- clear: Terminal ekranını temizler (kısayol: Ctrl + L).

- history: Daha önce çalıştırılan komutların geçmişini listeler.

- man (Manual): Herhangi bir komutun kullanım kılavuzunu açar.

## Temel Dosya Hiyerarşisi

• /bin: Kullanıcı komutlarını barındırır.
• /etc: Ayar ve konfigürasyon dosyalarını tutar.
• /home: Kullanıcıların kişisel dosyalarının bulunduğu dizindir.
• /dev: Donanım dosyalarını kapsar.
• /var: Log ve geçici değişim gösteren dosyaları saklar.


## Linux'ta Süreç (Process) ve Bellek Yönetimi

İşletim sisteminin çalışan her bir programa fiziksel ve sanal bellek(RAM) alanları ataması, bu alanları düzenlemesi ve işlevleri bittiğinde temizlemesidir.

# Temel Kavramlar ve Bileşenler

• Sanal Bellek : Linux, her prosese gerçek RAM boyutundan bağımsız olarak sanki tüm bellek kendisine aitmiş gibi özel ve kesintisiz bir sanal adres alanı sunar.
• Bellek Sayfaları : Bellek yönetimi, RAM'i genellikle 4 KB'lık küçük parçalara (sayfalara) bölerek yönetir.
• Talep Üzerine Sayfalama : Bir proses çalıştırıldığında tümü birden RAM'e yüklenmez; yalnızca ihtiyaç duyulan kısımlar diskten belleğe getirilir.
• Swap Alanı: Fiziksel RAM dolduğunda, aktif olmayan veriler geçici olarak sabit disk üzerindeki takas (swap) alanına taşınır.

# Process Bellek Alanı Yapısı

Her Linux prosesinin sanal bellek uzayı belirli bölümlere ayrılır:

• Text (Kod) Alanı: Programın çalıştırılabilir makine komutlarını barındırır.
• Data Alanı: Başlangıç değeri atanmış global ve statik değişkenleri tutar.
• BSS Alanı: Değeri atanmamış global ve statik değişkenler için ayrılır.
• Heap (Yığın) Alanı: Çalışma zamanında dinamik olarak büyüyüp küçülen bellek alanıdır.
• Stack (Yığın/Çağrı) Alanı: Yerel (local) değişkenleri ve fonksiyon çağrı bilgilerini saklar.

## Paket Yönetimi
Linux paket yönetimi, işletim sistemindeki yazılımların kurulmasını, güncellenmesini, kaldırılmasını ve yönetilmesini sağlayan sistemlerin genel adıdır. Windows'taki ".exe " dosyalarını tek te internetten indirmek yerine merkezi kaynaklardan (depolardan) güvenli ve tek komutla işlem yapmanızı sağlar.

# Temel Görevleri

- Programları ve gerekli dosyaları sisteme ekler.

- Bir programın çalışması için gereken diğer alt kütüphaneleri otomatik olarak bulur ve kurar.

- Yüklü uygulamaları tek merkezden güncel tutar.

- Artık gerekmeyen programları ve kalıntılarını sistemden temizler.

# Paket Yöneticileri ve Dağıtımlar

•  APT (Advanced Package Tool) / dpkg: Ubuntu, Debian ve Linux Mint gibi dağıtımlarda kullanılır. 

-Örnek komut: sudo apt install paket_adi

• DNF / YUM / RPM: Fedora, Red Hat (RHEL) ve CentOS sistemlerinde görev yapar. 

-Örnek komut: sudo dnf install paket_adi

• Pacman: Arch Linux ve Manjaro gibi dağıtımların tercih ettiği hızlı yöneticidir.

 -Örnek komut: sudo pacman -S paket_adi

## Dosya İzinleri

Bir dosya veya dizine kimlerin erişebileceğini, içeriğini okuyabileceğini, değiştirebileceğini veya çalıştırabileceğini belirleyen güvenlik kurallarıdır.

# Temel İzin Türleri
Linux'ta üç temel izin vardır:

• Okuma (Read - r): Dosya içeriğini okuma veya klasör içindekileri listeleme. Değeri 4'tür.

• Yazma (Write - w): Dosyayı değiştirme/silme veya klasör içinde dosya oluşturma/silme. Değeri 2'dir.

• Çalıştırma (Execute - x): Dosyayı (betik veya program) çalıştırma veya klasörün içine girme. Değeri 1'dir.

# Kullanıcı Grupları
İzinler üç farklı sınıf için ayrı ayrı tanımlanır.

• Sahip (User - u): Dosyayı oluşturan kişi.
• Grup (Group - g): Dosyanın ait olduğu kullanıcı grubu.
• Diğerleri (Others - o): Sahip ve grup dışındaki herkes.

- İzinleri görmek için terminale "ls -l " yazılır.
- İzinleri değiştirmek için "chmod" komutu kullanılır.

## systemctl nedir?

Arka planda çalışan servislerin (deamon), sistem durumlarını, hedef (target) bileşenleri ve donanım/güç yönetimini denetlememizi sağlar. Eskiden ayrı ayrı yapılan servis yönetimi ve başlangıç ayarları işlemlerini tek bir komut altında birleştirir.

# Temel Kullanım ve Komutlar

Günlük sistem yönetiminde en çok kullanılan systemctl komutları şunlardır:

• Servis Durumunu Kontrol Etme: 
systemctl status servis_adi (Çalışıp çalışmadığını, hata kayıtlarını ve aktiflik durumunu gösterir).

• Servis Başlatma:
 sudo systemctl start servis_adi (Durdurulmuş bir servisi çalıştırır).

• Servis Durdurma: 
sudo systemctl stop servis_adi (Çalışan bir servisi durdurur).

• Servis Yeniden Başlatma:
 sudo systemctl restart servis_adi (Servisi durdurup tekrar başlatır).

• Sistem Açılışında Otomatik Başlatma (Enable): sudo systemctl enable servis_adi (Bilgisayar her açıldığında servisin otomatik başlamasını sağlar).

• Otomatik Başlatmayı Kapatma (Disable):
 sudo systemctl disable servis_adi (Servisin açılışta otomatik başlamasını engeller).

• Aktif Servisleri Listeleme: 
systemctl list-units --type=service (Sistemde çalışan veya tanımlı tüm servisleri gösterir)

## Kali Linux Nedir?

Kali Linux, Offensive Security tarafından geliştirilen ve sürdürülen açık kaynaklı bir Linux dağıtımıdır. İlk olarak 2013 yılında, önceki bir sızma testi dağıtımı olan BackTrack Linux'un halefi olarak piyasaya sürülmüştür. Kali Linux, siber güvenlik uzmanlarının sızma testleri ve güvenlik denetimleri yapmak için kullandığı özel bir Linux işletim sistemi dağıtımıdır. Tamamen ücretsizdir ve herkes tarafından geliştirilebilir.

# Kali Linux İle Neler Yapılabilir?

- Günlükleri analiz etme, silinen dosyaları kurtarma ve etkinlikleri izleme araçlarıyla Kali Linux, dijital adli soruşturmalarda sıklıkla kullanılır.

- Kali Linux, Wi-Fi şifrelerini kırmak ve WPA/WPA2 güvenlik açıklarını test etmek için Aircrack-ng gibi araçlarla gelişmiş kablosuz ağ testlerini destekler.

- Kali Linux'taki Ghidra ve Radare2 gibi araçlar ikili kodu analiz etmek, uygulamaları derlemek ve yazılımda hata ayıklamak için kullanılır.

- Araştırmacılar Kali Linux'u güvenlik önlemlerinin etkinliğini test etmek, kötü amaçlı yazılım davranışını incelemek ve yeni bilgisayar korsanlığı teknikleri geliştirmek için kullanılır.
