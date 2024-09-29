# **GitHub ve GitHub Codespaces Kullanım Kılavuzu**

Bu kılavuz, **IST2083** dersi boyunca GitHub ve GitHub Codespaces kullanarak ders materyallerine erişim sağlamanızı ve bu araçlarla nasıl çalışabileceğinizi adım adım gösterecektir.

## **1. GitHub’a Kaydolma ve Giriş Yapma**

Ders materyallerine erişebilmek için öncelikle bir **GitHub** hesabına ihtiyacınız olacak. Eğer henüz bir GitHub hesabınız yoksa, şu adımları takip ederek kolayca kaydolabilirsiniz:

### **1.1 GitHub’a Kaydolma:**

1. [GitHub](https://github.com) web sitesine gidin.
2. Sağ üst köşedeki **"Sign up"** butonuna tıklayın.
3. Kullanıcı adı, e-posta ve şifre bilgilerinizi doldurarak bir hesap oluşturun.

### **1.2 GitHub’a Giriş Yapma:**

1. GitHub hesabınızı oluşturduktan sonra [GitHub](https://github.com) web sitesinde sağ üst köşedeki **"Sign in"** butonuna tıklayın.
2. GitHub kullanıcı adınız ve şifrenizle giriş yapın.

---

## **2. Ders Repository'sine Erişim**

Ders materyalleri, Quarto dosyaları ve veri setlerine ulaşmak için **IST2083 GitHub Repository**'sini kullanacaksınız. Bu repository’de haftalık ders konuları ve ilgili materyaller düzenli olarak paylaşılacaktır.

### **2.1 Repository'ye Gitmek:**

1. Ders materyallerine erişmek için [IST2083 GitHub Repository](https://github.com/HakanMehmetcik/IST2083.git) sayfasına gidin.
2. Bu sayfa üzerinden haftalık dosyalara, veri setlerine ve diğer materyallere ulaşabilirsiniz.

### **2.2 Repository'nin Yapısı:**

- **qmd Dosyaları:** Her haftanın ders notları, R kodları ve açıklamalarını içeren Quarto formatındaki dosyalar.
- **Veri Setleri:** Haftalık analizlerde kullanacağınız veri setleri bu bölümde yer alacaktır.
- **Ders İzlencesi:** Dönem boyunca takip edeceğiniz ders programı.

---

## **3. GitHub Repository'yi Bilgisayarınıza Klonlama**

Repository’deki materyalleri yerel bilgisayarınıza indirip üzerinde çalışmak istiyorsanız, repository’yi klonlamanız gerekir. GitHub üzerinden bir repository’yi klonlamak için şu adımları takip edin:

### **3.1 Repository’yi Klonlama:**

1. Repository sayfasında sağ üst köşedeki **"Code"** butonuna tıklayın.
2. **"HTTPS"** seçeneğini seçin ve kopya simgesine tıklayarak URL’yi kopyalayın.
3. Bilgisayarınızda Git'i açın ve aşağıdaki komutu kullanarak repository’yi klonlayın:

   ```bash
   git clone https://github.com/HakanMehmetcik/IST2083.git
   ```

4. Bu komut, repository'nin tüm dosyalarını bilgisayarınıza indirir. Klonladığınız dosyalara yerel bilgisayarınızdan ulaşabilirsiniz.

---

## **4. GitHub Codespaces ile Çalışma**

GitHub Codespaces, bulut üzerinde doğrudan çalışmanıza olanak sağlayan güçlü bir geliştirme ortamıdır. Bilgisayarınıza herhangi bir yazılım kurmadan GitHub Codespaces ile RStudio benzeri bir ortamda ders materyalleriyle çalışabilirsiniz.

### **4.1 GitHub Codespaces’i Açma:**

1. **IST2083 GitHub Repository** sayfasına gidin.
2. Sağ üst köşedeki **"Code"** butonuna tıklayın.
3. Açılan menüde **"Open with Codespaces"** seçeneğine tıklayın.
4. Eğer Codespace oluşturulmamışsa, **"Create Codespace on main"** butonuna tıklayın.
5. Codespace açıldığında, bir geliştirme ortamında Quarto dosyaları üzerinde çalışabilirsiniz.

### **4.2 Codespaces Ortamında Çalışma:**

- **Kodlarınızı Çalıştırma:** Quarto dosyalarındaki R kodlarını direkt çalıştırabilir ve sonuçları görebilirsiniz.
- **Grafik Oluşturma:** RStudio gibi, Codespaces’te de grafiklerinizi anında görselleştirebilirsiniz.
- **Veri Setleri Üzerinde Çalışma:** Repository’de yer alan veri setlerini kullanarak veri analizi yapabilirsiniz.

---

## **5. Quarto ve R ile Çalışma**

Repository’deki her hafta için hazırlanmış `.qmd` (Quarto) dosyalarını düzenleyerek ve çalıştırarak ders materyallerine erişebilirsiniz.

### **5.1 Quarto Dosyalarını Düzenleme:**

- Codespaces veya RStudio üzerinde `.qmd` dosyalarını açın.
- Bu dosyalar ders notları, R kodları ve veri setleri içerir.
- Kendi notlarınızı ekleyebilir veya kodlar üzerinde değişiklik yapabilirsiniz.

### **5.2 R Kodlarını Çalıştırma:**

- Quarto dosyaları içinde yer alan R kodlarını **konsol** üzerinden çalıştırarak sonuçları anında görebilirsiniz.
- Her hafta üzerinde çalışmanız gereken veri setleri de bu dosyalarda yer alacak.

---

## **6. Güncellemeleri Takip Etme**

Ders materyalleri ve veri setleri düzenli olarak güncellenecek. Bu güncellemeleri takip etmek için repository'yi güncellemeniz gerekecek.

### **6.1 GitHub Repository’yi Güncelleme:**

1. Bilgisayarınıza klonladığınız repository’yi güncel tutmak için şu komutu kullanabilirsiniz:

   ```bash
   git pull
   ```

2. Bu komut, öğretim üyesi tarafından yapılan tüm güncellemeleri yerel bilgisayarınıza indirir.

---

## **7. GitHub Student Developer Pack’e Başvuru**

GitHub Codespaces’i ücretsiz kullanabilmek için **GitHub Student Developer Pack**'e başvurmanız gerekecek.

### **7.1 GitHub Student Developer Pack’e Nasıl Başvurulur?**

1. [GitHub Student Developer Pack](https://education.github.com/pack) sayfasına gidin.
2. GitHub hesabınızla giriş yapın.
3. **"Get Your Pack"** butonuna tıklayarak öğrenci olduğunuzu doğrulamak için gerekli adımları izleyin:
   - Üniversitenize ait e-posta adresini kullanın **veya**
   - Öğrenci kimliği veya belgenizi yükleyerek doğrulama yapın.

4. Başvurunuz birkaç gün içinde onaylanacaktır.

---

## **8. Yardım ve Destek**

GitHub ve GitHub Codespaces kullanımıyla ilgili herhangi bir sorununuz olursa aşağıdaki adımları izleyebilirsiniz:

1. GitHub’ın yardım sayfasına göz atın: [GitHub Docs](https://docs.github.com)
2. Dersin öğretim asistanına veya öğretim üyesine e-posta yoluyla ulaşabilirsiniz.
3. GitHub destek ekibine başvurarak sorunlarınızı iletebilirsiniz.

---

Bu kılavuzla, GitHub ve GitHub Codespaces’i kullanarak ders materyallerine erişebilir ve üzerinde çalışabilirsiniz. Hem bulut tabanlı hem de yerel ortamda çalışmanıza imkan veren bu araçlar, dersteki çalışmalarınızı kolaylaştıracaktır.

Başarılar!