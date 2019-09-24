# Apa itu CSS?

## PENGERTIAN

CSS singkatan dari Cascading Style Sheet, yakni dokumen yang berisi definisi style untuk sebuah dokumen HTML atau untuk mengatur tampilan dari dokumen HTML, meliputi layout dokumen, pewarnaan dan tampilan font dan teks dan lain sebagainya. Penulisan CSS baiknya ditulis terpisah dari konten HTML, hal ini dilakukan untuk meningkatkan daya akses konten pada web dan mengurangi kerumitan dalam penulisan kode dan struktur dari dokumen HTML.

Dengan adanya CSS, konten dan desain web akan mudah dibedakan, jadi memungkinkan untuk melakukan pengulangan pada tampilan-tampilan tertentu dalam suatu web, sehingga akan memudahkan dalam membuat halaman web yang banyak, yang pada akhirnya dapat memangkas waktu pembuatan web.

## STRUKTUR_CSS

CSS ditulis dengan format penulisan seperti berikut:

--DEFAULT--
```
    selector { property:value }
    selector { property:value; property:value }    
```

--REALITY--
```
    h1 { font-size: 20px;}

    p { height: 40px; }

    .judul {
        height: 40px;
        font-size: 20px;
    }

```
Pada contoh di atas, kita menulis h1 sebagai selector yang artinya kita ingin agar elemen `<h1>` pada HTML dikenai style. Property yang diterapkan adalah font-size untuk mengatur ukuran font, diatur dengan nilai 20px, dan property *heigth* untuk mengatur tinggi teks, diatur dengan nilai tinggi 40px.

## Teknik Penulisan CSS
Ada 3 cara untuk memasang CSS pada dokumen HTML yaitu external, internal dan inline.

### Inline Style Sheet
Pada teknik ini kita menulis kode CSS di dalam tag HTML, tepatnya di dalam atribut style.
```
    <h1 style="font-size:40px; color:orange;"> Teks Judul </h1>
```

### External Style Sheet
Teknik eksternal stylesheet adalah menuliskan kode untuk style CSS di file terpisah dengan kode HTML.
Style di definisikan di dalam file, misalkan style.css:
```
    /* style.css */

    h1 {
        font-size: 40px;
        color: orange;
    }
```
Kemudian style.css ditautkan di dalam dokumen HTML menggunakan tag `<link>`:
```
    <!-- index.html-->

    <link href="style.css" rel="stylesheet" type="text/css" />
    <h1>Teks Judul</h1>
```

## CSS Properties
Property digunakan untuk memilih jenis style apa yang akan diterapkan pada tag, class, atau id yang telah dipilih pada selector, dan pada satu selector bisa berisi beberapa property. Pada CSS terdapat banyak sekali property yang dapat digunakan untuk menghias website

Jenis property CSS di antaranya adalah:

1.background

2.border

3.box model

4.layouting

5.font & text, dll.

Karena ada begitu banyak property CSS, maka kita tidak perlu menghafal semuanya, cukup pahami apa fungsi dari property yang akan digunakan. Referensi property CSS lebih lengkap bisa dilihat di[W3SCHOOLS.COM](https://www.w3schools.com/cssref/)

## Selector
Pada CSS terdapat selector yang digunakan untuk memilih elemen HTML yang akan dikenai style. Pemilihan elemen menggunakan nama tag, nilai atribut, atau pola tertentu.

Berikut adalah contoh penulisan selector:
```
    h1 { color:red }
```
Cara membaca selector di atas adalah "Pilih elemen h1 pada document, lalu atur property color-nya menjadi red."
Terdapat dua macam tag selector yaitu single selector dan multiple selector (menargetkan tag yang berbeda dengan style yang sama), bisa kita lihat pada contoh di bawah ini:

Contoh single selector:
```
    h1 { color:red }
    p { font-size:16px }
```
Contoh multiple selector (menargetkan tag yang berbeda dengan style yang sama):
```
    h1,h2,h3,p {
    font-family: "arial", sans-sarif;
    color: #666;
}
```

## Selector dengan id dan class
Selector class digunakan untuk menentukan style juga sama seperti id. Bedanya adalah jika id hanya boleh dipanggil satu kali saja, class bisa dipanggil berkali kali pada satu halaman. Selector ini ditulis dengan awalan titik atau dot “.” pada CSS dan class=“nama-class” pada HTML. Sedangkan selector id hanya boleh dipanggil satu kali, selain itu untuk Selector ini ditulis dengan awalan pagar “#” pada CSS dan id=“nama-id” pada HTML.

Berikut contoh implementasi selector id dan class:
```
<style>
    #highlight {background-color:yellow}
    .red{color:red}
</style>
 
<h1>Penggunaan Selector Class dan Id</h1>
<p class="red">Ini selector class</p>
<p id="highlight">Ini selector id</p>
```

## Agar Lebih Paham simak vidio ini [Vidio_CSS](https://youtu.be/eE3MW_doEg0)

[Lanjut_gan!](https://github.com/arizkayusril/Frontend_RoadMap/blob/master/2.HTML/Make%20tabel/Tabel_html.md)