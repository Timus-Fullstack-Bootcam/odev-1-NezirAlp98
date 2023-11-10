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



7. Global değişken ne demektir açıklayınız
8. Javascript’te this anahtar kelimesi nedir açıklayınız
9. == ile === farkını örnekler ile açıklayınız
10. let var const farkını tablo yapınız
11. Arrow fonksiyonun normal fonksiyondan farkları nelerdir
12. swich bloğu içinde hatasız nasıl değişken tanımlanır
13. Pure fonksiyon ne demektir açıklayınız
14. Rest operatör nedir örnekle açıklayınız
15. Object destructuring nedir örnekle açıklayınız
16. 2 elemanlı bir objeyi 6 farklı şekilde oluşturunuz
17. 2 elemanlı bir objenin key ve value değerlerinin karakter sayısı ile 2 farklı döngü
methodu kullanarak yeni bir obje oluşturunuz
18. Cookie, local storage ve session storage farkını tablo yapınız
19. asenkron ve senkron işlem farkı nedir
20. promise nedir ve neden ihtiyaç duyarız

    
Array Soruları
Ödev 2
var dolap = ["Shirt", "Pant","TShirt"];

1. dolap arrayindeki son elemanı silip consola yazdırın
2. dolap arrayindeki ilk elamanı silip yerine “Hat” elemanını gönderip consola yazdırın
3. dolap değişkeninin array olup olmadığını kontrol edin ve sonucu bir değişkene
eşitleyin
4. dolap arrayinde “Pant” elemanın olup olmadığını 3 farklı method ile kontrol edin
5. dolap arrayindeki elemanların karakter sayısını toplayıp geriye döndürecek
fonksiyonu yazın
6. dolap arrayindki tüm elemanları büyük harfe çevirip yeni bir değişkene 3 farklı
yöntemle atayın
7. dolap arrayini index sayıları key olacak şekilde objeye çeviriniz
8. slice ile splice farkı nedir

const arr = [1,2,3,4,5,6,7,7,8,6,10];
1. arrayindeki yinelenen sayıları bulun
2. arrayindeki tüm yinelenen sayıları silip yeni bir arrayi 2 farklı method ile oluşturun
3. arrayindeki en yüksek ve en düşük değeri 2 farklı methodla bulun


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
Ödev 4
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
