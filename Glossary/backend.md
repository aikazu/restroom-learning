# Backend

> Satu kalimat sederhana: Backend itu **dapur di balik layar** yang mengolah data dan aturan.

## Analogi Sehari-hari

Lanjut analogi restoran: Backend adalah **dapur + kasir**. Pengunjung tidak masuk dapur, tapi pesanan mereka dimasak di sana, dicatat di kasir, dan hasilnya diantar ke meja ([Frontend](./frontend.md)).

## Penjelasan Teknikal

Backend biasanya mengurus:

- Menerima permintaan dari frontend lewat [API](./api.md).
- Menyimpan / mengambil data dari [Database](./database.md).
- Aturan bisnis: siapa boleh apa, validasi form, anti-[Spam](./spam.md).

Kabar baik untuk pemula: di arsitektur repo ini kamu **jarang bikin backend dari nol** — [Supabase](./supabase.md) sudah menyediakannya (database + auth + API otomatis).

## Contoh TypeScript (kalau relevan)

```ts
// "Backend" versi Supabase: simpan pesan kontak tanpa bikin server sendiri
import { createClient } from "@supabase/supabase-js";

const supabase = createClient(process.env.SUPABASE_URL!, process.env.SUPABASE_KEY!);

async function simpanPesan(nama: string, pesan: string): Promise<void> {
  await supabase.from("pesan").insert({ nama, pesan });
}
```

## Kapan Kamu Ketemu Istilah Ini?

Saat materi bilang "data disimpan di ...", "form dikirim ke ...", atau "login dicek oleh ..." — itu Backend.

## Istilah Terkait

- [Frontend](./frontend.md)
- [API](./api.md)
- [Supabase](./supabase.md)
