# pinepass todo

Todo Lits Pinepass Project And Cofiguration

## init section

- [x] Make Init System
- [x] Make System Can Auto Setup For Easy Configuration
- [x] init `{exampleInputName}.config.pinepass.json`
- [x] init `.env` and setup env

## Configuration

>[!NOTE]
>This Section Support `CRUD` method

- [x] config `.env`
- [ ] config `{exampleInputName}.config.pinepass.json`
- [ ] config System{
        - [ ] configToken
        - [ ] configGetToken
        - [ ] configTestToken
        - [ ] convigVerifiedToken
        }
- [ ] config gh org acount

## Login to gh

- [ ] loginTest
- [ ] loginVerif
- [ ] TestReadJsonEncrypt

## function/

- [x] init
- [x] .env
- [ ] config
- [ ] pharaphase
- [ ] import
- [ ] executeRuner
- [ ] connetAllToMAin

---

- [ ] encryptMethod
- [ ] decryptMethod
- [ ] ReadFormRawGithubMethod
- [ ] printoTerminal
- [ ] debug
- [ ] savety save
- [ ] GenerateFernetKey

## CRUD SYSTEM TO ALL `FUNCTION APPS`

- [ ] crudSystemAdd
- [x] version
- [x] lic
- [x] documentation
- [x] issue
- [x] report
- [x] contacUs


## 🛡️ Sistem Keamanan Pinepass

### 📁 Obfuscation & Proteksi Kode

- [ ] 🔐 PyArmor Full Obfuscation
  - [ ] Obfuscate semua file `.py` di `pinepasspy/`
  - [ ] Gunakan mode `--advanced 2` atau `--wrap-mode 1`
  - [ ] Sertakan binding ke hardware/expired key (optional)

- [ ] 🔒 Enkripsi Environment & Konfigurasi
  - [ ] Simpan `username`, `token`, dan key penting di `.env`
  - [ ] Encrypt file `.json` init menggunakan `fernet` + key dari `.env`
  - [ ] Hindari hardcode di dalam source code

### 🧾 Signature & Validasi Distribusi

- [ ] 🔐 SHA256 Checksum untuk .whl dan .tar.gz
  - [ ] Buat file `.sha256` untuk setiap file distribusi
  - [ ] Validasi file saat diinstal/dijalankan

- [ ] 🖊️ GPG Sign (PGP) untuk Validasi Asli
  - [ ] Buat file `.asc` signature untuk .whl / .tar.gz
  - [ ] Upload GPG Public Key ke GitHub / Docsify

- [ ] 🧬 Watermark dalam Kode
  - [ ] Sisipkan watermark dengan nama `pinepass.id` di bagian obfuscated
  - [ ] Pastikan watermark tidak bisa dihapus tanpa merusak file
  - [ ] Cek watermark saat runtime sebagai anti-tamper

### 📦 Keamanan Distribusi via PyPI / GitHub

- [ ] 🚧 Proteksi setup.py dan metadata
  - [ ] Hilangkan komentar penting
  - [ ] Rename field sensitif

- [ ] ⛔ Blok import `__main__` palsu
  - [ ] Cek keaslian file dengan SHA256 atau checksum

- [ ] 🔎 Monitoring Manual
  - [ ] Cek file `.whl`/`.tar.gz` di PyPI/GitHub apakah diubah
  - [ ] Bandingkan signature GPG dan SHA256

