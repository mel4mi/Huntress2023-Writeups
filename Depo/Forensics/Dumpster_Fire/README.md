# Dumpster Fire
![Soru](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Forensics/Dumpster_Fire/Dumpster_Fire.png)
## Soru İçeriği
[dumpster_fire.tar.xz](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Forensics/Dumpster_Fire/dumpster_fire.tar.xz)

## Çözüm
İlk başta verilen dosyaları verilen tar'dan çıkartıyoruz.

![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Forensics/Dumpster_Fire/Screenshot_4.png)

Dosyaları incelediğimde linux kök diziniyle aynı olduğunu farkediyorum ve araştırma yapmaya başlıyorum. İlk merak ettiğim kısım sisteme ait user'ların dosyaları olduğundan hemen home dizinine giriyorum.

![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Forensics/Dumpster_Fire/Screenshot_5.png)

Challange user'ına ait dosyalarına baktığım zaman ".mozilla" dosyası buluyorum. Bu dosya, cihazda çalışan Mozilla Firefox tarayıcısının önbellek dosyalarını bulunduruyor. Bu dosyalarının bana kalırsa en önemli özelliği, tarayıcıda kayıt edilmiş şifrelere erişebilmemiz.
Bunun için öncellikle [firefox_decrypt](https://github.com/unode/firefox_decrypt) toolunu indirip kuruyorum.

Sonrasında indirdiğim toola .mozilla klasörünün yolunu belirterek programı çalıştırıyorum.
```
python3 firefox_decrypt.py ~/path/to/.mozilla/file/...
```
![](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Forensics/Dumpster_Fire/Screenshot_6.png)

İşte flag.
