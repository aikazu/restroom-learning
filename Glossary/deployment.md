# Deployment

> Satu kalimat sederhana: Deployment itu **proses menerbitkan** websitemu dari laptop ke internet.

## Analogi Sehari-hari

Seperti menerbitkan buku: naskah di laptop (draf) → dicetak → dipajang di toko buku (bisa dibeli orang). Deployment = langkah "cetak + pajang"-nya website.

## Penjelasan Teknikal

Alurnya: kode di [Repo](./repo.md) → dibuild (dirapikan jadi file siap saji) → diupload ke [Hosting](./hosting.md) → dapat URL publik. Di Cloudflare Pages ini otomatis: tiap kamu push ke Git, deployment baru jalan sendiri (disebut CI/CD sederhana).

```mermaid
flowchart LR
  A[Kode di Git] --> B[Build otomatis]
  B --> C[Upload ke Hosting]
  C --> D[Online! Ada URL-nya]
```

Cara baca diagramnya: alur kiri ke kanan, tiap kotak adalah tahap. Kalau ada yang gagal (misal build error), proses berhenti dan kamu dapat laporannya.

## Kapan Kamu Ketemu Istilah Ini?

Setiap kali materi bilang "publish", "online-kan", "naik ke production".

## Istilah Terkait

- [Deploy](./deploy.md)
- [Hosting](./hosting.md)
- [Git](./git.md)
