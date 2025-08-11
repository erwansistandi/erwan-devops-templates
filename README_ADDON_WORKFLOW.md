## Workflow: Issue → Branch → PR + CI

- **Issue** = tiket pekerjaan; tulis *apa, kenapa, bagaimana, acceptance criteria*.
- **Branch** = jalur aman untuk mengerjakan 1 isu tanpa ganggu `main`.
- **PR** = pengajuan perubahan + ruang review. Gunakan `Closes #<nomor>`.
- **CI** = pemeriksaan otomatis setiap push/PR.

### Contoh cepat
```bash
git switch main && git pull
git checkout -b issue-12-motivasi
echo "Tetap konsisten. Progres kecil menang." >> catatan.txt
git add . && git commit -m "feat: tambah quote motivasi (Closes #12)"
git push -u origin issue-12-motivasi
# buka PR: compare main...issue-12-motivasi