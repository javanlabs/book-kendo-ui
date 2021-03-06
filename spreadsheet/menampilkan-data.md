# Menampilkan Data

Ada 3 cara untuk menampilkan data ke spreadsheet:

1. Via constructor parameter
2. Via method range\(\).values\(\)
3. Via data binding

## Via constructor

Metode ini digunakan jika data yang ingin ditampilkan sudah diketahui sejak pertama kali halaman ditampilkan.

```javascript
$('#spreadsheet').kendoSpreadsheet({
    sheets: [
        {
            name: "Jadwal Piket",
            mergedCells: [
                "A1:G1"
            ],
            rows: [
                {
                    cells:[
                        {value: "Jadwal Piket Bulan Agustus", textAlign: "center"}
                    ]
                },
                {
                    cells: [
                        {value: "Minggu Ke"},
                        {value: "Senin"},
                        {value: "Selasa"},
                        {value: "Rabu"},
                        {value: "Kamis"},
                        {value: "Jumat"},
                        {value: "Sabtu"},
                    ]
                },
                {
                    cells: [
                        {value: "1"},
                        {value: "Andi"},
                        {value: "Bayu"},
                        {value: "Citra"},
                        {value: "Dimas"},
                        {value: "Eko"},
                        {value: "Fitra"},
                    ]
                },
            ]
        }
    ]
});
```

 Pada kasus nyata, parameter `rows` ini bisa digenerate secara dinamis dari backend.

## Via method sheet.range\(\).values\(\)

Metode ini digunakan jika data tidak harus ditampilkan di awal, tetapi bisa nanti \(setelah ada trigger tertentu\).

```javascript
// Inisiasi spreadsheet
$('#spreadsheet').kendoSpreadsheet();

// Dapatkan instance spreadsheet
var spreadsheet = $("#spreadsheet").data("kendoSpreadsheet"); 

// Karena satu spreadsheet terdiri dari beberapa sheets,
// maka kita perlu menentukan sheet yang mana yang akan dimodifikasi.
var sheet = spreadsheet.activeSheet(); // bisa juga menggunakan method sheetByName() atau sheetByIndex()


// Insert data pada range tertentu
sheet.range("A3:G3").values([["1", "Andi", "Bayu", "Citra", "Dani", "Eko", "Fitra"]]);

```

## Via Data Binding

```javascript
// TODO
```



{% hint style="info" %}
Ketiga method di atas tentunya bisa di-mix and match, tidak harus strict pada satu method tertentu. Bisa saja kita menampilkan data awal via constructor atau data binding, lalu data lainnya ditambahkan menggunakan method `values()` secara dinamis.
{% endhint %}



