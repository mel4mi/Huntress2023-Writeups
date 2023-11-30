# Welcome to the Park
![Soru](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Miscellaneous/Welcome_To_The_Park/Welcome_To_The_Park.png)
## Soru İçeriği
[welcomeToThePark.zip](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Miscellaneous/Welcome_To_The_Park/welcomeToThePark.zip)

## Çözüm
![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Miscellaneous/Welcome_To_The_Park/Screenshot_1.png)

İndirilen dosyayı zip'ten çıkartıyorum. 

![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Miscellaneous/Welcome_To_The_Park/Screenshot_2.png)

Welcome dosyasının içine girip "ls -la " komutu çalıştırıyorum.

![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Miscellaneous/Welcome_To_The_Park/Screenshot_3.png)

".hidden" adlı klasör dikkat çekiyor. 

![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Miscellaneous/Welcome_To_The_Park/Screenshot_4.png)

Welcome adlı bir dosya olduğunu görüyoruz. "strings" komutu ile dosyasının içeriğini okuyoruz.

![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Miscellaneous/Welcome_To_The_Park/Screenshot_5.png)

Dosya içeriğinde base64 ile şifrelenmiş bir metin olduğunu görüyoruz. Metni çözmek için [Cyberchef](https://gchq.github.io/CyberChef/) sitesini ziyaret ediyoruz.
<!-- fotoğrafın obfuscate kısmı kalemle işaretlenecek -->
![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Miscellaneous/Welcome_To_The_Park/Screenshot_6.png)

Şifrelenmiş metni çözdüğümüzde obfuscate edilmiş bir payload görüyoruz. Bu payload'ı çözmek için link parçalarını birleştiriyorum. Ve bir github linki ortaya çıkıyor.

![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Miscellaneous/Welcome_To_The_Park/Screenshot_7.png)

Github linkini ziyaret ettiğimizde başka bir fotoğraf olduğunu görüyoruz ve fotoğrafı incelemek için bilgisayarıma indiriyorum.

![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Miscellaneous/Welcome_To_The_Park/Screenshot_8.png)

Fotoğrafa strings komutu ile içeriğini okuyorum ve flag ortaya çıkıyor.

![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Miscellaneous/Welcome_To_The_Park/Screenshot_9.png)
