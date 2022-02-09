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

    - kemudian save dengan cara menekan tombol `CTRL`+`O`

    - kemudian exit dengan cara menekan tombol `CTRL`+`X`

- Restart networking dengan cara
    ```shell
    systemctl restart networking
    ```

- cek IP address dengan cara
    ```shell
    ip a
    ```

sampai tahap ini IP sudah tersetting

