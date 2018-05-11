# Basic Usage

## Creating Spreadsheet Component

Sama seperti komponen lainnya, untuk membuat sebuah spreadsheet, langkah minimal yang diperlukan adalah membuat satu elemen DOM dan satu baris kode Javascript.

```markup
<div id="spreadsheet"></div>

<script>
    $('#spreadsheet').kendoSpreadsheet();
</script>
```

![Basic spreadsheet](../.gitbook/assets/image%20%282%29.png)

Silakan dieksplorasi apa saja yang bisa dilakukan terhadap spreadsheet tersebut. Sangat mirip dengan fungsionalitas yang disediakan Excell. 

Bahkan spreadsheet Kendo UI juga mampu membuka file Excell dan menampilkan isinya \(preview\), tanpa perlu mengirim file ke server terlebih dahulu. Semuanya murni dilakukan di browser \(client side\).

{% hint style="warning" %}
Untuk bisa memanfaatkan fitur preview, kamu harus menambahkan satu file lagi untuk di-include di template HTML:  
`<script src="js/jszip.min.js"></script>`
{% endhint %}

Jika tidak ditambahkan, akan muncul error **`Uncaught ReferenceError: JSZip is not defined`**.

