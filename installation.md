# Installation & Integration

### 1. Download

Source code Kendo UI versi jQuery bisa di-download di [https://www.telerik.com/kendo-ui](https://www.telerik.com/kendo-ui). Ada beberapa versi lain seperti Vue, React, atau Angular, tetapi kita akan menggunakan jQuery sebagai contoh karena paling mudah dan paling dikenali oleh programmer pemula. 

### 2. Ekstrak dan setup HTML

Setelah diekstrak, ada 2 folder utama yang dibutuhkan yaitu `styles` dan `js`. Salin 2 folder tersebut ke direktori proyek lalu include di main template:

```css
<head>
    <link href="styles/kendo.common.min.css" rel="stylesheet" type="text/css"/>
    <link href="styles/kendo.default.min.css" rel="stylesheet" type="text/css"/>
```

```javascript
// CONTENT

    <script src="js/jquery.min.js"></script>
    <script src="js/kendo.web.min.js"></script>

// OTHERS SCRIPT HERE

</body>
```

Lalu cobalah bermain-main dengan membuat elemen HTML biasa seperti form, tabel, list, heading, dan lain-lain.

**SURPRISE!!!**

![Style bawaan HTML tidak di-override oleh Kendo UI](.gitbook/assets/image%20%281%29.png)

Berbeda dengan Bootstrap yang ketika CSS-nya di-include tampilan HTML web langsung kelihatan cantik, Kendo UI ternyata tidak memberikan style default kepada elemen HTML.

Di Kendo UI, kita perlu melakukan instansiasi secara manual kepada setiap komponen sesuai kebutuhan.





