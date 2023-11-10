# Book by its cover
![Soru](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Warmups/Book_By_Its_Cover/Book_By_Its_Cover.png)
## Soru İçeriği
![Soru İçeriği](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Warmups/Book_By_Its_Cover/soru_icerigi.png)

## Çözüm
verilen dosyayı açmaya çalıştığımız zaman bize arşiv bozuk hatası veriyor. Dosyayı kontrol etmek için ilk başta magic bytlerını kontrol etmek istedim. 

![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Warmups/Book_By_Its_Cover/Screenshot_3.png)
"File" komutu ile dosyayı kontrol ettiğimde dosyanın .rar ile kayıt edilmesine rağmen magic byte'ları png olduğunu söylüyor. Bende "book.rar" olan dosyasını "book.png" olarak değiştirdim.

![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Warmups/Book_By_Its_Cover/Screenshot_2.png)


## Magic Byte nedir
Magic byte bir dosyanın ilk satırında bulunan ayrılmış bir byte dizisini ifade eder. bu byte'lar sayesinde dosyanın türünü tanımlayabiliriz. Yani bir nevi imza görevi görür. örneklendirmek gerekirse "FF D8" byte'ları jpeg(resim) dosyalarını tanımlamak için kullanılır. eğer bir jpeg dosyasının ilk baytları "FF D8" değilse o dosya açılmayabilir ve bozuk çalışabilir. Dosyanın sağlıklı işlenebilmesi için ise bu byte'ları düzeltmemiz gerekir.

