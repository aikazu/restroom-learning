# Environment Variable

> Satu kalimat sederhana: Environment Variable itu **catatan rahasia yang ditempel di server, bukan di kode**.

## Analogi Sehari-hari

Kunci brankas tidak ditulis di dinding warung (kode yang diupload ke GitHub) — tapi disimpan di saku pemilik (server). Environment variable = "saku" itu: tempat menyimpan kunci [API](./api.md), password [DB](./db.md), yang dibaca kode saat jalan tapi tidak ikut disebar.

## Penjelasan Teknikal

Namanya ditulis kapital dengan underscore: `SUPABASE_URL`, `SUPABASE_KEY`. Di kode dibaca lewat `process.env.NAMA`. Di Cloudflare Pages diisi lewat dashboard (Settings → Environment Variables). **Jangan pernah** menulis kunci asli di kode / chat / screenshot.

## Contoh TypeScript (kalau relevan)

```ts
// Benar: baca dari saku server
const key: string | undefined = process.env.SUPABASE_KEY;

// Salah: kunci ditulis di dinding (jangan lakukan ini!)
// const key = "eyJhbGciOi...asli...";
```

## Kapan Kamu Ketemu Istilah Ini?

Saat menghubungkan frontend ke Supabase atau layanan apa pun yang butuh kunci.

## Istilah Terkait

- [Supabase](./supabase.md)
- [Deploy](./deploy.md)
- [API](./api.md)
