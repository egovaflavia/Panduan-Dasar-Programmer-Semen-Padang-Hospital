# Struktur Git Branch

Gunakan branching model Git untuk memisahkan pengembangan dari produksi:

* `main`: Branch utama, siap dirilis.
* `develop`: Branch penggabungan fitur.
* `feature/xyz`: Untuk fitur baru.
* `bugfix/xyz`: Untuk perbaikan minor.
* `hotfix/xyz`: Patch cepat langsung dari `main`.

Semua perubahan harus melewati proses Pull Request dan code review.
