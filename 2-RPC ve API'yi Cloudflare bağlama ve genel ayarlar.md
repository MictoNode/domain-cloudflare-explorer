  Evet şuan RPC ve API'nizi kurdunuz. İstediğiniz subdomain'i de oraya yazdığınız ve onların notlarını aldınız. Sunucu ipniz de kenarda. O zaman hazırız.

  **1)** Cloudflare anasayfasında website kısmına girip sitemizi seçiyoruz. Soldaki DNS/Records kısmına geliyoruz. (Tam görünüm şeklinde DNS ayarları 1.Bölümde var bi göz atabilirsiniz tekrar)
    
  **2)** "Add record" kısmına tıklıyoruz. Type kısmından A'yı seçiyoruz. "Name (required)" kısmına Yapılandırma Dosyasına yazdığımız adresin ilk kısmını yazıyoruz. Örnek: RPC Yapılandırma Dosyasında Server_name kısmına yazdığınız **corenode-testnet-rpc.mictonode.com** diyelim. Oradaki "corenode-testnet-rpc" kısmını yazıyoruz. IPv4 address (required) kısmına sunucu ipmizi yazıyoruz.
  Bu adımı hem rpc hem api için yaptınız artık tamamız. Peki başka ne ayarları yapmamız gerekiyor derseniz devam edelim. Çok güzel ayarlar var.

![image](https://github.com/user-attachments/assets/dac04345-6c98-4c15-848c-7293b4d13235)

  **3)** Yine Cloudflare'dan website kısmına girelim ve websitemize girelim. Soldaki SSL/TLS'ne tıklayın Overwiev kısmında SSL/TLS Recommender açık. Eğer hostunuzda ssl hizmeti varsa veya daha önce yaptıysanız üstteyi ayarı benim gibi Full strict yapabilirsiniz. Ben de google amca sayesinde öğrendim yaşadığım sorunu hatırlamıyorum. İsterseniz o ayara dokunmayabilirsiniz. Daha sonra bir alt menüdeki edge certificates kısmına gelelim ve Always Use HTTPS'yi açalım.

![image](https://github.com/user-attachments/assets/9c566acc-1f34-4c95-93dc-a8b185e586b8)

![image](https://github.com/user-attachments/assets/e35b1dcc-aac0-46d2-bfb3-18e568cf620d)

  **4)** Lazım olur diye Bypass Cache ayarını da yapalım. Caching > Cache Rules > Create rule. 2. Görseldeki gibi ayarlar sadece domain değişmesi önemli. mictonode.com / explorer.mictonode.com gibi gibi..

![image](https://github.com/user-attachments/assets/1806ee3a-e6d7-4420-bdab-79f9db5d1f1e)

![image](https://github.com/user-attachments/assets/df383b83-50e3-442f-bf44-f01d5c5243d7)

  **5)** Daha fazla bizlik bir ayar yok. İngilizce makalelere göz atarak ekstra ayarları öğrenebilirsiniz ama bunlar iş görecektir. Ben yine explorer kısmında Cloudflare kısmına domain bağlamak için bahsedeceğim. Cloudflare ile aramızı iyi tutalım. Bu arada CertBot kısmını şuan yapanilirsiniz ama sanırım cloudflare'sa ssl sertifikası atıyor otomatik.
