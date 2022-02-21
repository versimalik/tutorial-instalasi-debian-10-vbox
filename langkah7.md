# Langkah ketujuh - Update repo list dari DVD dan instalasi package

- Masukkan DVD 1 dengan cara klik kanan pada icon cd di bagian bawah

    ![Masukkan DVD](https://drive.google.com/uc?export=view&id=1ONxpaPSXbtoZjuIr036tmTEphVHAHQ70)

- pilih DVD 1    
    ![Masukkan DVD 1](https://drive.google.com/uc?export=view&id=1OuzzwfF3FG_QjtOhT_sXWcAqkFEBkX9_)

- Kemudian ketikkan perintah ini

    ```shell
    apt-cdrom add
    ```
- Lakukan langkah yang sama untuk DVD 2 dan 3

## Lakukan instalasi package

- masukkan perintah ini untuk update repo dan langsung install package

    ```shell
    apt update 
    ```
    jika sudah selesai, kemudian

    ```shell
    apt install php apache2 mariadb-server mariadb-client samba clamav -y 
    ```

- jika diminta memasukkan DVD, lakukan cara yang sama seperti pada langkah 6

    ![Masukkan DVD](https://drive.google.com/uc?export=view&id=1ONxpaPSXbtoZjuIr036tmTEphVHAHQ70)

    pilih DVD sesuai yang diminta
      
    ![Masukkan DVD 1](https://drive.google.com/uc?export=view&id=1OuzzwfF3FG_QjtOhT_sXWcAqkFEBkX9_)

    kemudian tekan `ENTER`

- lakukan hal yang sama jika diminta DVD lain lagi

- tunggu sampai instalasi selesai

## [Lanjut ke langkah kedelapan - Menambahkan user pada system](langkah8.md)

