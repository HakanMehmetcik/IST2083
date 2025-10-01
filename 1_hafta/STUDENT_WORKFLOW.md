# STUDENT_WORKFLOW — IST2083

Bu belge öğrencilerin **orijinal dersi klonlayıp**, kendi çalışmalarını **kendi depolarında** güvenle saklaması için kısa akışı özetler. Amaç: **Orijinal repoyu bozmadan** güncel kalmak + kendi işini versiyonlamak.

------------------------------------------------------------------------

## 0) Gerekli yazılımlar

-   **Git**, **R**, **RStudio** (kurulum için bkz: Onboarding rehberi)
-   (İsteğe bağlı) **GitHub hesabı** — *B akışı için gerekli*

------------------------------------------------------------------------

## 1) Ders deposunu klonla (salt okunur)

**RStudio → File → New Project → Version Control → Git** - Repository URL: `https://github.com/HakanMehmetcik/IST2083.git` - Create Project

> Alternatif (Terminal):\
> `git clone https://github.com/HakanMehmetcik/IST2083.git`

------------------------------------------------------------------------

## 2) ÖNERİLEN AKIŞ — “origin = benim depom”, “upstream = ders deposu”

> Bu akış, **kendi çalışmalarınızı GitHub’da yedeklerken** ders deposundan **güncellemeleri kolayca çekmenizi** sağlar.

### 2.1 GitHub’da **boş bir repo** oluştur (öğrenci hesabında)

Örn: `IST2083-works` (private önerilir).

### 2.2 Remote’ları ayarla (RStudio Terminal’de)

``` bash
# 1) Orijinal ders repounu "upstream" olarak adlandır
git remote rename origin upstream

# 2) Kendi boş deponu "origin" olarak ekle
git remote add origin https://github.com/<kullanici>/IST2083-works.git

# 3) İlk push (main dalı kendi repona)
git push -u origin main
```

### 2.3 Güncel kalma (her hafta)

``` bash
git pull upstream main   # dersteki güncellemeleri al
git push origin main     # kendi depona da gönder
```

> **Not:** Çalışmalarınızı `analysis/`, `notes/`, `homework/` gibi **yeni klasörlerde** tutun; orijinal materyalleri silmeyin/taşımayın.

------------------------------------------------------------------------

## 3) ALTERNATİF — Fork akışı (isteğe bağlı)

-   GitHub’da dersi **Fork** et → **kendi fork’unu** klonla.
-   `git remote add upstream https://github.com/HakanMehmetcik/IST2083.git`
-   `git pull upstream main` ile günceli al; `git push origin main` ile fork’una gönder.

------------------------------------------------------------------------

## 4) RStudio ile günlük kullanım

-   **Çalış** → dosya ekle/değiştir
-   **Git paneli** → `Stage` → `Commit` (anlamlı mesajlarla)
-   **Pull** (upstream’den), ardından **Push** (origin’e)\
    \> Pull düğmesi upstream’i değil origin’i çekiyorsa Terminal komutlarını kullanın (bkz. 2.3).

------------------------------------------------------------------------

## 5) Önerilen `.gitignore` (kısaltılmış)

```         
.Rproj.user/
.Rhistory
.RData
.Ruserdata
.quarto/
_site/
_freeze/
.vscode/
*.html
*.pdf
outputs/
tmp/
data/raw/*
!data/raw/README.md
```

------------------------------------------------------------------------

## 6) Sıkça karşılaşılanlar

-   **Pull yaparken çakışma (merge conflict)**: Değiştirdiğiniz dosya derste de güncellendiyse oluşur.
    -   `git status` ile çatışan dosyayı görün, işaretli yerleri düzenleyip `git add` → `git commit`.
-   **RStudio Git görünmüyor**: `Tools → Global Options → Git/SVN` altında Git yolunu doğrulayın; RStudio’yu yeniden başlatın.
-   **HTTPS/SSH hataları**: HTTPS URL kullanın; kurum ağında SSL sorunları için ev ağında deneyin.

------------------------------------------------------------------------

## 7) Hızlı kontrol listesi

-   [ ] Repoyu **klonladım** (salt-okunur)
-   [ ] **origin = kendi repo**, **upstream = ders repo** ayarlandı
-   [ ] Commit’lerimi **origin**’e **push** edebiliyorum
-   [ ] Dersten **upstream pull** ile güncelleme alabiliyorum
-   [ ] Çalışmalarımı **ayrı klasörlerde** tutuyorum

> Sorunda ekran görüntüsü ile mesaj atın: `git status` çıktısı + hata metni çözümü hızlandırır.
