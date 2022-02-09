# Langkah kesembilan - Konfigurasi samba


- menambahkan user dan password samba dengan memasukkan perintah
    ```shell
    smbpasswd -a user1
    ```
    akan diminta password untuk samba sebanyak 2 kali

    ```shell
    New SMB password:
    Retype new SMB password:
    ```
---
- Buat folder baru di /home
    ```shell
    mkdir /home/bolehedit /home/hanyalihat
    ```
    > nama folder bisa di sesuaikan
- Ubah permission pada folder baru
    ```shell
    chmod -R 777 /home/bolehedit/
    chmod -R 777 /home/hanyalihat/
    ```
- Masuk ke file konfigurasi samba
    ```shell
    nano /etc/samba/smb.conf
    ```
- ketikkan konfigurasi file sharing
    ```shell
    [bolehedit]
    comment = folder yang boleh diedit
    path = /home/bolehedit
    browsable = yes
    writeable = yes
    write list = user1, user2, user3

    [hanyalihat]
    comment = folder yang tidak bisa diedit
    path = /home/hanyalihat
    browsable = yes
    readonly = yes
    ```

    - kemudian save dengan cara menekan tombol `CTRL`+`O`, kemudian tekan `ENTER`

    - kemudian exit dengan cara menekan tombol `CTRL`+`X`

- Restart samba dengan cara
    ```shell
    systemctl restart smdb
    ```
