# Публикация Zargariyan / Naira Signature Boutique на GitHub Pages

Этот сайт уже подготовлен как статический проект для GitHub Pages. Ему не нужен `npm install`, сборка, сервер или база данных. GitHub будет публиковать файлы напрямую из корня репозитория.

## 1. Создать репозиторий на GitHub

1. Откройте GitHub.
2. Нажмите `+` в правом верхнем углу.
3. Выберите `New repository`.
4. Название можно поставить, например:

```text
naira-signature-boutique
```

5. Выберите `Public`, если у вас обычный бесплатный GitHub и вы хотите опубликовать сайт через GitHub Pages.
6. Не включайте `Add a README file`, `.gitignore` и `license`, потому что эти файлы уже есть локально.
7. Нажмите `Create repository`.

## 2. Загрузить сайт в репозиторий

Откройте Terminal и выполните команды:

```bash
cd "/Users/filianov/Documents/New project/naira-signature-boutique"
git init
git branch -M main
git add .
git commit -m "Publish Zargariyan boutique"
git remote add origin https://github.com/YOUR_USERNAME/naira-signature-boutique.git
git push -u origin main
```

Замените `YOUR_USERNAME` на свой логин GitHub.

Если GitHub покажет вам SSH-адрес вместо HTTPS, можно использовать такой вариант:

```bash
git remote add origin git@github.com:YOUR_USERNAME/naira-signature-boutique.git
git push -u origin main
```

## 3. Включить GitHub Pages

1. Откройте созданный репозиторий на GitHub.
2. Перейдите в `Settings`.
3. В левом меню откройте `Pages`.
4. В блоке `Build and deployment` выберите:

```text
Source: Deploy from a branch
Branch: main
Folder: / (root)
```

5. Нажмите `Save`.

## 4. Открыть опубликованный сайт

Через несколько минут GitHub Pages выдаст адрес вида:

```text
https://YOUR_USERNAME.github.io/naira-signature-boutique/
```

Если сайт не появился сразу, подождите 5-10 минут и обновите страницу.

## 5. Как обновлять сайт после правок

После любых изменений в файлах выполните:

```bash
cd "/Users/filianov/Documents/New project/naira-signature-boutique"
git status
git add .
git commit -m "Update boutique site"
git push
```

GitHub Pages сам обновит опубликованный сайт.

## 6. Что важно перед коммерческим запуском

Сейчас сайт готов как премиальная витрина и демо-каталог. Перед реальными продажами нужно:

- заменить демо-юридические ссылки на настоящие страницы для Австрии: `Impressum`, `Datenschutz`, `AGB`, `Widerruf`;
- подключить реальный платежный процессинг: Stripe, PayPal, Klarna или другой backend;
- заменить ссылку Instagram на настоящий профиль;
- проверить цены, наличие, доставку и правила продажи алкоголя.

