# Tugas_2-Student-CRUD-App

Tambah Data Student
![Screenshot 2022-03-21 194431 (1)](https://user-images.githubusercontent.com/101171434/159270061-86a93428-49f2-4c58-ba84-f10e88d49dcb.jpg)

curl --location --request POST 'localhost:8080/api/students' \
--header 'Content-Type: application/json' \
--data-raw '{
    "firstName" : "Putri",
    "lastName": "Fuji",
    "email": "Putrifj@gmail.com",
    "phoneNumber": "+628132167891"
}'


Menampilkan Semua Data Student
![Screenshot 2022-03-21 195025 (2)](https://user-images.githubusercontent.com/101171434/159270782-bdf9a1fb-7b4a-4153-ad67-f3119a7064c4.jpg)

curl --location --request GET 'localhost:8080/api/students'


Update Data Student
![Screenshot 2022-03-21 195225 (3)](https://user-images.githubusercontent.com/101171434/159270997-a407b051-6397-4408-a0ce-86f65e5ff528.jpg)

curl --location --request PUT 'localhost:8080/api/students/1' \
--header 'Content-Type: application/json' \
--data-raw '{
    "firstName" : "putra",
    "lastName": "zhafar",
    "email": "putra@gmail.com",
    "phone": "+6281321411511"
}'



Hapus Data Student
![Screenshot 2022-03-21 195310 (4)](https://user-images.githubusercontent.com/101171434/159271441-1c2895da-be5d-435a-9ecb-2dc8f19267af.jpg)

curl --location --request DELETE 'localhost:8080/api/students/4'



Mencari Salah Satu Data Student
![Screenshot 2022-03-21 203354 (5)](https://user-images.githubusercontent.com/101171434/159271980-0eb18748-981b-4e21-85b1-58affaf1a8f7.jpg)

curl --location --request GET 'localhost:8080/api/students/4'
