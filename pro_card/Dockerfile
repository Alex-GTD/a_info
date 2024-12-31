# 1. Используем официальный образ Python
FROM python:3.12-slim

# 2. Устанавливаем рабочую директорию внутри контейнера
WORKDIR /pro_card

# 3. Копируем файлы проекта в контейнер
COPY . /pro_card

# 4. Устанавливаем зависимости из файла requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# 5. Указываем команду для запуска приложения
CMD ["gunicorn", "main:app", "-b", "0.0.0.0:8080"]
