# Pertemuan 3

## Persiapan

Dalam pertemuan ke 3 ini kita akan membuat sebuah aplikasi ToDo List sebagai bentuk penyempurna dari aplikasi yang telah kita buat di pertemuan ke 2.

di pertemuan ini kita akan mempelajari pembuatan sebuah Restfull API yang nanti akan dikonsumsi oleh frontend secara realtime update atau disebut asynchronuos  menggunakan jQuery, juga kita akan memplejari templating html, css dan js menggunakan CSS framework Bootstrap.

Sebelum mempelajati lebih lanjut diharapkan peserta telah membaca dan mempersiapkan materi referensi tentang :
* REST API menggunakan Codeigniter [disini](https://belajarphp.net/membuat-rest-api-codeigniter/) 
* Api Dokumentasi menggunakan apidocjs [disini](http://apidocjs.com/) 
* CSS Framework Bootstrap
* Javascript Framework jQuery


## Materi
### Mengenal REST API
Membuat REST atau RESTfull API Dengan Codeigniter – REST (REpresentational State Transfer) adalah suatu arsitektur atau metode komunikasi yang sering diterapkan dalam pengembangan layanan berbasis web. Arsitektur REST yang umumnya dijalankan via HTTP (Hypertext Transfer Protocol), melibatkan proses pembacaan laman web tertentu yang memuat sebuah file XML atau JSON. File inilah yang menguraikan dan memuat konten yang hendak disajikan. Setelah melalui sebuah proses definisi tertentu, konsumen dalam hal ini frontend atau Mobile (Android/iOS) akan bisa mengakses antarmuka aplikasi yang dimaksudkan.

Perhatikan table standar method yang didefinisikan untuk semua resource dan collections dari REST API :

| Methods | Scope | Descriptions |
| -- | -- | -- |
| GET | collection | Retrieve all resources in a collection |
| GEt | resource | Retrieve a single resource |
| HEAD | collection | Retrieve all resources in a collection (header only) |
| HEAD | resource | Retrieve a single resource (header only) |
| POST | collecction | Create a new resource in a collection |
| PUT | resource | Update a resource |
| PATCH | resource | Update a resource |
| DELETE | resource | Delete a resource |
| OPTIONS | any | Return available HTTP methods and other options |

Contoh request URI pada REST API

```
HTTP GET http://www.appdomain.com/todos
HTTP GET http://www.appdomain.com/todos?size=20&page=5
HTTP GET http://www.appdomain.com/todos/123
HTTP GET http://www.appdomain.com/todos/123/completed
```

Berikut contoh output dengan method `HTTP GET` pada RESTfull 

`http://api.domain.com/todos/10`

```
{
    "id": 10,
    "name": "Workshop Technical Backend on Bekup 2.0",  
    "is_status" : 1,
    "users": [
        {
            "name": "Mukidi",
            "email": "me@mukidi.co"
        }
    ]
}

```




## Project

