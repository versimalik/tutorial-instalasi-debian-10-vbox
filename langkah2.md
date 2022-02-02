# Langkah Kedua - Setting pada virtual machine

1. Pilih virtual machine dan klik tombol settings

    ![setting pada virtual machine](https://drive.google.com/uc?export=view&id=15qOJq0abmlxPFHgceGD9XXCyDD9BX6E4)

2. Pada menu System:
    
    - uncheck Floppy
    - ubah urutan boot order menjadi optical paling atas, kemudian harddisk berada di bawahnya

    ![uncheck floppy dan ubah boot order](https://drive.google.com/uc?export=view&id=1nOHw22PR0GoGDcbxXnOZ80PrccutHNRa)

3. Pada menu Storage:

    - Pilih tulisan Empty di bawah Controller: IDE
    - Pilih gambar cd di pojok kanan
    - cari file ISO Debian 10 32 bit

    ![cari dan pilih file iso debian](https://drive.google.com/uc?export=view&id=1Z9wKqnKHejRdS2haeNkZHLtMOuYm2OS6)

    Sehingga menjadi seperti ini, jika file iso debian sudah terpilih

    ![file iso debian terpilih](https://drive.google.com/uc?export=view&id=1CkIW33NXzNg-UB8qGnRNpQTMR1ZFCddb)

4. Pada menu Network:
    
    - Attached to : Host-only Adapter
    - Name : Nama adapter host-only

    > Note: pada OS Windows, nama host-only adapter biasanya `Virtualbox Host-Only Adapter`

    ![network pada virtual machone](https://drive.google.com/uc?export=view&id=1fkXH2Jc2EACUkZAodHZq_TVLWsvjgfwO)

Jika sudah sesuai, tekan tombol OK.

Sampai tahap ini, virtual machine sudah siap untuk dijalankan

## [Lanjut ke langkah ketiga - menjalankan virtual machine dan melakukan instalasi Debian 10](/langkah3.md)