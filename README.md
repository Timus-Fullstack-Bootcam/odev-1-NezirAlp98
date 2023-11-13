**1. JavaScript nedir ve tarihsel gelişiminden bahsedin:**
JavaScript, 1995 yılında bir Netscape çalışanı olan Brandan Eich tarafından geliştirilmiştir. İlk ortaya çıktığı dönemde söz konusu yazılımın adı Mocha idi. Sonradan Mona adını alan yazılım, zaman içerisinde LiveScript ve en son da JavaScript adı ile anılmıştır. Yazılım ilk geliştirildiği dönemde çok sınırlı bir işleve sahipti. Fakat zaman içerisinde web dünyasında yaşanan gelişmeler de dikkate alınarak günümüzdeki halini almıştır. 

JavaScript, ortaya çıktığı günden bugüne inanılmaz bir hızla gelişimini sürdürmüştür. 2016 yılına gelindiğinde ise web sitelerinin yaklaşık %92’lik kısmı bu yazılımı kullanmaya başlamıştır. Sadece 20 yıl gibi kısa bir sürede büyük bir başarıya imza atan JavaScript, büyük bir yazılım dili olmayı başarmıştır


**2. Java ile javascript arasındaki fark nedir?**
- Java bir OOP programlama dilidir, Java Script bir OOP komut listesi oluşturma dilidir.
- Java, sanal makinede veya tarayıcıda çalışan uygulamalar oluşturur, JavaScript kodu sadece tarayıcıda çalıştırılır.
- Java kodunun derlenmesi gerekir, JavaScript kodları metinlerden oluşur.
- Farklı eklentiler gerektirirler.

**3. Javascript teki veri tipleri nelerdir açıklayınız:**
1. **String(Metin):** Metin verilerini temsil eder.

    ```javascript
    let metin = "Merhaba, Dünya!";
    console.log(metin);
    ```
2. **Number(Sayı):** Tamsayılar veya ondalık sayılar gibi sayısal değerleri temsil eder.

    ```javascript
    let sayi = 42;
    let sayi2= 3.14
    console.log(sayi,sayi2);
    ```
3. **Boolean (Mantıksal Değer):**
"true" veya "false" gibi iki değeri temsil eder.

    ```javascript
    let dogruMu = true;
    console.log(dogruMu);
    ```
4. **Array(Dizi):** Bir dizi içinde birden çok değeri sıralar.

    ```javascript
    let dizi = [1, 2, 3, 4];
    console.log(dizi);
    ```
5. **Object (Nesne):** İsimlendirilmiş özelliklerle ilişkilendirilmiş bir dizi değeri temsil eder.

    ```javascript
    let insan = { ad: "John", yaş: 30 };
    console.log(insan.ad); // John
    console.log(insan.yaş); // 30
    ```
6. **Undefined:** Bir değişkenin değeri atanmamışsa veya bir fonksiyon bir değer döndürmezse, bu değer atanır.

    ```javascript
    let x;
    console.log(x); // undefined
    ```
7. **Null:** Bir değişkenin değerini bilinçli olarak boş bırakmak için kullanılır.

    ```javascript
    let y = null;
    console.log(y); // null
    ```
8. **Symbol:** Benzersiz ve değişmez bir veri tipini temsil eder.

    ```javascript
    const mySymbol = Symbol('açıklama');
    console.log(mySymbol);
    ```
9. **Function(Fonksiyon):** Bir fonksiyon, bir işlem veya işlevi temsil eder.

    ```javascript
    function topla(a, b) {
    return a + b;
    }

    let sonuc = topla(3, 5);
    console.log(sonuc); // 8

    ```

**4. null ile undefined arasıdaki fark nedir açıklayınız:**  Undefined,daha önce hiç referans alınmadığı, “değer yok” anlamına gelir.

Null,varlığın bilindiği yer, ancak değerin ne olduğu bilinmemektedir.

```javascript
var x; // Undefined değer
var y = null;  // Null değer
```
**5. NaN nedir açıklayınız:** Not a number yani sayısal olmayan bir değer demektir.

```javascript
var y = 3 + 'x'; // Number(y) yapmaya çalıştığımızda NaN değerini almış oluruz.
```
**6. Javascript’te yorum satırı eklemenin kaç farklı yolu vardır?** Çoklu satır ve tek satır olarak yorum ekleyebiliriz.

```javascript
// Tek satır yorumlar için

/* Birden fazla
satır
yorumlar için *\
```



**7. Global değişken ne demektir açıklayınız:**
Global scope'ta tanımlanan değişkenlere verilen addır. Global scope'un içindeki tüm scopelarda bu değişkenlere erişilebilir olur.

```javascript
var global = 5; //Bu değişkenle aynı scopeta her yerden erişilebilir. Global Değişkendir.
   ```

**8. Javascript’te this anahtar kelimesi nedir açıklayınız:**
JavaScript'teki this anahtar kelimesi, bulunduğu bağlam veya kapsam içindeki nesneyi referans alır. this, bir fonksiyonun içinde kullanıldığında, o fonksiyonun çalışma bağlamına göre değer alır. Bu bağlam, çağrıldığı yer veya bağlamın nasıl tanımlandığına bağlı olarak değişebilir.

```javascript
const obj = {
  ad: "John",
  selamla: function() {
    console.log("Merhaba, " + this.ad);
  }
};

obj.selamla(); // Merhaba, John
```
**9. == ile === farkını örnekler ile açıklayınız:**
  == type farketmeksizin veri dönüşümü yaparak değerleri karşılaştırmayı yaparken, === operatörü ise değerler yanında veri dönüşümü yapmadan karşılaştırılan verilerin type'larını da karşılaştırır.

  ```javascript
  10==10 //True
  5=="5" //True

  10===10 //True
  5==="5" //False
   ```


**10. let var const farkını tablo yapınız**

| Özellik     | `let`                  | `const`                | `var`                    |
|-------------|------------------------|------------------------|--------------------------|
| Atama       | Değiştirilebilir        | Değiştirilemez         | Değiştirilebilir        |
| Kapsam      | Blok kapsamı (Block-scoped) | Blok kapsamı (Block-scoped) | Fonksiyon kapsamı (Function-scoped) |
| Hosting     | Hoist edilir (hoisted) | Hoist edilir (hoisted) | Hoist edilir (hoisted)   |
| Tekrar Tanımlama | Tekrar tanımlanabilir | Tekrar tanımlanamaz    | Tekrar tanımlanabilir    |
| İlk Değer Atama Zorunluluğu | Opsiyonel          | Zorunlu                | Opsiyonel                |


**11. Arrow fonksiyonun normal fonksiyondan farkları nelerdir?**
* Arrow fonksiyonları new ile kullanılamaz. Yani, arrow fonksiyonları constructor olarak kullanılamaz ve this bağlamını oluşturmazlar.
* arguments nesnesine erişimleri yoktur. Arrow fonksiyonları kendi arguments nesnesini oluşturmaz.

**12. swich bloğu içinde hatasız nasıl değişken tanımlanır?**
Switch bloğunda her case'de değişken tanımlamak istiyorsak bu değişkenlerin her birinin adı farklı olması gerekir. Eğer bir değeri değiştirmek istiyorsak Switch case'den önce değişken tanımlanalarak içi doldurulur.

**13. Pure fonksiyon ne demektir açıklayınız:**
Pure fonksiyon, iki önemli özelliğe sahip bir JavaScript fonksiyon türüdür: belirli bir giriş seti için her zaman aynı çıkışı üretir ve yan etkisi yoktur. İki özellik bir araya geldiğinde, bu fonksiyonlara "pure" veya "saf" fonksiyonlar denir.

```javascript
// Pure fonksiyon örneği
function topla(a, b) {
  return a + b;
}

// Pure fonksiyon örneği
function kareAl(x) {
  return x * x;
}

```

**14. Rest operatör nedir örnekle açıklayınız:**
Rest operatörü belirsiz sayıda değişkeni bir dizi olarak kabul etmesine yarar ve bunu tanımlamayı sağlar.

```javascript
function topla(...sayilar) {
  return sayilar.reduce((toplam, sayi) => toplam + sayi, 0);
}

console.log(topla(1, 2, 3, 4, 5)); // 15
console.log(topla(10, 20)); // 30
console.log(topla()); // 0

```

**15. Object destructuring nedir örnekle açıklayınız:**
Destructuring bir object veya bir array içinden her elemanın başka bir değişken içine kaydedilmesine verilen addır. 



```javascript
const example { name: 'Alp', age:25,country:Turkey}
const name = example.name
const age = example.age
const country=example.country
// Ya da 
const {name, age,country} = example
//Şeklinde destructuring yapılabilir.
   ```

**16. 2 elemanlı bir objeyi 6 farklı şekilde oluşturunuz:**

```javascript
const obje1 = { name: "Alp", country: "Turkey" };
```
```javascript
const obje2 = new Object();
obje2.name = "Alp";
obje2.country = "Turkey";
```

```javascript
const obje3 = Object.create(null);
obje3.name = "Alp";
obje3.country = "Turkey";
```

```javascript
const obje4 = Object.assign({}, { name: "Alp", country: "Turkey" });
```

```javascript
function ObjeYapici(name, country) {
  this.name = name;
  this.country = country;
}

const obje5 = new ObjeYapici("Alp", "Turkey");
```

```javascript
const { anahtar1, anahtar2 } = { name: "Alp", country: "Turkey" };
const obje6 = { anahtar1, anahtar2 };
```

**17. 2 elemanlı bir objenin key ve value değerlerinin karakter sayısı ile 2 farklı döngü methodu kullanarak yeni bir obje oluşturunuz:**

```javascript
const obje1 = { name: "Alp", country: "Turkey" };
const yeniObje1 = {};

for (let key in obje1) {
  yeniObje1[key] = obje1[key].length; // Anahtarın değerinin karakter sayısını yeni objeye ekle
}

console.log(yeniObje1);
// Çıktı: { name: 3, country: 6 }
```

```javascript
const obje1 = { name: "Alp", country: "Turkey" };
const yeniObje2 = {};

Object.entries(obje1).forEach(([key, value]) => {
  yeniObje2[key] = value.length; // Anahtarın değerinin karakter sayısını yeni objeye ekle
});

console.log(yeniObje2);
// Çıktı: { name: 3, country: 6 }
```

**18. Cookie, local storage ve session storage farkını tablo yapınız:**

| | Cookie| Local Storage| Session Storage|
|--|--|--|--|
|  Kapasite| 4kb |5-10Mb|5Mb
|  Erişilebilirlik| Tüm pencereler |Tüm pencereler|Sekmeye özel
|  Sona erme süresi| Manuel olarak ayarlanır |Hiçbir zaman sona ermez|Sekme kapatıldığında sona erer
|  Depolama| Tarayıcı ve sunucu |Tarayıcı|Tarayıcı
|  İstekte gönderme| Evet |Hayır|Hayır

**19. asenkron ve senkron işlem farkı nedir?**
* Senkron işlemler sırayla ve adım adım çalışan işlemlerdir. Bir işlem tamamlanmadan bir sonraki başlamaz. 
* Asenkron işlemler, sırayla çalışmayan ve paralel olarak gerçekleşebilen işlemlerdir. Bir işlem başladığında bitmesini beklemek zorunda değildir, bu sırada başka bir işlem de çalışabilir. Hangi işlem önce biterse onun sonucu daha önce gösterilir.

**20. promise nedir ve neden ihtiyaç duyarız?**
Promise bir işlemin sonucunun olacağını temsil eden bir JavaScript objesidir. Eğer promise başarılı bir şekilde gerçekleşirse resolved değer döner, eğer işler ters giderse de reject olarak neden bu işlemin gerçekleşemediği döner. 
Promise'ler callback hell gibi kod karmaşasına sebep olan, okunurluğu azaltan sorunlar sebebiyle ortaya çıkmıştır. 

    
## Array Soruları
**Ödev 2**

**var dolap = ["Shirt", "Pant","TShirt"];**

**1. dolap arrayindeki son elemanı silip consola yazdırın**

```javascript
let lastItem=dolap.pop()
console.log(lastItem)
```

**2. dolap arrayindeki ilk elamanı silip yerine “Hat” elemanını gönderip consola yazdırın**
```javascript
dolap.shift()
let newItem=dolap.unshift("Hat")
console.log(newItem)
```

**3. dolap değişkeninin array olup olmadığını kontrol edin ve sonucu bir değişkene eşitleyin**

```javascript
let isArray = Array.isArray(dolap)
```
**4. dolap arrayinde “Pant” elemanın olup olmadığını 3 farklı method ile kontrol edin:**

```javascript
dolap.find((e)=>e==="Pant")
```

```javascript
dolap.includes("Pant")
```

```javascript
dolap.some((e)=>e==="Pant")
```

**5. dolap arrayindeki elemanların karakter sayısını toplayıp geriye döndürecek fonksiyonu yazın**

```javascript
function sumOfElements(arr){
    let sum=0
    for(let i=0;i<arr.length;i++){
        sum+=arr[i].length
        console.log(sum)
    }
}
sumOfElements(dolap)
```
**6. dolap arrayindki tüm elemanları büyük harfe çevirip yeni bir değişkene 3 farklı yöntemle atayın**

```javascript
const buyukHarf=dolap.map(e=>e.toUpperCase())
console.log(buyukHarf)
```
```javascript
const buyukHarf2=[]
for (let eleman of dolap){
    buyukHarf2.push(eleman.toUpperCase())
}
console.log(buyukHarf2)
```

```javascript
const buyukHarf3=[]
dolap.forEach(e=>{
    buyukHarf3.push(e.toUpperCase())
})
console.log(buyukHarf3)
```

**7. dolap arrayini index sayıları key olacak şekilde objeye çeviriniz**

```javascript
let obj = {}
Object.assign(obj, dolap)
```
**8. slice ile splice farkı nedir?**
splice() orijinal array'in değerlerini değiştirerek ekleme, silme ve yer değiştirme işlemlerini yapar. Fakat slice() orijinal array'in bir kopyasını oluşturur.

## Array Soruları 2
**const arr = [1,2,3,4,5,6,7,7,8,6,10]**

**1. arrayindeki yinelenen sayıları bulun**

```javascript
let recurringNumbers = arr.filter((item,index) => 
{return arr.indexOf(item) !== index})
```
**2. arrayindeki tüm yinelenen sayıları silip yeni bir arrayi 2 farklı method ile oluşturun**

```javascript
let newArr = arr.filter((item, index) => {
  return arr.indexOf(item) == index
})
```
```javascript
let newArr = []
for(let i=0;i<arr.length;i++){
    if(!newArr.includes(arr[i])) newArr.push(arr[i])
}
   ```

**3. arrayindeki en yüksek ve en düşük değeri 2 farklı methodla bulun**

```javascript
const highest = arr.sort((a, b) => b - a)[0]
   ```

   ```javascript
   let max=Math.max(...arr)
   ```

   ```javascript
const lowest = arr.sort((a, b) => a - b)[0]
   ```

   ```javascript
   let max=Math.min(...arr)
   ```

## Promise Soruları

## Soru 1

```javascript
// Bu kodun çıktısı nedir neden ?

function job() {
    return new Promise(function(resolve, reject) {
        reject();
    });
}

let promise = job();

promise.then(function() {
    console.log('Success 1');
}).then(function() {
    console.log('Success 2');
})
.then(function() {
    console.log('Success 3');
})
.catch(function() {
    console.log('Error 1');
}).then(function() {
    console.log('Success 4');
});
```

**Cevap1:** Kodun çıktısı Error1 ve Succes 4 olacaktır.Çünkü fonksiyon reject ile döndüğü için catch bloğu çalışır ve Error 1 yazdırır then bloğundan dolayı ardından Succes 4 yazılacaktır.


## Soru 2
```javascript
// Bu kodun çıktısı nedir neden ?
function job(state) {
return new Promise(function(resolve, reject) {
if (state) {
resolve('success');
} else {
reject('error');
}
});
}
let promise = job(true);
promise
.then(function(data) {
console.log(data);
return job(true);
})
.then(function(data) {
if (data !== 'victory') {
throw 'Defeat';
}
return job(true);
})
.then(function(data) {
console.log(data);
})
.catch(function(error) {
console.log(error);
return job(false);
})
.then(function(data) {
console.log(data);
return job(true);
})
.catch(function(error) {
console.log(error);
return 'Error caught';
})
.then(function(data) {
console.log(data);
return new Error('test');
})
.then(function(data) {
console.log('Success:'
, data.message);
})
.catch(function(data) {
console.log('Error:'
, data.message);
```

**Cevap2:** job(true) fonksiyonu 'success' olarak döndürecektir. promise.then ikinci kısmında hata fırlatılır.  Bu hata, promise.catch fonksiyonunun ilk kısmını tetikler. Bu yüzden, promise.catch ilk kısmı çalışacaktır. Bu fonksiyon, hata mesajını konsola yazdıracak ve sonra job fonksiyonunu false parametresiyle çağıracaktır. Bu fonksiyon, yeni bir Promise nesnesi döndürecektir. Bu nesne, 1 saniye sonra reject fonksiyonunu çağırarak başarısız olacaktır. Bu durumda, promise.then fonksiyonunun dördüncü kısmı çalışmayacak, promise.catch fonksiyonunun ikinci kısmı çalışacaktır. Bu fonksiyon, hata mesajını konsola yazdıracak ve "Error caught" değerini döndürecektir. Bu değer, promise.then fonksiyonunun beşinci kısmına gidecektir. Bu fonksiyon, "Error caught" değerini konsola yazdıracak ve yeni bir Error nesnesi döndürecektir. Bu nesne, "test" mesajını içerecektir. Bu nesne, promise.then fonksiyonunun altıncı kısmını çalıştırmayacak, promise.catch fonksiyonunun üçüncü kısmını çalıştıracaktır. Bu fonksiyon, hata mesajını konsola yazdıracaktır.

Çıktı: success Defeat error Error caught Error:test