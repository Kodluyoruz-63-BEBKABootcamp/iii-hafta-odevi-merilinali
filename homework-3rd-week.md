#### .Net kodu nedir ve nasıl derlenir?
.NET Framework, Microsoft tarafından geliştirilen, açık İnternet protokolleri ve standartları üzerine kurulmuş bir “uygulama” geliştirme platformudur. Sağladığı çoklu dil desteğiyle, tek dile bağlı kalmadan değişik tipte uygulamalar geliştirmemize olanak sağlar.

#### Roslyn compiler ne işe yarar?
Roslyn adı ile de bilinen .NET Derleyici Platformu (.NET Compiler Platform), Microsoft'tan C# ve Visual Basic .NET dilleri için bir dizi açık kaynak derleyici ve kod analizi API'sıdır. Özellikle C# ve VB.NET derleyicilerinin kendi kendini barındıran sürümlerini içerir - dillerin kendisinde yazılan derleyiciler.


#### Restful servisler nasıl çalışır? Alternatifleri nelerdir ve nasıl çalışırlar?
REST, client-server arasındaki haberleşmeyi sağlayan HTTP protokolü üzerinden çalışan bir mimaridir. REST ,servis yönelimli mimari üzerine oluşturulan yazılımlarda kullanılan bir transfer yöntemidir.İstemci ve sunucu arasında XML ve JSON verilerini taşıyarak uygulamanın haberleşmesini sağlar.REST mimarisini kullanan servislere ise RESTful servis denir.
##### Alternatifler:

- **GraphQL** belirli şema doğrultusunda verileri istemeyi açıklayan bir syntax'dır. Facebook tarafından geliştirilmektedir. GraphQL katmanlı veya birden fazla veri kaynağı ile istemvinin arasında yaşar, istemciden (client) gelen istekleri alır ve gereken verileri döner. Yani, üç ana özelliğe sahiptir:
İstemcinin (client) istediği verilerin belirtmesini sağlar
Birden fazla kaynağın veriye ulaşmasını kolaylaştırır
Bir tür sistem ile veriyi açıklar

- **Falcor** modeli Netflix tarafından geliştirilen bir JavaScript kütüphanesidir. Tüm uzak veri kaynaklarının sanal bir JSON graph aracılığı ile tek bir domian model aracılıyla temsil edilmesini sağlar. Veri toplamak için hala REST yapısını kullanır. Yani, bir request için farklı endpoint'lere istek gönderlir ve her resource için JSON object döndürür.

- Google Protobuf serialization altyapısını kullanan **gRPC**, programlar arası iletişimi sağlayan bir RPC(Remote Procedure Call) yöntemidir. Bu yöntem, uygulamalararası iletişim(IPC) ve uzak metod çağrımı(RPC) ve Web Servis gibi haberleşme yapılarının temeli olacak şekilde kullanılabilir.

- **OData**, url üzerinden veri kaynaklarını sorgulamak ve elde edilecek sonucu özelleştirmek için kullanılan REST ve HTTP tabanlı bir protokoldür. HTTP tabanlı olmasından dolayı tüm sorguları url üzerinden gerçekleştirmektedir. API’lar da elde edilecek verilerin özelleştirilmesi ve ihtiyaç doğrultusunda farklı formatlara büründürülebilmesi için normal durumda farklı endpointlerin geliştirilmesi ihtiyacını ortadan kaldırarak direkt olarak entityler üzerinde sorgulamayı üstlenmekte ve developerların sadece business logic ile ilgilenmesini sağlamaktadır. Böylece çok hızlı bir şekilde veri modellerine ait servisler oluşturulmasına imkan sağlamaktadır.




#### Extension method nedir? Nasıl yazılır?
Extension method, kelime anlamı ile genişletilebilir metod anlamına gelmektedir. Extension method bize .Net içerisinde bulunan sınıflara yeni metodlar eklememizi sağlamaktadır. Extension metodlar static class içerisinde static olarak tanımlanmaktadır.


#### MVC'nin alternatifleri nelerdir?
- HMVC - Hierarchical Model-View-Controller
- MVVM - Model-View-ViewModel
- MVP - Model View Presenter
- MVA - Model View Adapter
- PAC - Presentation Abstraction Control
- RMR - Resource-Method-Representation
- ADR - Action-Domain-Responder


#### Architectural pattern nedir? Neden ihtiyaç duyuyoruz?
Mimari desenler, yazılım mühendisliğindeki mimari sorunlara çözümler öneren yazılım desenleridir. Bir mimari desen, yazılım sistemi için alt sistemlerden ve bunların sorumluluklarıyla iç ilişkilerinden meydana gelen temel ve yapısal bir organizasyon şemasını ifade eder.

#### ViewData, ViewBag, TempData farkları nelerdir? Çalıştığımız proje üzerinde başka bir branch açarak bunları deneyiniz?
ViewBag, runtime esnasında oluşan dinamik bir yapıdır. ViewData, ViewDataDictionary sınıfı ile Key/Value ilişkisine göre çalışır. TempData, Controller da oluştutulan veriyi tek View içerisinde kullanabilmemizi ve View ler arasında taşımamızı sağlar. Taşıma işlemi diğer action a redirect edilmesi ile yapılır.
