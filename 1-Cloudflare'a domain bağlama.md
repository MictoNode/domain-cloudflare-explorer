İlk önce Domaininizi alın. Websitesi oluşturma fikriniz varsa domain ve host'unuzu ayrı ayrı almanızı öneririm. Domain'i de bilindik yerden almanızı da ayrıca tavsiye ederim. Websitesine gerek yok diyorsanız Domain yeterli.
Benim örnek vereceğim firmaları söyleyim; **Domain firması - spaceship** **Hosting firması - Odeaweb**

**1)** İlk yapmamız gereken bir cloudflare hesabı oluşturmak. Daha sonrada anasayfadan direkt "Get started" a tıklıyoruz. Aldığımız domaini giriyoruz. Bedavayı seçiyoruz. Biraz bekletecek domain'in dnslerini vs. çekecek.

![image](https://github.com/user-attachments/assets/bf2bb996-9db2-4c5a-827d-ca8bf0aba671)


**Alttaki görselde kendi satın aldığınız domain adını yazın. Görseldeki örnek farazi. Mesela ben aslında oraya mictonode.com yazdım**

![image](https://github.com/user-attachments/assets/e90f4289-22ed-4b3e-97d9-c18ed86a7ab9)

![image](https://github.com/user-attachments/assets/6288d275-dbf3-42c6-8076-85ea1e8e3093)

![image](https://github.com/user-attachments/assets/02c79f3f-dbef-41d7-bd20-4be130ed66fe)

**2)** Burada odaklanmanız gereken şuanlık en alttaki "nameservers" kısmı. Merak edersiniz de görselde biraz açıkladım. Nameservers kısmında yazanların ikisini de kopyalayın kenarda dursun lazım olacak.

![image](https://github.com/user-attachments/assets/b8a3a6e5-1b6b-499d-a4b3-8e4d7be96102)

**3)** Şimdi domain aldığımız yere dönüyoruz. Kendi domaini firmanızın illa nameserver değiştirme yeri vardır. Spaceship'e kayıt olup aldıktan sonra sağ üstte "Launchpad" tıklayınca karşınıza bir panel gelecek. Oradan Domain List'e tıklıyoruz. Domain'in Nameserverlarını Cloudflare Nameserverlarla değiştiriyoruz. Görselde açıkladım zaten.

![image](https://github.com/user-attachments/assets/2f8aa75f-1a04-4995-84ad-904d9a71529b)

![image](https://github.com/user-attachments/assets/c3a3656e-6572-48d5-923f-62ea3b46cb90)

![image](https://github.com/user-attachments/assets/46ac6959-e33f-4e15-926c-7a61d75179b1)

**4)** Son görseldeki adımdan sonra domain nameserverlarının işleve geçmesi maksimum 24 saat sürüyor. Bazen direkt işleme geçiyor. Spaceship'te yaklaşık 6 saat falan sürdü. Önemli değil biz domaini taşıdık. Artık her şeyi Cloudflare üzerinden yapcaz. Şimdi siz [Coinsspor reposundaki](https://github.com/coinsspor/crossfi/blob/main/Crossfi%20Rpc%20ve%20Api%20Kurulumu.md) RPC ve API kurulumunu yapın ama CertBot kısmını bekletin. 2.bölümde size hatırlatacağım. CertBot kısmına o zaman dönersiniz. Bu 1.bölümdü. Bitti...

*2. Bölüm için Coinsspor'un anlattığı gibi API ve RPC'nizi kurduktan sonra hazırda sunucu ip'niz olsun. Cloudflare'dan subdomain oluşturup (aslında tam subdomain değil ama çalışıyor sorun yok) sunucumuza bağlayacağız. Aslında Coinsspor hocam da açıklamış ama gerekli tüm ayarların üstünden geçeceğiz.*

**Not:** *RPC ve API kurulumdaki "Yapılandırma Dosyanızı Oluşturma" bölümlerinde oraya yazdığınız "projeadı-testnet-api/rpc.domainadresiniz.com" kısmını da kenara kaydedin ve kurulumda istediğiniz subdomaini oraya yazın. Cloudflare'a "projeadı-testnet-api/rpc" kısmını yazacağız.*
