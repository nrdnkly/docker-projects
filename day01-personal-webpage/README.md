
# Day 01 – Personal Web Page with Docker

## 📌 Project Overview

Bu proje, Docker kullanarak basit bir statik web sayfasını Nginx container içinde çalıştırmayı amaçlamaktadır.
İlk Docker deneyimi olarak container çalıştırma, port mapping ve volume kullanımını öğrenmek hedeflenmiştir.



## 🎯 Objectives

* Docker ile ilk container'ı çalıştırmak
* Nginx kullanarak statik web sayfası yayınlamak
* Port mapping (`-p`) mantığını öğrenmek
* Volume mount (`-v`) kullanımı ile dosya bağlamak



## 🛠 Technologies Used

* Docker
* Nginx
* HTML



## 📁 Project Structure

```text
day01-personal-webpage/
├── index.html
└── README.md
```



## 🚀 How to Run

Proje klasöründe terminal aç ve şu komutu çalıştır:

```bash
docker run -d --name myweb -p 8080:80 -v $(pwd):/usr/share/nginx/html nginx
```


## 🌐 Access

Tarayıcıdan şu adrese git:

```
http://localhost:8080
```

## 📚 What I Learned

* Docker container nasıl çalıştırılır
* Nginx container kullanımı
* Port yönlendirme (port mapping)
* Volume mount ile dosya paylaşımı
* Container lifecycle yönetimi

## 📌 Outcome

Başarılı bir şekilde ilk Docker container’ımı çalıştırdım ve statik bir web sayfasını container üzerinden yayınladım.
