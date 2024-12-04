# Используем легковесный образ Node.js
FROM node:alpine

# Устанавливаем рабочую директорию
WORKDIR /app

# Копируем package.json и устанавливаем зависимости
COPY package.json package-lock.json ./
RUN npm install

# Копируем весь исходный код
COPY . /app/

# Открываем порт 8954 для фронтенда
EXPOSE 8954

# Запускаем фронтенд через Vite
CMD ["npm", "run", "dev"]
