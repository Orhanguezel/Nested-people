# İç İçe Nesneler Görevi

## Görev 1

Aşağıdaki nesne verildi:

```javascript
let person = {
    name: "Petra Morin",
    address: {
        delivery: {
            street: "371-7636 Nulla Road",
            zip: "83-315",
            country: "Germany",
        },
        billing: {
            street: "123-999 Fake Street",
            zip: "12345",
            country: "Germany",
        }
    },
    hobbies: ["drums", "skating", "comics"],
    languages: [
        {
            name: "German",
            level: 5 
        },
        {
            name: "English",
            level: 4 
        },
        {
            name: "Spanish",
            level: 2 
        },
    ]
};
```

### Görev 1.1

Fatura adresinin posta kodunu konsola yazdırın

Beklenen çıktı:

```plaintext
12345
```

### Görev 1.2

Son hobiyi yazdırın

Beklenen çıktı:

```plaintext
comics
```

### Görev 1.3

İkinci konuşulan dilin adını ve seviyesini yazdırın

Beklenen çıktı:

```plaintext
English: 4
```

### Görev 1.4

Teslimat adresi ile ilgili tüm bilgileri yazdırın.

Beklenen çıktı:

```plaintext
Street: 371-7636 Nulla Road
Zip: 83-315
Country: Germany
```

### Görev 1.5

Bir döngü kullanarak tüm hobileri, her biri ayrı satırda olacak şekilde yazdırın

Beklenen çıktı:

```plaintext
Hobbies: 
- drums
- skating
- comics
```

### Görev 1.6

Bir döngü kullanarak, seviyesi 5’ten küçük olan tüm dilleri ve seviyelerini listeleyin.

Beklenen çıktı:

```plaintext
English: 4
Spanish: 2
```

## Görev 2

Aşağıdaki kişi listesine sahip olan bir dizi verildi:

```javascript
const users = [
  {
    name: "Petra Morin",
    address: {
        delivery: {
            street: "371-7636 Nulla Road",
            zip: "83-315",
            country: "Germany",
        },
        billing: {
            street: "123-999 Fake Street",
            zip: "12345",
            country: "Germany",
        }
    },
    hobbies: ["drums", "skating", "comics"],
    languages: [
        {
            name: "German",
            level: 5 
        },
        {
            name: "English",
            level: 4 
        },
        {
            name: "Spanish",
            level: 2 
        },
    ]
  },
  {
    name: "Abel Ashley",
    address: {
        delivery: {
            street: "9977 Aliquam Avenue",
            zip: "920134",
            country: "Mexico",
        },
        billing: {
            street: "123 Lorem Square",
            zip: "912098",
            country: "Mexico",
        }
    } ,
    hobbies: ["reading books", "wood working"],
    languages: [
        {
            name: "Spanish",
            level: 5 
        },
        {
            name: "English",
            level: 5 
        },
        {
            name: "Italian",
            level: 3 
        },
    ]
  },
  {
    name: "Aaron Cardenas",
    address: {
        delivery: {
            street: "987 Ipsum",
            zip: "129-234",
            country: "France",
        },
        billing: {
            street: "123 Etwas Plaza",
            zip: "912098",
            country: "Spain",
        }
    },
    hobbies: ["painting", "singing", "hiking"],
    languages: [
        {
            name: "French",
            level: 5 
        },
        {
            name: "Spanish",
            level: 5 
        },
        {
            name: "German",
            level: 1 
        },
    ]
  },
  {
    name: "Felix Moreno",
    address: {
        delivery: {
            street: "320-7871 Nec, Av.",
            zip: "59156",
            country: "New Zealand",
        },
        billing: {
            street: "921 Nullae Aliquam",
            zip: "912098",
            country: "New Zealand",
        }
    }, 
    hobbies: ["jogging", "coffee", "bird watching"],
    languages: [
        {
            name: "English",
            level: 5 
        },
        {
            name: "Italian",
            level: 3 
        },
    ]
  },
  {
    name: "Skyler May",
    address: {
        delivery: {
            street: "Ap #854-6462 Consectetuer Ave",
            zip: "00608",
            country: "Singapore",
        },
        billing: {
            street: "Ap #854-6462 Consectetuer Ave",
            zip: "00608",
            country: "Singapore",
        }
    },
    hobbies: ["cycling", "soccer", "bouldering"],
    languages: [
        {
            name: "Malay",
            level: 5 
        },
        {
            name: "English",
            level: 5 
        },
        {
            name: "Mandarin",
            level: 4 
        },
        {
            name: "French",
            level: 2 
        },
    ]
  },
];
```

### Görev 2.1

Listedeki son kişinin adını ve hobilerini virgülle ayrılmış bir şekilde yazdırın.

Beklenen çıktı:

```plaintext
Skyler May
Hobbies: cycling, soccer, bouldering
```

### Görev 2.2

Listedeki ikinci kişinin adını ve fatura adresi bilgilerini yazdırın.

Beklenen çıktı:

```plaintext
Abel Ashley

Billing address:

Street: 123 Lorem Square
Zip: 912098
Country: Mexico
```

### Görev 2.3

Döngüler kullanarak listedeki tüm kişilerin isimlerini yazdırın.

Her isim için, 1’den başlayarak bir sıra numarası da yazdırın.

Beklenen çıktı:

```plaintext
1. Petra Morin
2. Abel Ashley
3. Aaron Cardenas
4. Felix Moreno
5. Skyler May
```

### Görev 2.4

Döngüler kullanarak, listedeki her bir kişi için adını, teslimat ülkesini ve listedeki ilk hobisini içeren bir mesaj yazdırın.

Beklenen çıktı:

```plaintext
Petra Morin lives in Germany and their favourite hobby is: drums.

Abel Ashley lives in Mexico and their favourite hobby is: reading books.

Aaron Cardenas lives in France and their favourite hobby is: painting.

Felix Moreno lives in New Zealand and their favourite hobby is: jogging.

Skyler May lives in Singapore and their favourite hobby is: cycling.
```

### Görev 2.5

Döngüler kullanarak, her kişinin adını ve seviye 4 veya daha yüksek olan tüm dillerini listeleyin.

Beklenen çıktı:

```plaintext
Petra Morin speaks fluently:
- German
- English

Abel Ashley speaks fluently:
- Spanish
- English

...
```