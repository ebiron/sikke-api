.. raw:: html

   <p align="center">

.. raw:: html

   </p>

.. raw:: html

   <h1 align="center">

Sikke API v1.0 Dokümantasyonu

.. raw:: html

   </h1>

.. raw:: html

   <p align="justify">

Sikke API henüz V1.0 BETA aşamasında olup bazı endpointer için token
almanız gerekmektedir. Sikke API’yi kullanarak Sikke veritabanına
erişebilir ve kendi yazdığınız uygulamalar ile entegre edebilirsiniz.
Sikke API JSONAPI (http://jsonapi.org/) standartlarına uygunluğa dikkat
etmiştir.

Sikke.Network ağı MAINNET ve TESTNET sunucularından yayınlanır. Uygulama
geliştirme ve testler için TESTNET endpoint’ini, Productionlarınız için
MAINNET endpoint’ini kullanmalısınız. MAINNET ve TESTNET endpoint’leri
arasında versiyon farklılıkları olabilir! Lütfen sürüm versiyonlarını
kontrol etmeyi unutmayınız.

.. raw:: html

   </p>

Sikke.Network Endpointler
-------------------------

-  MAINNET BASE_URL : ``https://api.sikke.network/``
-  TESTNET BASE_URL : ``https://testnet.sikke.network/``
-  v1.0 ENDPOINT : ``https://*.sikke.network/v1``

Public Metodlar
---------------

Public Metodlar; erişim için Access Token gerektirmeyen ve herkesin
``GET`` ile sorgulamalar yapabileceği halka açık metodlardır.

-  `Wallet (Cüzdan)`_

   -  `Bakiye Sorgulama`_
   -  `Cüzdan Oluşturma`_

-  `Transaction (İşlemler)`_

   -  `İşlem Detayı`_
   -  `İşlem Listeleri`_

-  Node’ler (Madenciler)

   -  Node’ler
   -  Node Sorgulama

Private Metodlar
----------------

Private Metodlar; erişim için Access Token gerektiren ve gelişmiş
sorgulama ve işlemlerin yapılabileceği metodlardır.

-  `oAuth`_

   -  `Access Token Alma`_
   -  `Access Token Yenileme`_

-  `User (Kullanıcı)`_

   -  `Üye Olma`_
   -  `Giriş Yapma`_
   -  `Şifre Hatırlatma`_
   -  `Şifre Sıfırlama`_
   -  `Geçerli Kullanıcı`_

      -  `Kullanıcı Bilgileri`_
      -  `Bilgileri Güncelleme`_

-  `Wallet (Cüzdan) <Wallet-(Cüzdan)->`__

   -  `Bakiye Sorgulama <Wallet-(Cüzdan)-#bakiye-sorgulama>`__
   -  `Cüzdan Oluşturma <Wallet-(Cüzdan)-#cüzdan-oluşturma>`__
   -  `Cüzdan Bilgileri`_
   -  `İşlem Geçmişi`_

-  İşlemler

   -  Ödeme Gönderme
   -  İşlem Bilgileri

-  Node’ler (Madenciler)

   -  Node’ler
   -  Node Sorgulama

.. _Wallet (Cüzdan): Wallet-(Cüzdan)
.. _Bakiye Sorgulama: Wallet-(Cüzdan)#bakiye-sorgulama
.. _Cüzdan Oluşturma: Wallet-(Cüzdan)#cüzdan-oluşturma
.. _Transaction (İşlemler): Transaction-(İşlemler)
.. _İşlem Detayı: Transaction-(İşlemler)#İşlem-detayı
.. _İşlem Listeleri: Transaction-(İşlemler)#İşlem-listeleri
.. _oAuth: oAuth
.. _Access Token Alma: oAuth#access-token-alma
.. _Access Token Yenileme: oAuth#access-token-yenileme
.. _User (Kullanıcı): User-(Kullanıcı)
.. _Üye Olma: User-(Kullanıcı)#Üye-olma
.. _Giriş Yapma: User-(Kullanıcı)#giriş-yapma
.. _Şifre Hatırlatma: User-(Kullanıcı)#Şifre-hatırlatma
.. _Şifre Sıfırlama: User-(Kullanıcı)#Şifre-sıfırlama
.. _Geçerli Kullanıcı: User-(Kullanıcı)#geçerli-kullanıcı
.. _Kullanıcı Bilgileri: User-(Kullanıcı)#kullanıcı-bilgileri
.. _Bilgileri Güncelleme: User-(Kullanıcı)#bilgileri-güncelleme
.. _Cüzdan Bilgileri: Wallet-(Cüzdan)-#cüzdan-bilgileri
.. _İşlem Geçmişi: Wallet-(Cüzdan)-#İşlem-geçmişi
