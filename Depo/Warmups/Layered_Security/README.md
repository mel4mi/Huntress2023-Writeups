# Layered Security
![Soru](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Warmups/Layered_Security/layeredsecurity.png)
## Soru İçeriği
Sizde indirip deneyebilirsiniz.
[Layered_Security](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Warmups/Layered_Security/layered_security)

## Çözüm
Dosyayı ilk indirdiğimizde herhangi bir uzantıya sahip olmadığı için dosyanın ne olduğunu anlamakta zorluk çekebiliriz. Bu sorunu çözmek için "file" komutu ile dosyanın ne olduğunu öğrenmeye çalışabiliriz.

![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Warmups/Layered_Security/Screenshot_1.png)
Dosyanın gimp tarafından oluşturulmuş bir fotoğraf olduğunu söylüyor. Gimp'i açıklamak gerekirse, gimp linux ortamında çalışan fotoğraf düzenleme uygulamasıdır. şimdi ise verilen dosyayı gimp ile açıp ne olduğuna bakıyoruz.

![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Warmups/Layered_Security/Screenshot_2.png)

Yukarıdaki fotoğrafa dikkatli baktığımızda fotoğraf birbiri üstüne yerleştirilmiş bir sürü katmana sahip olduğunu görüyoruz(sağ alt kısma bakınız). Katmanları teker teker kaldırdığımda ise flagı buluyoruz.

![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Warmups/Layered_Security/Screenshot_3.png)
