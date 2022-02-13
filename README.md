# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### Screenshot

![](./images/screenshot.png)

### Links

- Solution URL: [repository](https://github.com/eLAmaravati/qr-code)
- Live Site URL: [live site](https://elamaravati.github.io/qr-code/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

Goal-nya adalah membuat komponen QR code dengan tinggi dan lebar tertentu. Bagian paling tricky adalah menempatkan komponen tersebut tepat di tengah-tengah halaman sedangkan atribut tetap berada di bawah.

Ada solusi yang lebih sederhana: flexbox. Tapi karena sekarang masih melatih grid (lagi), maka saya menggunakan grid. Kali ini tidak menggunakan property grid-templates-areas, tapi langsung grid. Membagi halaman (dalam hal ini body) ke dalam 9 kolom dan dua baris.

Tantangan lainnya adalah mengatur tinggi dan lebar komponen qr code. Apakah harus menggunakan satuan relatif atau absolut? Saya memutuskan untuk menggunakan absolut (px).

```css
body {
  background-color: var(--light-gray);
  font-family: "Outfit", sans-serif;
  display: grid;
  grid: auto / repeat(9, 1fr);
  grid-gap: 10px;
}
```

### Continued development

Menambahkan display grid ke body sepertinya bukan best practise jika diterapkan di riil web development.

## Author

- Website - [Langit Amaravati](https://www.langitamaravati.com)
- Frontend Mentor - [@eLAmaravati](https://www.frontendmentor.io/profile/eLAmaravati)
- Twitter - [@eLAmaravati](https://www.twitter.com/elamaravati)
