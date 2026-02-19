# qa-automation-practicum-first-project
Первый проект на курсе qa automation python в Практикуме

## Работа с bash

**Переход в домашнюю директорию**
```bash
cd ~
``` 

**Переход на одну директорию вверх**
```bash
cd ../
``` 

**Посмотреть список файлов директории (в том числе скрытые):**
```bash
ls -la
```

**Создать папку**
```bash
mkdir first-project-folder
```

**Создать файл**
```bash
touch hello.py
```

**Прочитать файл**
```bash
cat hello.py
```

## Работа с git. Создаем и добавляем ssh-ключ в Debian

1. Генерируем ssh-ключ командой:

```bash
ssh-keygen -t ed25519 -C "ваш_email"
```

2. Ключ будет создан в домашнем каталоге.
3. Копируем ключ встроенной утилитой `xclip`. Для этого в терминале  вводим команду:

```
cat ~/.ssh/id_ed25519.pub | xclip -selection clipboard
```

4. В Github переходим в секцию добавления [ssh-ключей](https://github.com/settings/keys)

5. Нажимаем кнопку **New SSH key**
    - Заполняем название ключа
    - Вставляем из буфера обмена скопированный ключ