# TUTORIAL INSTALASI DEBIAN 10 32 BIT DI VIRTUAL BOX

## Yang dibutuhkan
1. Aplikasi Oracle VM Virtual Box
2. File ISO Debian versi 10
    - debian-10.11.0-i386-netinst.iso untuk instalasi awal
    - debian-10.11.0-i386-DVD-1.iso untuk update repository list
    - debian-10.11.0-i386-DVD-2.iso untuk update repository list
    - debian-10.11.0-i386-DVD-3.iso untuk update repository list

    > DVD debian dibutuhkan untuk intalasi package  secara offline (__tanpa jaringan internet__)

> Note: untuk instalasi yang lebih cepat disarankan untuk __tidak terhubung koneksi internet atau jaringan lainnya__.

# Langkah Pertama - Membuat virtual machine baru di Virtual Box

1. Klik tombol "New"
    
    ![tombol new pada virtual box](https://drive.google.com/uc?export=view&id=1slEGxNmd-7mCJUJ0kvncQrcZsWjPeBzQ)

2. Isi nama, tipe dan versi menjadi

    - Name: debian_xyz
    - Type: Linux
    - Version: Debian (32-bit)

    > Nore: sesuaikan dengan kebutuhan

    ![menentukan nama virtual machine](https://drive.google.com/uc?export=view&id=1_HxfNL8xcgBVjqJidUDRZ1zFqvnUOr6i)

    Kemudian klik Next

3. Ubah memory size menjadi 1024 MB, atau jangan sampai melewati batas kuning apalagi merah, sesuaikan dengan kebutuhan

    ![memory size untuk virtual machine](https://drive.google.com/uc?export=view&id=1ncHZVgjWB3CSvzm88cXFlE8Q371qBaUk)

    Klik Next

4. Pilih Create a new Partition

     ![pilih Create a new partition](https://drive.google.com/uc?export=view&id=12fpqR9aVz02t1h_tujbSNwyL3R6W98Ks)
    
    Klik Create

5. Pilih Virtual Hard Disk

    ![pilih Virtual Hard Disk](https://drive.google.com/uc?export=view&id=1RHpg7RdkqUHj0qQZDyOUgASEo8ce9Xrh)

    Klik Next

6. Pilih Dinamically allocated

    ![Pilih Dinamically allocated](https://drive.google.com/uc?export=view&id=1-32fimxQ32h-gSr6f2BK3-7BpTTL8b3s)

    Klik Next

7. File Location and size, 8,00 GB
    
     ![File size 8,00 GB](https://drive.google.com/uc?export=view&id=1kD7hQPwf21YXq15ZNcWhddJ49Jgjr888)

    Klik Create

Sampai disini, pembuatan virtual machine baru sudah selesai

## [Lanjut ke langkah kedua - Setting pada virtual machine dan melakukan instalasi](/langkah2.md)
    


