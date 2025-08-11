# Panduan Kontribusi

## Alur Kerja (GitHub Flow)
1. Buat Issue (jelas & kecil), isi Acceptance Criteria.
2. Buat branch dari `main`: `issue-<nomor>-<slug-singkat>`.
3. Commit kecil & deskriptif (boleh format Conventional Commits: feat/fix/docs/chore/refactor/test).
4. Push branch → buat Pull Request (PR) berisi konteks + `Closes #<nomor>`.
5. Pastikan CI hijau. Perbaiki jika gagal.
6. Review → Merge → Hapus branch.

## Konvensi
- **Nama branch**: `issue-12-motivasi`, `fix-34-typo-docs`
- **Commit message**: `feat: tambah quote motivasi`
- **PR**: sertakan ringkasan, dampak, cara uji, dan checklist.

## Review Checklist (untuk reviewer)
- [ ] Perubahan fokus & relevan dengan Issue
- [ ] Kode mudah dipahami; tidak ada `debug` tersisa
- [ ] Tidak ada rahasia/kredensial dalam repo
- [ ] CI hijau; langkah uji jelas
- [ ] Dokumen diperbarui bila perlu
