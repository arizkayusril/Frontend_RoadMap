#Membuat Layout dengan `<div>`

Untuk membuat layout dengan tag `<div>`, kita membutuhkan style CSS.
Membuat kerangka / struktur Layout:

```<div id="header">
        Header
    </div>
    <div id="sidebar">
        Sidebar
    </div>
    <div id="content">
        Content
    </div>
    <div id="footer">
        Footer
    </div>
```
Pada baris kode di atas, akan menghasilkan output seperti di bawah ini, belum terlihat seperti sebuah layout.

AY1g4zXk3079gXILjDgYqVKZux8lpJVV-JTh7tXJa1DCe2vT1jm2TCqZtdiBHugjJ6nnfXmzQh0NjbwBlBg5U6dtt63Tijckk_r3VtGptLVWfqadSlL4xHtJF_f7xwFLzToS7XjB

Untuk membuatnya menjadi sebuah layout, kita harus menambahkan style css berdasarkan id yang dipanggil oleh masing-masing `<div>`.
Menambah style CSS:

```
    <style>
    #header
    {
        background  : #00ccff;
        height      : 10%;
        font-size   : 1.5em;
        text-align  :center;
        padding-top : 20px;
    }
    #sidebar
    {
        background  : #99ccff;  
        float       : left;
        height      : 400px;
        width       :30%;
        font-size   : 1.5em;
        text-align  :center;
        padding-top : 20px;
    
    }
    #content
    {
        background  : #9999ff;
        float       : right;
        width       : 70%;
        height      : 400px;
        font-size   : 1.5em;
        text-align  :center;
        padding-top : 20px;
    }
    #footer
    {
        background  : #3399ff;
        clear       : both;
        font-size   : 1.5em;
        text-align  :center;
    }
    </style>
```

Mengaitkan struktur layout html dengan style CSS:
```
    <style>
    #header
    {
        background  : #00ccff;
        height      : 10%;
        font-size   : 1.5em;
        text-align  :center;
        padding-top : 20px;
    }
    #sidebar
    {
        background  : #99ccff;  
        float       : left;
        height      : 400px;
        width       :30%;
        font-size   : 1.5em;
        text-align  :center;
        padding-top : 20px;
    
    }
    #content
    {
        background  : #9999ff;
        float       : right;
        width       : 70%;
        height      : 400px;
        font-size   : 1.5em;
        text-align  :center;
        padding-top : 20px;
    }
    #footer
    {
        background  : #3399ff;
        clear       : both;
        font-size   : 1.5em;
        text-align  :center;
    }
    </style>
    <div id="header">
        Header
    </div>
    <div id="sidebar">
        Sidebar
    </div>
    <div id="content">
        Content
    </div>
    <div id="footer">
        Footer
    </div>
```

Jika kode di atas dijalankan maka akan menghasilkan layout seperti gambar di bawah ini :
[alt text!](https://lh5.googleusercontent.com/jPDNc7ICky1u0zH1WHHXS0eZPpgbJWGzkr3WifrWWOUGn2j0ZHbr6Cn8UUJA9hnfvtlnfC5DmMIOz1m5eJrby86gWxISWbhhFXzEcycl9LJUmrrehBATHpT3RMCcRBzRfZ6oXQUT)
