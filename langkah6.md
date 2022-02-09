# Langkah keenam - Setting IP address pada debian 10

- Login ke OS debian menggunakan akun root
- masukkan perintah berikut
    ```shell
    nano /etc/network/interfaces
    ```
- masukkan setting IP untuk `enp0s3`, biasanya berada di baris paling bawah

    ```nano
    auto enp0s3
    iface enp0s3 inet static
        address 10.30.30.5
        netmask 255.255.255.128
        gateway 10.30.30.1
    ```

    > Setting IP address bisa disesusikan dengan kebutuhan

    - kemudian save dengan cara menekan tombol `CTRL`+`O`, kemudian tekan `ENTER`

    - kemudian exit dengan cara menekan tombol `CTRL`+`X`

- Restart networking dengan cara
    ```shell
    systemctl restart networking
    ```

- cek IP address dengan cara
    ```shell
    ip a
    ```

> sampai tahap ini IP sudah tersetting

- untuk menyambungkan ke PC host yang sudah terkoneksi dengan router, ubah network pada virtual machine menjadi bridged adapter

    ![Network ubah menjadi bridged adapter](https://drive.google.com/uc?export=view&id=1vmSFlCEFSo1yUb_RFcUCFfKWYgsAzpj-)

- silahkan ping IP debian menggunakan CMD dari PC


## [Lanjut ke langkah ketujuh - Update repo list dari DVD dan instalasi package](langkah7.md)