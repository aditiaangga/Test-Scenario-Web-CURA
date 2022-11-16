# Test-Scenario-Web-CURA
Test Scenario Website CURA Healthcare Service


| | | | | | | | | | | | | | | | | |
|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|
| | | | | | | | | | | | | | | | | |
| |Test Script Website https://katalon-demo-cura.herokuapp.com/ Fitur Appointment| | | | | | | | | | | | | | | |
| | | | | | | | | | | | | | | | | |
|Scenario ID|Case ID|Type|Test Case Description|Steps|Steps Description|Test Data|Expected Result|Actual Result|Log/Screenshot|Dates|Tester|Final Result|Notes|Version|Pre-condition|Post-condition|
|TS003.APMNT|TC.A001|POSITIVE|Pengguna membuka halaman Make Appointment via Click 'Make Appointment'|1|Pengguna berada di Halaman Home kondisi setelah Login| |Halaman Appointment Tersedia|as expected| |09/13/2022|Aditia|Passed| |Firefox 104.0.2  (64-bit)| | |
| | | | |2|Pengguna Klik Make Appointment| | | | | | | | | | | |
| | | | | | | | | | | | | | | | | |
| | | | | | | | | | | | | | | | | |
| |TC.A002|POSITIVE|Pengguna membuka halaman Make Appointment via Scroll|1|Pengguna berada di Halaman Home kondisi setelah Login| |Halaman Appointment Tersedia|as expected| |09/13/2022|Aditia|Passed| |Firefox 104.0.2  (64-bit)| | |
| | | | |2|Pengguna scroll menuju Halaman Make Appointment| | | | | | | | | | | |
| | | | | | | | | | | | | | | | | |
| | | | | | | | | | | | | | | | | |
| |TC.A003|POSITIVE|Pengguna melakukan Appointment dengan sukses kondisi semua field terisi|1|Pengguna berada di Halaman Appointment| |1. Appointment Berhasil 2. Masuk Ke Halaman Appointment Confirmation|as expected| |09/13/2022|Aditia|Passed| |Firefox 104.0.2  (64-bit)| | |
| | | | |2|Pengguna pilih Facility|Facility: 'Tokyo CURA Healthcare Center'| | | | | | | | | | |
| | | | |3|Pengguna ceklis Apply for hospital readmission| | | | | | | | | | | |
| | | | | | | | | | | | | | | | | |
| | | | |4|Pengguna pilih Healthcare Program|Healthcare Program: 'Medicare'| | | | | | | | | | |
| | | | |5|Pengguna memilih Visit Date|09/20/2022| | | | | | | | | | |
| | | | |6|Pengguna input Comment|Comment: 'Thank You'| | | | | | | | | | |
| | | | |7|Pengguna Klik 'Book Appointment'| | | | | | | | | | | |
| |TC.A004|POSITIVE|Pengguna melakukan Appointment dengan sukses kondisi hanya mengisi field yang bertanda required|1|Pengguna berada di Halaman Appointment| |1. Appointment Berhasil 2. Masuk Ke Halaman Appointment Confirmation|as expected| |09/13/2022|Aditia|Passed| |Firefox 104.0.2  (64-bit)| | |
| | | | |2|Pengguna tidak memilih Facility| | | | | | | | | | | |
| | | | |3|Pengguna tidak ceklis Apply for hospital readmission| | | | | | | | | | | |
| | | | | | | | | | | | | | | | | |
| | | | |4|Pengguna tidak memilih Healthcare Program| | | | | | | | | | | |
| | | | |5|Pengguna memilih Visit Date|09/22/2022| | | | | | | | | | |
| | | | |6|Pengguna tidak input Comment| | | | | | | | | | | |
| | | | |7|Pengguna Klik 'Book Appointment'| | | | | | | | | | | |
| |TC.A005|NEGATIVE|Pengguna melakukan Appointment dengan kondisi field tidak terisi|1|Pengguna berada di Halaman Appointment| |1. Appointment Gagal 2. Muncul Pop Up 'Please fill out this field'|as expected| |09/13/2022|Aditia|Passed| |Firefox 104.0.2  (64-bit)| | |
| | | | |2|Pengguna tidak memilih Facility| | | | | | | | | | | |
| | | | |3|Pengguna tidak ceklis Apply for hospital readmission| | | | | | | | | | | |
| | | | | | | | | | | | | | | | | |
| | | | |4|Pengguna tidak memilih Healthcare Program| | | | | | | | | | | |
| | | | |5|Pengguna tidak memilih Visit Date| | | | | | | | | | | |
| | | | |6|Pengguna tidak input Comment| | | | | | | | | | | |
| | | | |7|Pengguna Klik 'Book Appointment'| | | | | | | | | | | |
| |TC.A006|NEGATIVE|Pengguna melakukan Appointment dengan kondisi tanggal visit date sebelum hari ini|1|Pengguna berada di Halaman Appointment| |1. Appointment Gagal 2. Muncul Pop Up Error|is not expected| |09/13/2022|Aditia|Failed|1. Appointment Berhasil 2. Tidak Muncul Pop Up Error|Firefox 104.0.2  (64-bit)| | |
| | | | |2|Pengguna memilih Facility|Facility: 'Seoul CURA Healthcare Center'| | | | | | | | | | |
| | | | |3|Pengguna ceklis Apply for hospital readmission| | | | | | | | | | | |
| | | | | | | | | | | | | | | | | |
| | | | |4|Pengguna memilih Healthcare Program|Healthcare Program: 'Medicaid'| | | | | | | | | | |
| | | | |5|Pengguna memilih Visit Date sebelum hari ini|01/15/2022| | | | | | | | | | |
| | | | |6|Pengguna input Comment|Comment: 'Danke'| | | | | | | | | | |
| | | | |7|Pengguna Klik 'Book Appointment'| | | | | | | | | | | |
