# Spam

> Satu kalimat sederhana: Spam itu **pesan sampah massal** — iklan / penipuan yang tidak kamu minta.

## Analogi Sehari-hari

Seperti brosur pinjol yang diselipkan ke kotak surat rumahmu tiap hari oleh orang tak dikenal. Form kontak yang online tanpa perlindungan = kotak surat tanpa gembok: cepat penuh brosur sampah (atau lebih parah: skrip bot).

## Penjelasan Teknikal

Perlindungan dasar yang cukup untuk portfolio (gratis):

1. Validasi + batas panjang pesan.
2. Honeypot: kolom jebakan tak terlihat — bot mengisinya, manusia tidak.
3. Rate limit di [Supabase](./supabase.md): satu orang tidak bisa kirim 100x/menit.
4. (Opsional) CAPTCHA kalau sudah diserang.

## Kapan Kamu Ketemu Istilah Ini?

Di modul form kontak + checklist "siap online".

## Istilah Terkait

- [Form](./form.md)
- [Supabase](./supabase.md)
