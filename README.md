# 1. Membuat sebuah database dengan nama latihan2!
   
    create database latihan2;
   ![Screenshot (115)](https://user-images.githubusercontent.com/129852622/230273473-4c711d55-e9de-44f0-b8b0-d92781b8d038.png)

# 2. Membuat sebuah table dengan nama biodata (nama,alamat) didalam database latihan2!

    create table biodata (nama varchar(100), alamat text);
  ![Screenshot (116)](https://user-images.githubusercontent.com/129852622/230274512-9bcd1d2c-c345-468a-bd80-91fa538fbab0.png)

# 3. Menambahkan sebuah kolom keterangan (varchar 15),sebagai kolom terakhir!

    alter table biodata add column keterangan varchar (15);
  ![Screenshot (117)](https://user-images.githubusercontent.com/129852622/230275159-d6d0319a-5275-4218-b1c3-92dc16309778.png)

# 4. Menambahkan kolom id (int 11) di awal sebagai kolom pertama!

    alter table biodata add column id int (11) first;
  ![Screenshot (118)](https://user-images.githubusercontent.com/129852622/230275693-4b04235c-d4ea-4cee-9c8f-6e1401740022.png)

# 5. Menyisipkan sebuah kolom dengan nama phone (varchar 15) setelah kolom alamat!

    alter table biodata add column phone varchar (15) after alamat;
  ![Screenshot (119)](https://user-images.githubusercontent.com/129852622/230276184-d88d3ebc-a5c4-4126-b8f4-e6b5ce76c124.png)

# 6. Mengubah tipe data kolom id menjadi char (11)!

    alter table biodata modify column id varchar (11);
  ![Screenshot (120)](https://user-images.githubusercontent.com/129852622/230278271-b2b36550-620b-4e7b-8c48-7642469b4b52.png)
  
# 7. Mengubah nama kolom phone menjadi hp (varchar 20)!

    alter table biodata change phone hp varchar (20);
  ![Screenshot (121)](https://user-images.githubusercontent.com/129852622/230279007-28ec51db-ea67-4327-bb90-b8115787e02b.png)

# 8. Menambahkan kolom email setelah kolom hp!

    alter table biodata add column email after hp;
  ![Screenshot (122)](https://user-images.githubusercontent.com/129852622/230279373-78a9795a-b0d5-41c6-bcbb-94f1242c783b.png)

# 9. Menghapus kolom keterangan dari tabel!

    alter table biodata drop column keterangan;
  ![Screenshot (123)](https://user-images.githubusercontent.com/129852622/230279607-e7d4c8ce-e8ed-49a9-b266-c45c47efc67c.png)
  
# 10. Mengganti nama tabel menjadi data_mahasiswa!

    alter table biodata rename to data_mahasiswa;
  ![Screenshot (124)](https://user-images.githubusercontent.com/129852622/230282806-839072d5-45dd-4c6e-aa29-a894591c4ec1.png)

# 11. Mengganti nama field id menjadi nim!

    alter table data_mahasiswa change id nim varchar (20);
  ![Screenshot (125)](https://user-images.githubusercontent.com/129852622/230283219-efb592db-b381-4f0d-93cc-dffbb04e2bbd.png)

# 12. Menjadikan nim sebagai PRIMARY KEY!

    alter table data_mahasiswa add primary key (nim);
  ![Screenshot (126)](https://user-images.githubusercontent.com/129852622/230283564-6f6e93e0-56e7-4486-af51-ce329844b8ce.png)

# 13. Menjadikan kolom email sebagai UNIQUE KEY!

    alter table data_mahasiswa modifiy column email varchar (40);
    alter table data_mahasiswa add constraint unique_email unique (email);
  ![Screenshot (127)](https://user-images.githubusercontent.com/129852622/230284057-9c9ec289-1745-4bba-8713-0abf7c2dc07b.png)
  
