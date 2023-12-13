# Docker Stack

## Kurulum
Repo pull edildikten sonra konteynerleri ayağa kaldırmak için aşağıdaki komut girilmelidir:

```bash
docker-compose up -d
```
> **-d** parametresi, objeler oluşturulurken shell'e düşebilmek için girilir

## Kullanım
docker-compose.yml dosyasında herhangi bir değişiklik yapıldığı zaman konteynerleri ayağı kaldırırken **--build** parametresi eklenmelidir:
```bash
docker-compose up -d --build
```

Uygulamalar **app/** dizinine atılmalıdır. Daha sonra nginx servisinde çalışması istenen port girilip **nginx/conf.d/** dizininde web servisin çalıştıracağı uygulamaya ait conf dosyası oluşturulmalıdır.