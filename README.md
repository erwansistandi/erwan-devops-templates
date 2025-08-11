# Erwan DevOps Templates

[![Use this template](https://img.shields.io/badge/Use%20this%20template-💡-brightgreen)](https://github.com/erwansistandi/erwan-devops-templates/generate)
[![CI](https://github.com/erwansistandi/erwan-devops-templates/actions/workflows/ci.yml/badge.svg)](https://github.com/erwansistandi/erwan-devops-templates/actions/workflows/ci.yml)
[![Issues](https://img.shields.io/github/issues/erwansistandi/erwan-devops-templates)](https://github.com/erwansistandi/erwan-devops-templates/issues)

Repo template untuk menstandarkan **Issue → Branch → PR + CI**. Cocok dipakai ulang di semua proyek DevOps kamu.

## Cara pakai
1. Klik tombol **Use this template** (di atas repo atau badge hijau di atas).
2. Isi nama repo baru → **Create repository from template**.
3. Buka tab **Actions** (aktifkan jika diminta) → pastikan workflow **CI** berjalan.

## Isi penting
- `.github/ISSUE_TEMPLATE/*` — template Issue (feature, bug)
- `.github/pull_request_template.md` — template PR
- `.github/workflows/ci.yml` — workflow CI minimal
- `CONTRIBUTING.md` — panduan kontribusi & konvensi

## Workflow singkat
Issue → Branch → PR (`Closes #N`) → CI → Review → Merge → Hapus branch

## Contoh cepat

```bash
git switch main && git pull
git checkout -b issue-12-motivasi
echo "Tetap konsisten. Progres kecil menang." >> catatan.txt
git add . && git commit -m "feat: tambah quote motivasi (Closes #12)"
git push -u origin issue-12-motivasi
# buka PR: compare main...issue-12-motivasi

## README — Badge tambahan
Tambahkan badge berikut bila perlu (ganti `erwansistandi/erwan-devops-templates` sesuai repo kamu):

```markdown
[![Use this template](https://img.shields.io/badge/Use%20this%20template-💡-brightgreen)](https://github.com/erwansistandi/erwan-devops-templates/generate)
[![CI](https://github.com/erwansistandi/erwan-devops-templates/actions/workflows/ci.yml/badge.svg)](https://github.com/erwansistandi/erwan-devops-templates/actions/workflows/ci.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-ff69b4.svg)](CONTRIBUTING.md)

[![Release](https://img.shields.io/github/v/release/erwansistandi/erwan-devops-templates?display_name=tag)](https://github.com/erwansistandi/erwan-devops-templates/releases)
