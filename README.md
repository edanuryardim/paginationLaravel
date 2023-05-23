# paginationLaravel
paginationLaravel


Bu kod, bir sayfalama (pagination) sistemi oluşturmak için kullanılan bir HTML şablonunu temsil etmektedir. Aşağıda, kodun nasıl çalıştığına dair bir açıklama bulunmaktadır:

1. `$articles` değişkeni, sayfalama yapılacak makalelerin verilerini içeren bir koleksiyonu temsil etmektedir. Bu kodun tamamı bir sayfa şablonunda kullanılmak üzere tasarlanmıştır.

2. `if` koşulu, mevcut sayfanın 1'den büyük olduğunu kontrol eder. Eğer doğru ise, bir önceki sayfaya geçmek için bir düğme oluşturulur. Bu düğme, `$articles->previousPageUrl()` fonksiyonuyla bir önceki sayfanın URL'sini alır.

3. `for` döngüsü, sayfa numaralarını oluşturmak için kullanılır. Döngü, mevcut sayfanın 2 birim öncesinden başlayarak mevcut sayfanın 2 birim sonrasına kadar ilerler. Bu şekilde, mevcut sayfa ortada olacak şekilde maksimum 5 sayfa numarası gösterilir. Her sayfa numarası, `$articles->url($i)` fonksiyonuyla ilgili sayfanın URL'sine yönlendiren bir bağlantı oluşturur.

4. `if` koşulu, mevcut sayfanın son sayfadan küçük olduğunu kontrol eder. Eğer doğru ise, bir sonraki sayfaya geçmek için bir düğme oluşturulur. Bu düğme, `$articles->nextPageUrl()` fonksiyonuyla bir sonraki sayfanın URL'sini alır.

Bu kod, verilen makale koleksiyonunu sayfalar halinde görüntülemek için kullanılır. Her sayfada bir önceki sayfa, sayfa numaraları ve bir sonraki sayfa için bağlantılar bulunur. Bu sayede kullanıcılar, sayfalar arasında gezinebilir ve makaleleri görüntüleyebilirler.
