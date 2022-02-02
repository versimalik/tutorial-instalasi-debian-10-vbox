# Langkah keempat - Membagi harddisk menjadi 3 partisi

> Secara default, partisi harddisk pada debian dapat dibagi menjadi 3 partisi menjadi:
> 
> 1. partisi untuk / (root file system)
> 2. partisi untuk /home
> 3. partisi untuk swap area
>
> `root` dan `swap` merupakan partisi yang wajib ada

1. Partition method, pilih manual

    ![Partition method, manual](https://drive.google.com/uc?export=view&id=1e6wkpFLq-Fiv1GziLTXmcLldfKT8vWbI)

2. Pilih, ATA VBOX HARDDISK 

    ![Pilih, ATA VBOX HARDDISK](https://drive.google.com/uc?export=view&id=166W8XliEGpl8NoNeue0lx0D_X3ETQJTH)

3. Create new empty partition table on this device? Pilih Yes. 

    ![Pilih, ATA VBOX HARDDISK](https://drive.google.com/uc?export=view&id=1WfOAEDghLNGmaLPyAw48LMIUa9dI9FBB)

## Partisi untuk / (root file system)

1. Pilih `FREE SPACE`

    ![Pilih FREE SPACE](https://drive.google.com/uc?export=view&id=139ol__RwYMzIN2ZACG2MhgQrm6OrcaGa)

2. Pilih `Create a new partition` 

    ![Pilih Create a new partition](https://drive.google.com/uc?export=view&id=1VF-tveCm4X6T4SDYGFegwTf1l5Kllk5Q)

3. Ubah partisi menjadi 3 GB

    ![Ubah partisi menjadi 3 GB](https://drive.google.com/uc?export=view&id=1MLj70QxeACMok7djITkMRgV6cNZwx6YF)

4. Pilih `Primary`

    ![pilih primary](https://drive.google.com/uc?export=view&id=1faH7qxkG1c2JFH8MAtArbQUcpu4Vxl4H)


5. Pilih `Beginning`

    ![pilih beginning](https://drive.google.com/uc?export=view&id=1Ye5mu5D8B6-LPAPPnU9O5adSyM4VZIaD)

6. Pastikan:

    - Use as : Ext4 journaling file system
    - Mount point : /

    > Tekan tombol `ENTER` untuk memunculkan pilihan

    ![use as ext4, mount point /](https://drive.google.com/uc?export=view&id=1mltJh8afGwkgaHMfSOy2LuRJLEt0FcuM)

    jika sudah, pilih `Done setting up the partition`

## Partisi untuk /home

1. Pilih `FREE SPACE`

    ![Pilih FREE SPACE](https://drive.google.com/uc?export=view&id=1mj0kRIBJ_NQbVMaDSiBGFogogt7O4IGp)

2. Pilih Create a new partition 

    ![Pilih Create a new partition](https://drive.google.com/uc?export=view&id=1WfOAEDghLNGmaLPyAw48LMIUa9dI9FBB)

3. Ubah partisi menjadi 3 GB

    ![Ubah partisi menjadi 3 GB](https://drive.google.com/uc?export=view&id=1i3RaoCXvTvBVJxQlR2FWIk3flU5mLOu3)

4. Pilih primary

    ![pilih primary](https://drive.google.com/uc?export=view&id=1faH7qxkG1c2JFH8MAtArbQUcpu4Vxl4H)


5. Pilih Beginning

    ![pilih beginning](https://drive.google.com/uc?export=view&id=1Ye5mu5D8B6-LPAPPnU9O5adSyM4VZIaD)

6. Pastikan:

    - Use as : Ext4 journaling file system
    - Mount point : /home

    > Tekan tombol `ENTER` untuk memunculkan pilihan

    ![use as ext4, mount point /home](https://drive.google.com/uc?export=view&id=15SWtUSO9wkKuLqlvO67tpapkm4xUITxt)

    jika sudah, pilih `Done setting up the partition`

## Partisi untuk swap area

1. Pilih `FREE SPACE`

    ![Pilih FREE SPACE](https://drive.google.com/uc?export=view&id=1AZgJJavu5SZYoAv2NOPL3nc9oSzAwW72)

2. Pilih Create a new partition 

    ![Pilih Create a new partition](https://drive.google.com/uc?export=view&id=1WfOAEDghLNGmaLPyAw48LMIUa9dI9FBB)

3. Ubah partisi menjadi 2.6 GB

    ![Ubah partisi menjadi 2.6 GB](https://drive.google.com/uc?export=view&id=1dVe5r92tiaxNqfqQ2miEw15XUw9lJD3z)

4. Pilih primary

    ![pilih primary](https://drive.google.com/uc?export=view&id=1faH7qxkG1c2JFH8MAtArbQUcpu4Vxl4H)


5. Pastikan:

    - Use as : Swap area

    > Tekan tombol `ENTER` untuk memunculkan pilihan

    ![use as swap area](https://drive.google.com/uc?export=view&id=18iVYk3kh6qZsOuyK00FoQbdidYUmmbSt)

    jika sudah, pilih `Done setting up the partition`

---

Pastikan semua partisi sudah selesa dibuat

- Klik `Finish partitioning and write changes to disk`

    ![harddisk sudah terbagi menjadi 3 partisi](https://drive.google.com/uc?export=view&id=1Ef-eMXISblrvz5FHAGECRcZ5qDJX_cZS)

- `Write changes to disks?` Pilih `Yes`

    ![write changes to disks? yes](https://drive.google.com/uc?export=view&id=16At64EQJ_y8NxUT3rTuH9OgbNeDQUOqf)

Sampai disini proses partisi sudah selesai dan system akan melakukan `Installing base system`. Silahkan ditunggu sampai proses selesai.

![Installing base system](https://drive.google.com/uc?export=view&id=1znCgbEd4OXRDiMaqJZ275NVcssrjfdih)

## [Lanjut ke langkah kelima - Menyelesaikan instalasi](langkah5.md)

