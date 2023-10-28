# test_project_mobile

Тестовый проект/Тестовый проект v2

## Начало работы

### Подготовка работы

1. Получение зависимостей: `flutter pub get`
2. Генерация файлов проекта: `flutter pub run build_runner build --delete-conflicting-outputs`
3. Можно также настроить run configuration для запуска из IDE.


### Тестовый проект

1. Настройка env: Создать файл `.env` и скопировать в него содержимое `.env.dev`
2. Запуск проекта: `flutter run --flavor kamball -t lib/main_kamball.dart`
3. Сборка (Android):
   ```
   flutter build appbundle -t lib/main_kamball.dart --flavor=kamball \
       --build-name 1.0.0 --build-number 1 
   ```
4. Сборка (iOS):
   ```
   flutter build ipa -t lib/main_kamball.dart --flavor=kamball \
       --build-name 1.0.0 --build-number 1
   ```

### Тестовый проект v2

1. Настройка env: Создать файл `sakhball.env` и скопировать в него содержимое
   `sakhball.env.dev`
2. Запуск проекта: `flutter run --flavor sakhball -t lib/main_sakhball.dart`
3. Сборка (Android):
   ```
   flutter build appbundle -t lib/main_sakhball.dart --flavor=sakhball \
       --build-name 1.0.0 --build-number 1
   ```
4. Сборка (iOS):
   ```
   flutter build ipa -t lib/main_sakhball.dart --flavor=sakhball \
       --build-name 1.0.0 --build-number 1
   ```

## Релиз 
   Релиз делать из релизных веток release/kamball или release/islands предварительно запушив в одну из них с обязательным
   указанием тега версии, например тег islands-1.0.0+1-RC1
  