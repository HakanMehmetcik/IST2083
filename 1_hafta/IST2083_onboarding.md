# IST2083 — Öğrenci Kurulum & Kullanım Kılavuzu

Bu doküman, ders materyallerine **GitHub deposu** üzerinden erişmeniz için adım adım bir rehberdir. Depo **salt-okunur** kullanılacak; lütfen **değişiklik (commit/push)** yapmayın.

------------------------------------------------------------------------

## 0) Gereksinimler (Kısa Liste)

-   **R** (4.3+ önerilir) ve **RStudio** (2023+ önerilir) yüklü olmalı.
-   **Git** kurulu olmalı (aşağıda anlatılıyor).
-   Bir **GitHub hesabı** (ücretsiz).

> Not: Depo **genel (public)** olduğu için *klonlama* ve *güncelleme (pull)* için giriş yapmanız gerekmez. (Yazma izniniz yoktur.)

------------------------------------------------------------------------

## 1) Git Kurulumu

### Windows

1.  <https://gitforwindows.org> adresinden **Git for Windows** indirin ve kurun.
2.  Kurulum sihirbazında varsayılan ayarlar uygundur. (Öneri: *Checkout Windows-style, commit Unix-style*)
3.  Kurulumdan sonra **RStudio’yu yeniden başlatın**.

### macOS

-   En hızlı yol: Terminal’de `xcode-select --install` komutunu çalıştırın ve **Command Line Tools**’u yükleyin.\
    *Alternatif:* Homebrew kullanıyorsanız `brew install git`.
-   Kurulumdan sonra **RStudio’yu yeniden başlatın**.

### Linux

-   Debian/Ubuntu: `sudo apt-get update && sudo apt-get install -y git`
-   Fedora: `sudo dnf install -y git`
-   Arch: `sudo pacman -S git`

> Kontrol: Terminal veya RStudio Terminal’inde `git --version` komutunun sürüm döndürdüğünü doğrulayın.

------------------------------------------------------------------------

## 2) GitHub Hesabı Açma (Gerekirse)

1.  <https://github.com/> adresinden **Sign up** ile ücretsiz hesap oluşturun.
2.  Profil e-postanızı doğrulayın.
3.  (İsteğe bağlı) Profil adınızı düzenleyin.

> Bu ders için repoya **yazma izniniz yok**; hesabınız olmasa da klon/pull yapabilirsiniz. Ancak ileride ödev/katkı süreçleri için hesap gerekebilir.

------------------------------------------------------------------------

## 3) Git’i Kimlik Bilgilerinizle Tanıtma (Önerilir)

Terminal (veya RStudio Terminal) açın ve ad/eposta tanımlayın:

``` bash
git config --global user.name "Ad Soyad"
git config --global user.email "eposta@ornek.com"
```

> Bu ayar, yerel commit geçmişinizin doğru görünmesini sağlar. Yazma izniniz olmadığı için **push** yapmayacaksınız; bu ayar zorunlu değildir ama tavsiye edilir.

------------------------------------------------------------------------

## 4) R ve RStudio

-   R’ı <https://cran.r-project.org/> adresinden yükleyin.
-   RStudio’yu <https://posit.co/download/> adresinden yükleyin.
-   RStudio’da **Git’i algılatma**: `Tools → Global Options → Git/SVN` altında **Enable version control interface for RStudio projects** işaretli olmalı ve **Git executable** yolu dolu görünmeli. Boşsa Git kurulumunu kontrol edin ve RStudio’yu yeniden başlatın.

------------------------------------------------------------------------

## 5) Depoyu RStudio İçine Klonlama (Önerilen Yol)

1.  RStudio’yu açın → **File → New Project…**
2.  **Version Control**’ü seçin.
3.  **Git**’i seçin.
4.  **Repository URL** alanına şu adresi yapıştırın:\
    `https://github.com/HakanMehmetcik/IST2083.git`
5.  **Project directory name** otomatik dolacaktır (`IST2083`). İsterseniz değiştirin.
6.  **Create project as a subdirectory of:** altında proje klasörünüzü seçin (ör. `Documents/R/`).
7.  **Create Project**’e tıklayın.

RStudio, projeyi açtığında sağ üstte **Git** panelini göreceksiniz (History, Diff, Pull, …).

### Alternatif: Komut Satırı ile Klonlama

Terminal’de (klonlamak istediğiniz klasöre giderek):

``` bash
git clone https://github.com/HakanMehmetcik/IST2083.git
```

Sonra RStudio’dan **File → Open Project…** ile klonlanan klasördeki `.Rproj` dosyasını açın.

------------------------------------------------------------------------

## 6) Güncellemeleri Çekme (Pull)

-   RStudio’da **Git panelindeki “Pull”** düğmesine tıklayın.

-   Terminal’den yapmak isterseniz:

    ``` bash
    cd IST2083
    git pull origin main
    ```

    > Ders materyallerindeki değişiklikler periyodik olarak repoya işlenecektir. **Push/commit yapmayın.**

------------------------------------------------------------------------

## 7) “Salt-Okunur” Kullanım Kuralları

-   Bu depo **ders materyalleri içindir**. Lütfen:
    -   **Değişiklik yapmayın** (commit/push).
    -   Kendi denemeleriniz için **bilgisayarınızda ayrı bir klasörde** çalışın veya **kendi özel deponuzu** oluşturun.
-   Repo açık (public) olduğu için **fork** edebilirsiniz; bu, **asıl depoyu etkilemez**.

------------------------------------------------------------------------

## 8) Sık Karşılaşılan Hatalar ve Çözümler

**A) “Git not found” / RStudio Git’i görmüyor**\
- Git’i kurduğunuzdan ve RStudio’yu **yeniden başlattığınızdan** emin olun.\
- `Tools → Global Options → Git/SVN` altında **Git executable** yolunu kontrol edin.

**B) “Permission denied (publickey)”**\
- SSH adresi yerine **HTTPS URL** kullandığınızdan emin olun:\
`https://github.com/HakanMehmetcik/IST2083.git`

**C) “fatal: not a git repository”**\
- Komutu doğru klasörde çalıştırın (`IST2083` klasöründe).\
- Gerekirse `git status` ile kontrol edin.

**D) “already exists and not an empty directory”**\
- Aynı isimli klasör zaten varsa, ya **silin/taşıyın** ya da yeni bir **Project directory name** seçin.

**E) “SSL certificate problem”** (nadir / kurum ağı)\
- Kurum ağı/proxy nedeniyle olabilir. Ev ağında deneyin veya BT birimiyle iletişime geçin.

------------------------------------------------------------------------

## 9) (İsteğe Bağlı) GitHub’da Sürüm Takibi

-   Repoyu **Watch → Custom → Releases** olarak ayarlarsanız, yayınlanan sürümler (ör. `v1.0-week1`) için bildirim alırsınız.

------------------------------------------------------------------------

## 10) Kontrol Listesi (2 Dakikalık Özet)

-   [ ] Git yüklü, `git --version` çalışıyor
-   [ ] R ve RStudio yüklü
-   [ ] RStudio, `Tools → Global Options → Git/SVN` altında Git’i görüyor
-   [ ] **New Project → Version Control → Git** ile `IST2083` klonlandı
-   [ ] Güncelleme için: **Pull**

> Takıldığınız noktada önce bu kılavuzdaki “Sık Hatalar” bölümüne bakın; çözülmezse asistanlara/hocaya ekran görüntüsü ile sorun.
