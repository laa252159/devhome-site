# DEVHOME site content

Контент сайта `starkuz.ru` — отдельный проект разработки.

## Что здесь

- `index.html` — страница DEVHOME;
- `orca.jpg` — фото касатки (NOAA, Public Domain);
- `kustomization.yaml` — собирает ConfigMap `site-content` из двух файлов.

## Как обновить сайт

```sh
# правите index.html и/или orca.jpg
git add .
git commit -m "описание изменения"
git push
```

Изменения подхватываются автоматически при push в `master`.

Инфраструктура (Ingress, TLS, Deployment, Service) лежит в отдельном приватном
репозитории и здесь не хранится.
