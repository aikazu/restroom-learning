# Git

> Satu kalimat sederhana: Git itu **mesin waktu untuk kodemu** — bisa undo, bisa cabang cerita.

## Analogi Sehari-hari

Nulis skripsi: `skripsi-final.docx`, `skripsi-final2.docx`, `skripsi-final-beneran.docx`... Git menggantikan kekacauan itu dengan riwayat rapi: tiap "save point" (commit) tercatat siapa, kapan, apa yang berubah — dan kamu bisa kembali ke titik mana pun.

## Penjelasan Teknikal

Perintah intinya cuma 4: `add` (pilih perubahan), `commit` (simpan titik), `push` (kirim ke GitHub), `pull` (ambil update). Cloudflare Pages memakai riwayat Git ini untuk auto-[Deploy](./deploy.md): tiap push = versi online baru.

```mermaid
flowchart LR
  A[Ubah kode] --> B[commit: titik save]
  B --> C[push ke GitHub]
  C --> D[Cloudflare auto-deploy]
```

Cara baca diagramnya: alur kiri ke kanan seperti menyimpan game lalu lanjut main — tiap commit adalah save slot.

## Kapan Kamu Ketemu Istilah Ini?

Dari hari pertama ngoding. Semua deploy modern berangkat dari Git.

## Istilah Terkait

- [Repository](./repository.md)
- [Deploy](./deploy.md)
