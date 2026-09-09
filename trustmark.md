# 🏥 Trust Mark BPJS Kesehatan — Self Assessment & Preparation Checklist

[![BPJS Kesehatan](https://img.shields.io/badge/BPJS%20Kesehatan-Trust%20Mark%20Verified-green?style=for-the-badge&logo=shield)](https://trustmark.bpjs-kesehatan.go.id)
[![Compliance Status](https://img.shields.io/badge/ISO--27001%20%7C%20ISO--20000-Compliant-blue?style=for-the-badge)](https://trustmark.bpjs-kesehatan.go.id)
[![Hospital](https://img.shields.io/badge/Faskes-RSU%20Indriati%20Boyolali-emerald?style=for-the-badge)](https://trustmark.bpjs-kesehatan.go.id)

Dokumen ini berisi **Panduan Ringkasan, Breakdown 234 Pertanyaan / Indikator**, serta **Checklist Berkas Audit (SK, SOP, Bukti Fisik, & Screenshot)** yang siap digunakan sebagai acuan kerja tim IT, HRD, Legal, Rekam Medis, dan IPSRS **RSU INDRIATI BOYOLALI** dalam memenuhi penilaian *Self Assessment Trust Mark BPJS Kesehatan*.

---

## 📑 Daftar Isi
- [📌 Ringkasan Domain Penilaian](#-ringkasan-domain-penilaian)
- [🛡️ Domain 1: Keamanan Informasi (168 Indikator)](#️-domain-1-keamanan-informasi-168-indikator)
- [⚙️ Domain 2: Manajemen Layanan (42 Indikator)](#️-domain-2-manajemen-layanan-42-indikator)
- [💻 Domain 3: Standar Teknis & Cons-ID (24 Indikator)](#-domain-3-standar-teknis--cons-id-24-indikator)
- [📋 GitHub Checklist Berkas & Bukti Pembuktian Audit](#-github-checklist-berkas--bukti-pembuktian-audit)

---

## 📌 Ringkasan Domain Penilaian

| No | Kategori Utama | Jumlah Indikator | Acuan Standard / Framework | Status Kesiapan |
|:---:|---|:---:|---|:---:|
| **1** | **Keamanan Informasi** | **168 Pertanyaan** | ISO/IEC 27001 & UU PDP | `[ ] Pending Upload` |
| **2** | **Manajemen Layanan** | **42 Pertanyaan** | ISO/IEC 20000 & ITIL Service Management | `[ ] Pending Upload` |
| **3** | **Standar Teknis & API** | **24 Pertanyaan** | BPJS Security Standard, Database Hardening, Cons-ID | `[ ] Pending Upload` |

---

## 🛡️ Domain 1: Keamanan Informasi (168 Indikator)

<details>
<summary><b>🔍 Klik untuk membuka rincian kelompok pertanyaan Domain Keamanan Informasi</b></summary>

> [!NOTE]
> Menilai tingkat kematangan kerahasiaan (*Confidentiality*), keutuhan (*Integrity*), dan ketersediaan (*Availability*) data kesehatan pasien BPJS.

1. **Kontrol Personil (No. 1 - 29):**
   - Aturan *Remote Working* (penggunaan VPN SSL/IPsec terenkripsi).
   - Klausul Kerahasiaan Data Pasien pada Kontrak Kerja (PKWT/PKWTT).
   - Prosedur *Exit Clearance* & pencabutan akun SIMRS/VClaim harian saat pegawai resign/mutasi.
   - Pelatihan *Security Awareness* wajib tahunan untuk seluruh karyawan.
   - Penandatanganan Non-Disclosure Agreement (NDA) untuk karyawan & seluruh vendor IT.
   - Peraturan Disiplin Pegawai & Sanksi Pelanggaran IT.
   - *Background Check* (pemeriksaan SKCK & verifikasi ijazah) calon karyawan.
2. **Kontrol Teknologi (No. 30 - 81):**
   - Antivirus terpusat (100% protected status).
   - *Data Masking* (penyembunyian NIK `3309**************` & No. BPJS pada interface SIMRS).
   - *Data Leakage Prevention (DLP)* & pemblokiran USB Drive di PC Kasir/Pendaftaran.
   - Segregasi Jaringan Komputer (VLAN WiFi Tamu vs Jaringan SIMRS RS).
   - Larangan penggunaan database produksi untuk testing (wajib data dummy).
   - Pemindaian celah siber rutin (*Vulnerability Assessment / PenTest*).
   - Enkripsi data transit (SSL/TLS HTTPS A+ Labs Score).
   - Pembatasan Hak Akses berbasis Peran (Role-Based Access Control / RBAC).
   - *Secure Coding Standard* (OWASP Top 10).
   - Pencadangan Data (*Backup*) otomatis & Uji Pemulihan Data (*Restore Test*).
   - *Web Filtering* pemblokiran judi/pornografi pada router firewall.
3. **Kontrol Fisik `[Check Fisik]` (No. 82 - 111):**
   - *Door Access Control* (Fingerprint/Card Reader) Ruang Server.
   - Kerapihan Cable Tray, Server Rack Enclosure, & Labeling Kabel Patch Cord.
   - Suhu Ruang Server (18°C – 22°C), Thermometer, Hygrometer, & APAR CO2/Clean Agent.
   - UPS Online Centralized & CCTV 24 Jam dengan retensi rekaman.
4. **HAKI & Lisensi (No. 112 - 120):**
   - Legalitas lisensi OS Windows Server, Database, & Aplikasi SIMRS.
5. **Organisasi Keamanan Informasi (No. 121 - 168):**
   - SK Kebijakan Keamanan Informasi & Penunjukan Penanggung Jawab Keamanan Data/CISO.
   - Kontak Pelaporan Insiden Siber ke BSSN / CSIRT Kesehatan / Kepolisian.
   - Manajemen Risiko IT Proyek Baru & Pelabelan Dokumen "RAHASIA".

</details>

---

## ⚙️ Domain 2: Manajemen Layanan (42 Indikator)

<details>
<summary><b>🔍 Klik untuk membuka rincian kelompok pertanyaan Domain Manajemen Layanan</b></summary>

> [!NOTE]
> Menilai tata kelola operasional IT RS dalam memenuhi SLA (Service Level Agreement) pelayanan pasien.

1. **Portofolio & Katalog Layanan TI (No. 169 - 183):**
   - Publikasi Katalog Layanan TI & SLA penanganan kendala IT (misal max 15 menit).
   - Penggunaan aplikasi *Helpdesk Ticketing System* untuk mencatat & melacak laporan perawat/dokter.
2. **Pengendalian Pihak Ketiga & Vendor (No. 184 - 188):**
   - Daftar vendor IT (ISP Internet, Vendor SIMRS, Vendor Genset) & Perjanjian Kerjasama (PKS SLA).
   - Laporan Evaluasi Kinerja Vendor Tahunan.
3. **Konfigurasi & Change Management (No. 189 - 206):**
   - *Configuration Management Database (CMDB)* inventaris aset IT & Change Log Server.
   - Prosedur pengajuan update SIMRS menggunakan form *Request for Change (RFC)* & staging test.
   - Grafik pemantauan kapasitas Storage/RAM/CPU Server (Zabbix/PRTG).
4. **Keberlangsungan Bisnis / DRP (No. 207 - 210):**
   - Dokumen *Disaster Recovery Plan (DRP)* & *Business Continuity Plan (BCP)*.
   - SOP Pelayanan Pasien Manual (Kertas) saat SIMRS down total.

</details>

---

## 💻 Domain 3: Standar Teknis & Cons-ID (24 Indikator)

<details>
<summary><b>🔍 Klik untuk membuka rincian kelompok pertanyaan Domain Standar Teknis</b></summary>

> [!WARNING]
> Memerlukan pengunggahan bukti teknis konkret (`[Check Fisik]`) dan konfigurasi pengamanan API BPJS.

1. **Keamanan Database `[Check Fisik]` (No. 211 - 213):**
   - Hardening Database (nonaktifkan user root publik, ubah port default, aktifkan audit log SQL).
   - Berita Acara Uji Pemulihan Database (*Restore Test Report*).
2. **Keamanan Server `[Check Fisik]` (No. 214 - 216):**
   - Matikan service SSH/RDP publik, disable USB port server, dan log update patching OS.
3. **Jaringan & Firewall Rules `[Check Fisik]` (No. 217 - 224):**
   - Segmentasi VLAN, otentikasi WiFi Karyawan, dan Whitelisting IP Address Endpoint BPJS Kesehatan pada Firewall.
4. **Pengamanan Cons-ID BPJS `[Check Fisik]` (No. 225 - 229):**
   - 🔒 **Aturan Wajib:** Consumer ID & Secret Key API BPJS **DILARANG HARDCODED** di frontend JavaScript/HTML. Wajib disimpan di file `.env` / backend terenkripsi.
5. **Prasarana Data Center `[Check Fisik]` (No. 230 - 234):**
   - Pemeliharaan rutin Genset RS, UPS Centralized, dan Panel Listrik ATS/AMF oleh IPSRS.

</details>

---

## 📋 GitHub Checklist Berkas & Bukti Pembuktian Audit

> [!TIP]
> Gunakan checkbox di bawah ini untuk melacak status persiapan dokumen tim RS.

### 1. SK Direksi & Kebijakan Tertulis
- [ ] **SK-01:** SK Direksi tentang Kebijakan Keamanan Informasi RS & Perlindungan Data Pribadi.
- [ ] **SK-02:** SK Struktur Organisasi IT & Penunjukan Penanggung Jawab Keamanan Data (CISO/PIC Security).
- [ ] **SK-03:** SK Peraturan Disiplin Pegawai & Sanksi Pelanggaran Keamanan IT.
- [ ] **SK-04:** Kebijakan Penggunaan Aset IT (*Acceptable Use Policy*) & Larangan Software Bajakan.
- [ ] **SK-05:** Kebijakan Kriptografi, Enkripsi Data, & SSL Protocol.

---

### 2. Standard Operating Procedure (SOP) Teknis
- [ ] **SOP-01:** `SOP_Akses_Jarak_Jauh_Remote_VPN.pdf`
- [ ] **SOP-02:** `SOP_Mutasi_dan_Exit_Clearance_Pegawai.pdf`
- [ ] **SOP-03:** `SOP_Non_Disclosure_Agreement_NDA.pdf`
- [ ] **SOP-04:** `SOP_Rekrutmen_dan_Background_Check_Pegawai.pdf`
- [ ] **SOP-05:** `SOP_Update_Antivirus_dan_Patching_OS.pdf`
- [ ] **SOP-06:** `SOP_Pencegahan_Kebocoran_Data_DLP.pdf`
- [ ] **SOP-07:** `SOP_Manajemen_Hak_Akses_User_SIMRS.pdf`
- [ ] **SOP-08:** `SOP_Backup_dan_Recovery_Database.pdf`
- [ ] **SOP-09:** `SOP_Secure_Coding_dan_Pengamanan_API_BPJS.pdf`
- [ ] **SOP-10:** `SOP_Pengamanan_Fisik_Ruang_Server.pdf`
- [ ] **SOP-11:** `SOP_Pelaporan_Insiden_Siber_CSIRT.pdf`
- [ ] **SOP-12:** `SOP_Klasifikasi_dan_Pelabelan_Dokumen.pdf`
- [ ] **SOP-13:** `SOP_Helpdesk_Ticketing_dan_SLA_IT.pdf`
- [ ] **SOP-14:** `SOP_Request_for_Change_RFC.pdf`
- [ ] **SOP-15:** `SOP_Pelayanan_Manual_Saat_SIMRS_Down_BCP.pdf`
- [ ] **SOP-16:** `SOP_Hardening_Server_dan_Database.pdf`
- [ ] **SOP-17:** `SOP_Pemeliharaan_Genset_dan_UPS_IPSRS.pdf`

---

### 3. Formulir, Logbook & Berita Acara
- [ ] **FORM-01:** Draf Kontrak Kerja Pegawai (memuat pasal kerahasiaan data).
- [ ] **FORM-02:** Sampel Form Exit Clearance Pegawai Terisi & Deaktivasi Akun.
- [ ] **FORM-03:** Perjanjian Kerahasiaan (NDA) Vendor SIMRS/Network Bermaterai.
- [ ] **FORM-04:** Absensi & Slide Materi Edukasi Keamanan Informasi Tahunan.
- [ ] **FORM-05:** Berita Acara Uji Pemulihan Database (*Restore Test Report*).
- [ ] **FORM-06:** Form Request for Change (RFC) Update SIMRS Terisi.
- [ ] **FORM-07:** Logbook Fisik Pengunjung Ruang Server.
- [ ] **FORM-08:** Matrix Hak Akses User SIMRS (*Role-Based Access Control*).
- [ ] **FORM-09:** Tabel Inventaris Aset Hardware IT & Lisensi Software.
- [ ] **FORM-10:** Dokumen Publikasi Katalog Layanan TI & SLA RS.
- [ ] **FORM-11:** Laporan Evaluasi Kinerja Vendor Tahunan (ISP & SIMRS).
- [ ] **FORM-12:** Checklist Maintenance Bulanan Genset & UPS oleh IPSRS.

---

### 4. Bukti Foto Fisik Data Center `[Check Fisik]`
- [ ] **FOTO-01:** Foto Pintu Ruang Server terpasang *Door Access Control* & Signage Terbatas.
- [ ] **FOTO-02:** Foto Kerapihan Kabel LAN, *Cable Tray*, & Labeling Patch Cord di Server Rack.
- [ ] **FOTO-03:** Foto Thermometer / Display AC Presisi Ruang Server (Suhu **18°C – 22°C**).
- [ ] **FOTO-04:** Foto APAR Gas khusus (*Clean Agent / CO2 / FM200*) Ruang Server.
- [ ] **FOTO-05:** Foto Perangkat UPS Online Centralized Penopang Server.
- [ ] **FOTO-06:** Foto Kamera CCTV yang Mengawasi Ruang Server.
- [ ] **FOTO-07:** Foto Genset RS & Panel Otomatis ATS/AMF.

---

### 5. Bukti Digital & Screenshot Sistem
- [ ] **SS-01:** Screenshot Dashboard Central Antivirus (100% Protected Status).
- [ ] **SS-02:** Screenshot Tampilan Data Masking SIMRS (Sensor NIK `3309**************`).
- [ ] **SS-03:** Screenshot Konfigurasi GPO / USB Drive Blocking.
- [ ] **SS-04:** Skema Topologi Jaringan RS & Screenshot Config VLAN Router Firewall.
- [ ] **SS-05:** Screenshot Detail Sertifikat SSL/TLS Website RS (HTTPS).
- [ ] **SS-06:** Screenshot Dashboard Web Filter Router (Blokir Judi & Pornografi).
- [ ] **SS-07:** Screenshot Dashboard Aplikasi Helpdesk Ticketing IT.
- [ ] **SS-08:** Screenshot Graph Monitoring Kapasitas Server (Zabbix/PRTG).
- [ ] **SS-09:** Screenshot Terminal Log Update Patching OS Server.
- [ ] **SS-10:** Screenshot Rules Firewall Router (Whitelisting IP Address BPJS).
- [ ] **SS-11:** Snippet Code Backend Enkripsi `CONS_ID` & `SECRET_KEY` via `.env`.

---

## 🛠️ Pembagian Tugas Tim RS

| Tim / Unit Kerja | Tanggung Jawab Dokumen |
|---|---|
| **Tim IT & Developer SIMRS** | SOP Teknis IT, Screenshot Sistem, Snippet Code Cons-ID, Backup Restore Test, Config Router/VLAN. |
| **HRD & Legal RS** | SK Kebijakan, Kontrak Kerja Pegawai, Form Exit Clearance, NDA Vendor, SOP Rekrutmen. |
| **IPSRS & Teknisi Listrik** | Perawatan Genset, UPS Centralized, APAR, Suhu Ruang Server, & Form Maintenance Bulanan. |
| **Rekam Medis** | SOP Klasifikasi Dokumen Medis, Watermark Rahasia, SOP BCP Pelayanan Manual Kertas. |
