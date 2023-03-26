# Uygulamalı JavaScript Sprint Mücadelesi

**Bu talimatları dikkatlice okuyun. Bu Sprint Mücadelesine başlamadan önce tam olarak ne beklendiğini anlayın.**

Bu mücadele, geçmiş sprint boyunca öğrenilen kavramları ve teknikleri uygulamanıza ve bunları somut bir projede kullanmanıza olanak tanır. Bu sprint sayesinde **Uygulamalı JavaScript** 'i keşfettiniz. Bu sprint boyunca **DOM ve bileşenler**'i öğrendiniz. Bu mücadelede, **çevrimiçi bir Teknoloji Gazetesi** oluşturarak bu becerilerdeki ustalığınızı göstereceksiniz.

Bu projeyi, herkesin kendisinin yapması beklenmektedir. Tüm iş size ait olmalıdır. Mücadele puanınız, bu sprint boyunca işlenen materyali kullanarak bağımsız çalışma yeteneğinizin bir ölçüsüdür. Önceki Sprint'te tanıtılan ve uygulanan kavram ve hedeflerde yeterlilik göstermeniz gerekir.

Bu sprint mücadelesi sırasında işbirliği yapmanıza izin verilmez.

### Proje Kurulumu

- [ ] Bu projenyi forklayarak bir kopyasını oluşturun.
- [ ] Reponun kendi versiyonunuzu klonlayın.
- [ ] Commitinizi pushlayın: `git push origin main`.

## Proje Açıklaması

### Giriş

Bir teknoloji gazetesi oluşturacaksınız. İşiniz, gazetenin ana sayfasını oluşturan bileşenleri oluşturmak olacak..

Aşağıda listelenen minimum uygulanabilir ürün (MVP) spesifikasyonlarını karşılayan projeniz, aşağıda bağlantısı verilen görüntüye benzer görünmelidir.:

[Teknoloji Zamanı](/tasarım.png)

### Detaylar

- [ ] Komut satırınızla projenin kök dizinine gidin.
- [ ] `package.json` dosyasında listelenen bağımlılıkları indirmek için `npm install` komutunu çalıştırın.
- [ ] Projeyi derlemek ve sunmak için `npm start` komutunu çalıştırın.
- [ ] Chrome'da `http://localhost:3000` konumuna gidin
- [ ] Testleri çalıştırmak için ayrı bir terminalde `npm test` komutunu yazın.

**MVP için adımlar:**

- [ ] Adım 1 ve 2 `src/bileşenler/header.js` dosyasında açıklandı.
- [ ] Adım 3 ve 4 `src/bileşenler/tabs.js` dosyasında açıklandı.
- [ ] Adım 5 ve 6 `src/bileşenler/card.js` dosyasında açıklandı.

**Önemli Notlar:**

- Lütfen **dosyaları ya da klasörleri taşımayın ve isimlerini değiştirmeyin** .
- Geliştirme sunucunuz "otomatik yeniden yüklemeyi" durdurursa, `CTRL+C` ile manuel olarak sonlandırın ve yeniden başlatın.
- `package.json` 'ı değiştirmeyin, sadece NPM ile dosyaları indirin (Axios _halihazırda_ `package.json` 'a eklendi).
- Çözümünüzde en iyi uygulamaları izlemeniz, temiz ve profesyonel sonuçlar üretmeniz önemlidir.
- Yazım denetimi ve dilbilgisi denetimi de dahil olmak üzere çalışmanızı gözden geçirmek, iyileştirmek için zaman planlayın.
- MVP'yi karşılayan bir meydan okuma göndermek, çok fazla detayla uğraşılıp da çalışmayan bir kod göndermekten daha iyidir.

## Ek Sorular

Aşağıdaki soruları yanıtlayarak bu sprint'in kavramlarını anladığınızı gösterin. Her sorudan sonra yanıtlarınızı eklemek için bu belgeyi düzenleyin.

1. DOM nedir?

DOM, belgenin içeriğini belirli bir düzen içerisinde nesne olarak temsil edilmesini sağlayan bir modeldir. Bu modelde belge yapısında bulunan her bir nesne için bir düğüm bulunur. Alt düğümler kök bir düğüme bağlanır. Belge ile iletişim kuran servis düğümü çözerek işlemlerini gerçekleştirir. DOM yapısı nesnelerden oluşan bir yapıdır. Bir çeşit alt-üst ilişkisi bulunan soyağacı gibidir. Ana nesne altında birbirinden farklı alt nesneler, alt nesnelerin altında da hiyerarşik yapıda nesnelerden oluşur.

2. Bir event nedir?

JavaScript'te event, bir web sayfasında gerçekleşen herhangi bir etkileşim veya olaydır. Bu olaylar, kullanıcının sayfada yaptığı herhangi bir işlem veya sayfanın içeriği ile ilgili değişikliklerle tetiklenebilir. Örneğin, bir kullanıcının bir düğmeye tıklaması bir olaydır. Bir form gönderildiğinde veya sayfadaki bir metin kutusuna yazı yazıldığında da olay tetiklenebilir. Başka bir örnek olarak, sayfa yüklendiğinde veya tarayıcı boyutu değiştiğinde de olaylar tetiklenebilir. JavaScript, olayları dinleyebilir ve bu olayların gerçekleştiğinde belirli kodları çalıştırabilir. Bu şekilde, bir web sayfasındaki etkileşimleri yakalayabilir ve sayfanın davranışını değiştirebilirsiniz. Bu işlevsellik, dinamik web sayfaları oluşturmak için önemlidir.

3. Bir event dinleyici(listener) nedir?

JavaScript'te bir event dinleyici (listener), bir web sayfasındaki belirli bir olayı dinlemek ve bu olayın gerçekleştiğinde belirli bir kod bloğunu tetiklemek için kullanılan bir fonksiyondur. Event dinleyicileri, HTML DOM (Document Object Model) öğeleri veya belge nesnesindeki olaylara bağlanarak, belirli bir olayın gerçekleştiğinde tetiklenen bir işlevi çalıştırırlar. Bu olaylar, kullanıcının bir düğmeye tıklaması, bir form göndermesi veya sayfadaki bir metin kutusuna yazı yazması gibi herhangi bir kullanıcı etkileşimi olabilir.

4. Neden bir NodeList'i Array'e dönüştürelim??

JavaScript'te NodeList, belge nesnesindeki bir öğeler koleksiyonunu temsil eder ve tipik olarak querySelectorAll() gibi yöntemlerle seçilir. NodeList, bir diziye benzer bir yapıya sahiptir, ancak dizi yöntemlerine sahip değildir. Bunun anlamı, bir NodeList üzerinde forEach() gibi bir dizi yöntemi kullanılamayacağıdır. Bir NodeList'i bir diziye dönüştürmek, NodeList üzerinde dizi yöntemlerinin kullanılmasını sağlar. Bu, NodeList üzerinde daha fazla işlem yapmanıza ve daha özelleştirilmiş bir işlevsellik oluşturmanıza olanak tanır.

5. Bileşen nedir?

Component(Bileşen), yazılım geliştirmede tekrar kullanılabilir kod bloklarını ifade eder. Component, bir web uygulaması veya mobil uygulama gibi bir yazılım projesinde kullanılabilecek, kendine özgü işlevselliğe sahip ve bağımsız bir parçadır. Web uygulamalarında, bir component genellikle bir HTML öğesi, CSS stilleri ve JavaScript kodu içeren bir pakettir. Component'ler, genellikle web sayfalarında veya uygulamalarda birden fazla kez kullanılabilir. Böylece, bir component'i tek bir yerde oluşturup birden fazla sayfada veya uygulamada kullanarak, kod tekrarını azaltmak ve kod tabanını daha organize hale getirmek mümkündür. Component tabanlı yazılım geliştirme, genellikle daha modüler, esnek ve bakımı daha kolay olan kodlar oluşturur. Bir component'in farklı parçaları bağımsız olabileceğinden, geliştirme sürecinde bir bölüm değiştirildiğinde diğer bölümlere etkisi daha az olacaktır. Örneğin, bir web uygulamasında, bir navigation component'ı, site genelinde kullanılan gezinme menüsü veya butonları içerebilir. Böylece, bu component, site genelinde birden fazla yerde kullanılabilir ve her sayfada tekrar tekrar oluşturulması gerekmez. Aynı zamanda, gezinme menüsünün stilini veya işlevselliğini değiştirmek istediğinizde, yalnızca navigation component'ında yapmanız yeterlidir ve tüm uygulamada bu değişiklik yansıtılacaktır.
