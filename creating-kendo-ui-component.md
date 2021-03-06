---
description: >-
  Komponen itu satu buah elemen penyusun aplikasi yang bisa berdiri sendiri,
  mulai dari yang paling kecil seperti Button hingga yang cukup kompleks seperti
  DataGrid, Calendar, dan Spreadsheet.
---

# Creating Kendo UI Component

## Overview

Ada banyak cara untuk meng-instansiasi komponen. Berikut ini dijelaskan beberapa contohnya, terurut kemudahan implementasi.

## Metode Imperative \(Prosedural\)

Metode imperative dilakukan dengan memanggil fungsi dan memberikan parameter yang sesuai melalui kode javascript.

### Ala jQuery

```markup
<input type="text" id="datepicker1">

<script>
var dp1 = $('#datepicker1').kendoDatePicker({format:"d-M-yyyy"});
</script>
```

### Ala Kendo UI

```markup
<input type="text" id="datepicker2">

<script>
var dp2 = new kendo.ui.DatePicker(document.getElementById('datepicker2'), {format:"d-M-yyyy"}); 
</script>
```

## Metode Deklaratif

Metode deklaratif dilakukan dengan menambahkan `data-role="componentname"` di tag HTML. Selain nama komponen, parameter juga bisa diletakkan sebagai `data-parameter-name="value"`.

{% hint style="info" %}
Passing parameter melalui atribut `data-parameter-name` juga berlaku untuk metode prosedural.
{% endhint %}

### Via kendo.init\(\)

```markup
// TODO
```

### Via kendo.Views\(\)

```markup
// TODO
```

### Via kendo.observable\(\) a.k.a MVVM Pattern

```markup
// TODO
```



### 

