# Component

> Satu kalimat sederhana: Component itu **potongan LEGO** pembentuk halaman web.

## Analogi Sehari-hari

Halaman portfolio seperti susunan LEGO: balok "Header", balok "Kartu Proyek", balok "Tombol Kontak". Satu desain balok bisa dipakai ulang (3 kartu proyek = 1 desain dipakai 3 kali). Rusak satu balok? Ganti balok itu saja, tidak bongkar semua.

## Penjelasan Teknikal

Component = fungsi [TypeScript](./typescript.md) yang mengembalikan potongan tampilan. Menerima data (props) dan menampilkan sesuai data itu.

## Contoh TypeScript (kalau relevan)

```ts
// Satu desain kartu, dipakai untuk semua proyek
type KartuProyek = {
  judul: string;
  deskripsi: string;
};

function Kartu({ judul, deskripsi }: KartuProyek): string {
  return `<article><h3>${judul}</h3><p>${deskripsi}</p></article>`;
}
```

## Kapan Kamu Ketemu Istilah Ini?

Di modul anatomi portfolio: header, hero, kartu proyek, footer — semuanya component.

## Istilah Terkait

- [Frontend](./frontend.md)
- [Framework](./framework.md)
