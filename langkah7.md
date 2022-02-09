# Langkah ketujuh - Update repo list dari DVD dan instalasi package

- Masukkan DVD 1 dengan cara:
    ```shell
    apt-cdrom add
    ```

    akan muncul perintah

    ```shell
    Please insert a Disc in the drive an press [Enter]
    ```

    - masukkan dvd ke virtual machine, klik kanan pada icon cd di bagian bawah

        ![Masukkan DVD](https://drive.google.com/uc?export=view&id=1ONxpaPSXbtoZjuIr036tmTEphVHAHQ70)

    - pilih DVD 1    
        ![Masukkan DVD 1](https://drive.google.com/uc?export=view&id=1OuzzwfF3FG_QjtOhT_sXWcAqkFEBkX9_)

    - setelah terpilih, tekan `ENTER`

- Lakukan langkah yang sama untuk DVD 2 dan 3

- Tambahkan 1 repo list untuk instalasi cacti, ketikkan perintah berikut

    ```shell
    nano /etc/apt/sources.list
    ```

    masukkan link ini di baris paling bawah

    ```nano
    deb http://ftp.de.debian.org/debian buster main
    ```

    seperti pada gambar

     ![Repo list](https://drive.google.com/uc?export=view&id=10GZEjT-GfZ14o77yUHgjnP7A9KasLKTb)


    - kemudian save dengan cara menekan tombol `CTRL`+`O`, kemudian tekan `ENTER`

    - kemudian exit dengan cara menekan tombol `CTRL`+`X`

- sementara gunakan koneksi internet untuk instalasi. Ubah network pada virtual machine menjadi NAT

    ![Network NAT](https://drive.google.com/uc?export=view&id=1TYr0E3P4jF-zTXurEJdBU-iv7yzx2xzb)

    dan `RUBAH SEMENTARA` IP address pada debian menjadi DHCP serta tambahkan tanda `#` pada baris address, netmask dan gateway

    ```nano
    auto enp0s3
    iface enp0s3 inet dhcp
    #    address 10.30.30.5
    #    netmask 255.255.255.128
    #    gateway 10.30.30.1
    ```

    - kemudian save dengan cara menekan tombol `CTRL`+`O`, kemudian tekan `ENTER`

    - kemudian exit dengan cara menekan tombol `CTRL`+`X`

- Restart networking dengan cara
    ```shell
    systemctl restart networking
    ```

> Pastikan PC HOST atau windows memiliki koneksi internet

## Lakukan instalasi package

- masukkan perintah ini untuk update repo dan langsung install package

    ```shell
    apt update && apt install php apache2 mariadb-server mariadb-client cacti samba clamav -y 
    ```

- jika diminta memasukkan DVD, lakukan cara yang sama seperti pada langkah 6

    ![Masukkan DVD](https://drive.google.com/uc?export=view&id=1ONxpaPSXbtoZjuIr036tmTEphVHAHQ70)

    pilih DVD sesuai yang diminta
      
    ![Masukkan DVD 1](https://drive.google.com/uc?export=view&id=1OuzzwfF3FG_QjtOhT_sXWcAqkFEBkX9_)

    kemudian tekan `ENTER`

- lakukan hal yang sama jika diminta DVD lain lagi

- tunggu sampai instalasi selesai

