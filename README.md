# GitHub Collab Demo

Repo contoh untuk **Weekly Meet 3 Catalyst: Collaborative Development with GitHub** (Software Development).

Isi repo ini bukan website sungguhan. Repo ini dibuat sebagai **contoh alur kerja tim** supaya kamu bisa melihat langsung seperti apa Issue, Branch, Pull Request, Code Review, dan Merge Conflict di GitHub.

## Peta isi repo

| Konsep di materi | Lihat di sini |
|---|---|
| GitHub Issues (title, description, acceptance, assignee, label) | [Issue #1](https://github.com/DevinRafa/github-collab-demo/issues/1) sampai [#5](https://github.com/DevinRafa/github-collab-demo/issues/5) |
| Issue → Branch → Commit → Pull Request → Merge → Delete Branch | [Issue #1](https://github.com/DevinRafa/github-collab-demo/issues/1) → [PR #6](https://github.com/DevinRafa/github-collab-demo/pull/6) (sudah merged, branch sudah dihapus) |
| PR description (Changes / Related Issue / Testing) | [PR #7](https://github.com/DevinRafa/github-collab-demo/pull/7) |
| `Closes #N` menutup issue otomatis | PR #6 menutup Issue #1 |
| Code review dengan komentar yang membangun | [PR #8](https://github.com/DevinRafa/github-collab-demo/pull/8), tab *Files changed* |
| Merge conflict | [PR #10](https://github.com/DevinRafa/github-collab-demo/pull/10) dan [PR #9](https://github.com/DevinRafa/github-collab-demo/pull/9) |
| Latihan memperbaiki bug | [Issue #4](https://github.com/DevinRafa/github-collab-demo/issues/4) |

## Skenario demo (tinggal klik)

1. **Merge bersih.** Buka [PR #7](https://github.com/DevinRafa/github-collab-demo/pull/7) (Create Navbar), klik *Merge pull request*, lalu *Confirm merge*. Issue #2 otomatis tertutup karena deskripsi PR berisi `Closes #2`.
2. **Code review.** Buka [PR #8](https://github.com/DevinRafa/github-collab-demo/pull/8), masuk tab *Files changed*, baca komentar di baris 10, klik *Resolve conversation*, lalu merge. Issue #3 otomatis tertutup.
3. **Merge conflict.**
   - Merge [PR #10](https://github.com/DevinRafa/github-collab-demo/pull/10) (Dev A) lebih dulu.
   - Buka [PR #9](https://github.com/DevinRafa/github-collab-demo/pull/9) (Dev B). GitHub akan menampilkan *This branch has conflicts that must be resolved*.
   - Klik *Resolve conflicts*. Pilih atau gabungkan salah satu baris `<h1>`, lalu hapus penanda `<<<<<<<`, `=======`, dan `>>>>>>>`.
   - Klik *Mark as resolved*, lalu *Commit merge*, lalu *Merge pull request*.
4. **Latihan.** Kerjakan [Issue #4](https://github.com/DevinRafa/github-collab-demo/issues/4) dari awal: buat branch `fix/login-error`, perbaiki bug, push, buat PR dengan `Closes #4`.

## Alur kerja tim

GitHub Issue → Create Branch → Work on Task → Commit → Push Branch → Pull Request → Code Review → Request Changes / Approve → Merge → Delete Branch

## Penamaan branch

| Contoh yang baik | Hindari |
|---|---|
| `feature/homepage` | `branch1` |
| `feature/navbar` | `coba` |
| `feature/contact` | `baru` |
| `fix/login-error` | `test` |
| `fix/navbar-mobile` | `punya-saya` |

Nama branch harus menggambarkan pekerjaan yang sedang dilakukan.

## Isi file

- `index.html`: homepage (hasil PR #6)
- `login.html`: halaman login dengan **bug yang sengaja ditanam** untuk Issue #4
- `components/navbar.html`: ada di branch `feature/navbar` (PR #7)
- `contact.html`: ada di branch `feature/contact` (PR #8)
