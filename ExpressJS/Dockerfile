# 1. Base image olarak resmi Node.js image kullan
FROM node:18-alpine

# 2. Çalışma dizinini oluştur
WORKDIR /app

# 3. Bağımlılıkları kopyala ve yükle
COPY app/package.json ./
RUN npm install

# 4. Uygulama kodlarını kopyala
COPY app .

# 5. Container içindeki uygulamayı çalıştır
CMD ["npm", "start"]

# 6. Uygulamanın çalışacağı portu belirt
EXPOSE 3000
