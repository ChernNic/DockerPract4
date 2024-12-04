# Используем Node.js в легковесной версии
FROM node:alpine

# Устанавливаем рабочую директорию
WORKDIR /app

# Копируем package.json и устанавливаем зависимости
COPY package.json package-lock.json ./
RUN npm install

# Копируем исходный код
COPY . /app/

# Открываем порт для API
EXPOSE 5000

# Указываем команду запуска
CMD ["npm", "start"]
