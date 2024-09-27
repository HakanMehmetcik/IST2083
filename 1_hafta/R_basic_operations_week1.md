
# **R Konsolu ve Temel Aritmetik İşlemler**

R, bir programlama dili olmasının yanı sıra, aynı zamanda bir hesap makinesi gibi basit matematiksel işlemler yapabileceğiniz bir ortam sağlar. R konsolunu kullanarak basit komutları hemen çalıştırabilirsiniz. Aşağıda R konsolunda nasıl çalışacağınızı ve temel matematiksel işlemleri nasıl gerçekleştireceğinizi öğreneceksiniz.

## **R Konsolunu Kullanarak Basit Komutlar Çalıştırma**

GitHub Codespaces’te R konsolunu açarak komutlar yazabilirsiniz. R konsolu, yazdığınız her komutu anında çalıştırır ve size sonucu gösterir. Örneğin, R konsoluna aşağıdaki gibi bir toplama işlemi yazabilirsiniz:

```r
3 + 5
```

Bu komutu çalıştırdığınızda, R size işlemin sonucunu gösterecektir:

```r
[1] 8
```

## **Temel Matematiksel İşlemler**

R, toplama, çıkarma, çarpma ve bölme gibi temel matematiksel işlemleri doğrudan konsol üzerinde yapabilir. Aşağıda bazı temel matematiksel işlemlerin örnekleri verilmiştir:

### **Toplama**
İki sayıyı toplamak için `+` operatörünü kullanabilirsiniz:

```r
10 + 7
```
Çıktı:
```r
[1] 17
```

### **Çıkarma**
Çıkarma işlemi için `-` operatörünü kullanabilirsiniz:

```r
15 - 3
```
Çıktı:
```r
[1] 12
```

### **Çarpma**
Çarpma işlemi için `*` operatörünü kullanabilirsiniz:

```r
6 * 4
```
Çıktı:
```r
[1] 24
```

### **Bölme**
Bölme işlemi için `/` operatörünü kullanabilirsiniz:

```r
20 / 4
```
Çıktı:
```r
[1] 5
```

### **Üs Alma**
R, üs alma işlemi için `^` operatörünü kullanır:

```r
2^3
```
Çıktı:
```r
[1] 8
```

## **Hata Mesajlarını Anlama ve Çözme**

R ile çalışırken bazen hatalarla karşılaşabilirsiniz. Hatalar, kodunuzda bir sorun olduğunu ve R’ın bunu çalıştıramadığını belirtir. Ancak endişelenmenize gerek yok, bu hatalar çoğunlukla küçük yazım veya kullanım hatalarından kaynaklanır.

### **Örnek Bir Hata:**
Aşağıdaki komutta `*` yerine `x` yazıldığı için bir hata oluşacaktır:

```r
3 x 5
```
Çıktı:
```r
Error: unexpected symbol in "3 x"
```

Bu hata, R’ın `x` sembolünü tanımadığını ve bu yüzden işlemi gerçekleştiremediğini belirtir. Bu hatayı düzeltmek için `x` sembolünü `*` ile değiştirebilirsiniz:

```r
3 * 5
```
Bu sefer doğru sonuç olan `15` çıktısını elde edeceksiniz.

### **Genel Hata Çözme İpuçları:**
1. **Sembolleri Doğru Kullanın:** R'da toplama için `+`, çarpma için `*`, bölme için `/` gibi semboller kullanılır. Yanlış bir sembol kullanırsanız hata alırsınız.
2. **Kodunuzda Yazım Hataları Olup Olmadığını Kontrol Edin:** R büyük/küçük harfe duyarlıdır, yani `A` ve `a` R için farklı şeyler ifade eder. Yazım hatalarına dikkat edin.
3. **Hata Mesajını Dikkatlice Okuyun:** R’ın verdiği hata mesajları, sorunun ne olduğunu anlamanıza yardımcı olabilir. Örneğin, yukarıdaki hata mesajı, "unexpected symbol" ifadesiyle bir sembol hatası olduğunu belirtmiştir.

---

Bu bölümde, R konsolunu kullanarak temel matematiksel işlemleri nasıl gerçekleştireceğinizi ve hata mesajlarını nasıl çözeceğinizi öğrendiniz. Artık R dilinde basit komutlar çalıştırmaya ve karşılaştığınız hataları çözmeye hazırsınız!
