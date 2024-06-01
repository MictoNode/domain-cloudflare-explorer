İlk önce Domaininizi alın. Websitesi oluşturma fikriniz varsa domain ve host'unuzu ayrı ayrı almanızı öneririm. Domain'i de bilindik yerden almanızı da ayrıca tavsiye ederim. Websitesine gerek yok diyorsanız Domain yeterli.
Benim örnek vereceğim firmaları söyleyim; **Domain firması - spaceship** **Hosting firması - Odeaweb**

**1)** İlk yapmamız gereken bir cloudflare hesabı oluşturmak. Daha sonrada anasayfadan direkt "Get started" a tıklıyoruz. Aldığımız domaini giriyoruz. Bedavayı seçiyoruz. Biraz bekletecek domain'in dnslerini vs. çekecek.

![1](https://i.hizliresim.com/bf9rvqq.png)

**Alttaki görselde kendi satın aldığınız domain adını yazın. GÖrseldeki örnek farazi. Mesela ben aslında oraya mictonode.com yazdım**

![2](https://i.hizliresim.com/c1vzad1.png)

![3](https://i.hizliresim.com/gj4dzyd.png)

![4](https://i.hizliresim.com/1jv796u.png)


**2)** Burada odaklanmanız gereken şuanlık en alttaki "nameservers" kısmı. Merak edersiniz de görselde biraz açıkladım. Nameservers kısmında yazanların ikisini de kopyalayın kenarda dursun lazım olacak.

![5](https://i.hizliresim.com/chjxkw1.png)

**3)** Şimdi domain aldığımız yere dönüyoruz. Kendi domaini firmanızın illa nameserver değiştirme yeri vardır. Spaceship'e kayıt olup aldıktan sonra sağ üstte "Launchpad" tıklayınca karşınıza bir panel gelecek. Oradan Domain List'e tıklıyoruz. Domain'in Nameserverlarını Cloudflare Nameserverlarla değiştiriyoruz. Görselde açıkladım zaten.

![6](https://i.hizliresim.com/i1rtwiu.png)

![8](https://i.hizliresim.com/op7ario.png)

![9](https://i.hizliresim.com/lh2wmrs.png)

**4)** Son görseldeki adımdan sonra domain nameserverlarının işleve geçmesi maksimum 24 saat sürüyor. Bazen direkt işleme geçiyor. Spaceship'te yaklaşık 6 saat falan sürdü. Önemli değil biz domaini taşıdık. Artık her şeyi Cloudflare üzerinden yapcaz. Şimdi siz [Coinsspor reposundaki](https://github.com/coinsspor/crossfi/blob/main/Crossfi%20Rpc%20ve%20Api%20Kurulumu.md) RPC ve API kurulumunu yapın ama CertBot kısmını bekletin. 2.bölümde size hatırlatacağım. CertBot kısmına o zaman dönersiniz. Bu 1.bölümdü. Bitti...

*2. Bölüm için Coinsspor'un anlattığı gibi API ve RPC'nizi kurduktan sonra hazırda sunucu ip'niz olsun. Cloudflare'dan subdomain oluşturup (aslında tam subdomain değil ama çalışıyor sorun yok) sunucumuza bağlayacağız. Aslında Coinsspor hocam da açıklamış ama gerekli tüm ayarların üstünden geçeceğiz.*

**Not:** *RPC ve API kurulumdaki "Yapılandırma Dosyanızı Oluşturma" bölümlerinde oraya yazdığınız "projeadı-testnet-api/rpc.domainadresiniz.com" kısmını da kenara kaydedin ve kurulumda istediğiniz subdomaini oraya yazın. Cloudflare'a "projeadı-testnet-api/rpc" kısmını yazacağız.*
