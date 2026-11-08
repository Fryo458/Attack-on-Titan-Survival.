ATTACK ON TITAN: SURVIVAL — ANDROID / APK PROJECT
Версия игры: Update 2.2 Detail Build

ЧТО ВНУТРИ
- www/index.html — текущая HTML-игра, упакованная для Android WebView через Capacitor.
- package.json — зависимости Capacitor.
- capacitor.config.json — имя приложения, Android package ID и папка игры.

ВАЖНО
Это подготовленный исходный проект-оболочка, а не готовый APK. Для сборки APK нужны Android Studio, Android SDK и JDK, а также установка npm-зависимостей.

СБОРКА НА WINDOWS / MAC / LINUX
1. Установите Node.js LTS и Android Studio.
2. Распакуйте архив в отдельную папку.
3. Откройте терминал в папке Attack_on_Titan_Survival_APK_Project.
4. Выполните:
   npm install
   npx cap add android
   npx cap sync android
   npx cap open android
5. В Android Studio дождитесь синхронизации Gradle.
6. Для теста нажмите Run и выберите Android-телефон с включённой USB-отладкой или эмулятор.
7. Для APK: Build > Build Bundle(s) / APK(s) > Build APK(s).
8. APK обычно появится в android/app/build/outputs/apk/debug/app-debug.apk.

ДЛЯ ОБНОВЛЕНИЯ ИГРЫ
Замените www/index.html новой версией HTML, затем выполните:
   npx cap sync android
И пересоберите APK.

ПРИМЕЧАНИЯ
- Для публикации в Google Play потребуется подписанный release AAB/APK и оформление карточки приложения.
- Идентификатор приложения сейчас: com.survival.attackontitan. Не меняйте его после распространения первой версии, если хотите получать обновления поверх неё.
- Перед выпуском обязательно протестируйте управление на реальном телефоне, поворот экрана, сохранение и полноэкранный режим.
