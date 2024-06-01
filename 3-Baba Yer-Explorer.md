Şimdi ilk olarak üstünden anlatacağım ama kilit noktalara da değineceğim. Yapamadıklarınızı sorun tabi ama işlevsel çalıştıktan sonrası explorer'daki özelleştirmeler sizin yaratıcılığınıza aittir bilginiz olsun.

**1)** Dolandırmadan başlıyorum ilk önce explorer dosyalarını forklaycağız. Bunu isterseniz Ping-pub'dan direkt forklayın istersen itrocket'dan farketmez. Ben Itrocket'dan forkladım çünkü chain dosyaları neredeyse tam. Editlemesi kolay.

  ![1](https://i.hizliresim.com/l3al0c1.jpg)

**2)** İsterseniz indirip atın github'ınıza isterseniz forklayın. Sonuçta artık github'ınızda şimdi Vercel'e üye olmalısınız. Üyelik işlemlerinde sonra overview ekranından proje oluşturun. Daha sonra solda çıkan explorer'ı bağlayın. Daha sonra bi isim belirleyip deploy diyin.

  ![2](https://i.hizliresim.com/9sbl3nz.jpg)

  ![3](https://i.hizliresim.com/bccjy8o.jpg)

  ![4](https://i.hizliresim.com/mubie9w.jpg)

  ![5](https://i.hizliresim.com/9qtra74.jpg)

**3)** Şimdi direkt biz oyalanmadan "Add Domain" e tıklayalım. Açılan sayfada siteni yazıp Add'e bas. explorer.siteadınız.com gibi yazın çünkü Cloudflare'da bunu kullanacağız.

  ![6](https://i.hizliresim.com/dd8bddl.jpg)

  ![7](https://i.hizliresim.com/klont28.jpg)

**4)** Şimdi bu aşamayı art arda görsellerle anlatacağım. Görerek daha kolay :D CNAME olarak vercelin verdiği dns'i gireceğiz. Tam olarak da göründüğü gibi olacak. Görseller arasında domain farkı olabilir ben kendi domainimden test için bir subdomain oluşturacağım. CNAME eklemek için yeni sekme açıp CLoudflare'a giriyoruz ve DNS sekmesindeyiz.

  ![8](https://i.hizliresim.com/5zry8ng.jpg)

  ![9](https://i.hizliresim.com/gvb52v1.jpg)

  **Burada kontrol ediyoruz name'e sadece deneme yazdık diye olmadı zannetmeyin. Eklediğiniz domain'i kendisi otomatik ekliyor. Mouse'u üzerine getirdiğinde görüyorsun.**

  ![10](https://i.hizliresim.com/o6zfuth.jpg)

  **Kendi kendine otomatik onaylandı.**

  ![11](https://i.hizliresim.com/jd5hbm0.jpg)

 **Girip bakalım olmuş mu?**

  ![12](https://i.hizliresim.com/t580nlr.jpg)

**5)** Geri kalan explorer özelleştirme sizde. /airchains gibi sayfalarda f5 atınca 404 hatası veriyor. Onun çözümü de tek satır kod. Vercel.json diye bir klasör oluşturun içine aşağıda attığım kodu atın ve kaydedin. Dizinle birlikte görselleri atıyorum. 
Not: Github'a attığınız her şeyi vercel otomatik deploy edecektir.

```
{
    "rewrites": [{ "source": "/(.*)", "destination": "/" }]
}
```


  ![1](https://i.hizliresim.com/gubigl0.jpg)
