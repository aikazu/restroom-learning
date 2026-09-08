# TypeScript

> Satu kalimat sederhana: TypeScript itu **JavaScript yang dikasih label** biar tidak gampang salah.

## Analogi Sehari-hari

JavaScript seperti koper tanpa label — isinya bisa baju, bisa batu bata, kamu baru tahu saat dibuka (saat program jalan → error). TypeScript menempel **label di tiap koper** (`string`, `number`): kalau kamu salah masukkan barang, langsung ditegur sebelum berangkat.

## Penjelasan Teknikal

TypeScript = JavaScript + **tipe data**. Browser tetap menjalankan JavaScript, tapi TypeScript mengecek kesalahan lebih awal saat kamu ngoding. Contoh label yang sering dipakai: `string` (teks), `number` (angka), `boolean` (ya/tidak), dan tipe buatan sendiri dengan `type`.

## Contoh TypeScript (kalau relevan)

```ts
// Tanpa label: salah isi baru ketahuan belakangan. Dengan label: langsung ketahuan.
type Proyek = {
  judul: string;
  tahun: number;
  link?: string; // tanda ? artinya boleh kosong
};

const p1: Proyek = { judul: "Portfolio", tahun: 2026 };
```

## Kapan Kamu Ketemu Istilah Ini?

Di semua contoh kode repo ini. File-nya berakhiran `.ts`.

## Istilah Terkait

- [Frontend](./frontend.md)
- [Framework](./framework.md)
- [Component](./component.md)
