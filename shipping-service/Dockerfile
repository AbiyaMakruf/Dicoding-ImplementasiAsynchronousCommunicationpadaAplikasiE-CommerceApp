# Menggunakan base image resmi Node.js
FROM node:18-alpine

# Menentukan direktori di dalam container
WORKDIR /app

# Salin file package.json dan package-lock.json ke dalam container
COPY package.json ./

# Instal dependensi
RUN npm install

# Salin semua file ke dalam container
COPY . .

# Tentukan port yang digunakan oleh aplikasi
EXPOSE 3001

# Menjalankan aplikasi saat container dimulai
CMD ["node", "index.js"]
