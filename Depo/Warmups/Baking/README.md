
# Baking
![Soru](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Warmups/Baking/baking.png)
## Soru İçeriği
Online soru

## Çözüm
Soruda verilen siteye girdiğimiz zaman bir kaç tane tarif ve bir adet fırın olduğunu görüyoruz.

![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Warmups/Baking/Screenshot_1.png)

Bir tarifi pişirmek için cook a bastığımız zaman tarifin tamamlanması için gereken süreyi bize gösteriyor.

![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Warmups/Baking/Screenshot_2.png)

Fakat bu bilgiler soruyu çözmek için değil. BurpSuite ile sitede gelen giden paketleri inceleyerek sitenin nasıl çalıştığını anlamaya çalışıyorum.

![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Warmups/Baking/Screenshot_3.png)

Yukarıdaki paketlere baktığımız zaman cookie'lerde base64 ile encode edilmiş bir değer olduğunu görüyoruz. Cookie'nin içerisinde olduğunu öğrenmek için cyberchef de decode ediyorum.

![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Warmups/Baking/Screenshot_4.png)

Cookie'e baktığımız zaman json datası halinde seçtiğimiz tarif ve başlangıç vaktinin bulunduğunu görüyoruz. İstediğimiz tarifin pişmesi için 5 gün süre geçmesi gerektiği için cookie değerindeki tarihi 5 gün öncesine alıp encode edip tekrar siteye giriyorum.

![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Warmups/Baking/Screenshot_6.png)

işte flag

![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Warmups/Baking/Screenshot_5.png)
