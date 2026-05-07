# AgroVisualizer Pro — Android APK

## Як отримати APK за 5 хвилин (безкоштовно, без встановлення нічого)

### Крок 1 — Завантаж проєкт на GitHub

1. Зайди на [github.com](https://github.com) → **Sign up** (якщо немає акаунта)
2. Натисни **«+»** → **New repository**
3. Назва: `agrovisualizer` → **Create repository**
4. Натисни **«uploading an existing file»**
5. Перетягни ВСІ файли з цієї папки → **Commit changes**

### Крок 2 — Запусти збірку

1. Відкрий вкладку **Actions** у репозиторії
2. Зліва натисни **«Build APK»**
3. Натисни **«Run workflow»** → **Run workflow** (зелена кнопка)
4. Зачекай ~3-5 хвилин ☕

### Крок 3 — Завантаж APK

1. Коли з'явиться зелена галочка ✅ — натисни на неї
2. Внизу сторінки знайди **Artifacts → AgroVisualizerPro**
3. Натисни → завантажиться `AgroVisualizerPro.zip` з APK всередині

### Крок 4 — Встанови на телефон

1. Перенеси APK на телефон (через кабель або Telegram до себе)
2. Відкрий файл на телефоні
3. Android запитає дозвіл → **«Встановити з невідомих джерел»** → дозволь
4. Готово — іконка з'явиться на робочому столі!

---

## Структура проєкту

```
android-project/
├── app/
│   ├── src/main/
│   │   ├── assets/public/
│   │   │   └── index.html          ← весь додаток тут
│   │   ├── java/com/agrovisualizer/app/
│   │   │   └── MainActivity.java   ← WebView обгортка
│   │   ├── res/mipmap-*/
│   │   │   └── ic_launcher.png     ← іконки
│   │   ├── AndroidManifest.xml
│   │   └── res/values/styles.xml
│   └── build.gradle
├── .github/workflows/
│   └── build.yml                   ← автоматична збірка
├── build.gradle
└── settings.gradle
```

## Оновлення додатку

Щоб оновити — просто заміни `app/src/main/assets/public/index.html`
і знову запусти **Actions → Run workflow**.
