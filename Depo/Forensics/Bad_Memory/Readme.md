# Bad Memory(Forensic)
![Soru](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Forensics/Bad_Memory/Bad_Memory.png)
## Soru İçeriği
[eklenecek]()

## Çözüm
İmage isimli bir dosya verilmiş ve bizden kullanıcının şifresini bulmamızı istiyor. Dosyayı indirip arşivden çıkardığımda boyutunun 4gb civarında olduğunu gördüm ve memory dump olduğu düşündüm. Volatility sayesinde Memory dump dosyalarını analiz edebiliyoruz. Kullanıcının şifresini sorduğu için hivelist modulü ile tüm kullanıcı listesini çıkarttım. <br>
```vol.py -f image.bin windows.registry.hivelist```

![Soru](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Forensics/Bad_Memory/BadMemoryHive.PNG)

Kullanıcı listesinde "congo" adında bir local kullanıcı gözüküyor. Hashdump modulü ile kullanıcıların hash değerlerini çıkarttım. <br>
``` vol.py -f image.bin windows.hashdump > cikti.txt ```

![Soru](https://github.com/mel4mi/Huntress2023-Writeups/blob/main/Depo/Forensics/Bad_Memory/BadMemoryHash.PNG)

Çıkarttığım hash değerlerinden "congo" kullanıcısının hash değerini CrackStation sitesi üzerinde kırarak şifreyi elde ediyorum. <br>
```şifre = goldfish#```

En son olarak şifreyi md5 ile şifreleyip flag değerini girdim. <br>
```flag{2eb53da441962150ae7d3840444dfdde}```
