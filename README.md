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
- [Author](#author)

## Overview

### Screenshot

![](./images/screenshot.png)

### Links

- Solution URL: [repository](https://github.com/eLAmaravati/qr-code-component)
- Live Site URL: [live site](https://elamaravati.github.io/qr-code-component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

Goal-nya adalah membuat komponen QR code dengan tinggi dan lebar tertentu. Bagian paling tricky adalah menempatkan komponen tersebut tepat di tengah-tengah halaman sedangkan atribut tetap berada di bawah.

Karena sekarang masih melatih grid (lagi), maka saya menggunakan grid dan membuat solusi seperti ini:

- Membagi body ke dalam 3 kolom dan 3 baris. Height dan max-height tidak ditentukan.
- Membiarkan baris pertama untuk ruang kosong karena tinggi konten utama tidak diketahui (auto).
- Menempatkan main container (konten utama) di baris pertama, penuh 3 kolom.
- Menempatkan footer di baris ketiga, penuh 3 kolom. Dengan begini, footer akan tetap berada di bawah konten tak peduli berapa pun ukuran layarnya.

Main container:

- Display flex dan mengatur lebar konten sesuai dengan breakpoints menggunakan flex-basis.

```css
body {
  background-color: var(--light-gray);
  font-family: "Outfit", sans-serif;
  height: 100vh;
  display: grid;
  grid: repeat(3, 1fr) / repeat(3, 1fr);
}
```

### Continued development

- Saya masih ragu apakah menggunakan grid langsung di body merupakan best practise?
- Menggunakan shorthand untuk property grid agar CSS lebih ringkas.

## Author

- Website - [Langit Amaravati](https://www.langitamaravati.com)
- Frontend Mentor - [@eLAmaravati](https://www.frontendmentor.io/profile/eLAmaravati)
- Twitter - [@eLAmaravati](https://www.twitter.com/elamaravati)
