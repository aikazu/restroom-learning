# Frontend

> Satu kalimat sederhana: Frontend itu bagian website yang **dilihat dan diklik** pengunjung.

## Analogi Sehari-hari

Bayangkan sebuah restoran. Frontend adalah **ruang makannya**: meja, menu, dekorasi, lampu. Pengunjung tidak perlu tahu dapurnya seperti apa — yang penting mereka bisa lihat menu dan memesan dengan nyaman.

## Penjelasan Teknikal

Frontend berjalan di **browser** (Chrome, Safari, dst). Isinya tiga hal:

1. **Struktur** — teks, gambar, tombol apa saja yang tampil.
2. **Tampilan** — warna, jarak, font, animasi.
3. **Interaksi** — apa yang terjadi saat tombol diklik atau form diisi.

Di repo ini frontend ditulis dengan [TypeScript](./typescript.md) dan biasanya di-host di [Cloudflare](./cloudflare.md).

## Contoh TypeScript (kalau relevan)

```ts
// Contoh paling kecil: teks sambutan di portfolio
const nama: string = "Iqbal";
const sapaan: string = `Halo, saya ${nama} — saya bikin web.`;
document.title = sapaan;
```

## Kapan Kamu Ketemu Istilah Ini?

Setiap kali materi bilang "tampilan portfolio", "halaman web", atau "yang dilihat pengunjung" — itu Frontend.

## Istilah Terkait

- [Backend](./backend.md)
- [Component](./component.md)
- [Responsive](./responsive.md)
