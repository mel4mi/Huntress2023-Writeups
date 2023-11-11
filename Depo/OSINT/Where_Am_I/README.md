# Where am i
![Soru](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/OSINT/Where_Am_I/Where_Am_i.png)
## Soru İçeriği
[PXL_20230922_231845140_2](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/OSINT/Where_Am_I/PXL_20230922_231845140_2.jpg)

## Çözüm

Soruda fotoğraftan konum bulmamız isteniyor. Bu yüzden ilk yapacağımız iş "exiftool" ile fotoğrafın metadata'larına bakıyoruz.

![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/OSINT/Where_Am_I/Screenshot_1.png)

image description kısmında base64 ile şifrelenmiş bir yazı var. Yazıyı decode etmek için cyberchef'e atıyorum ve flag çıkıyor.

![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/OSINT/Where_Am_I/Screenshot_4.png)
