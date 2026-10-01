FROM node:24-alpine

WORKDIR /app

# คัดลอก package files เพื่อแคชการ install dependencies
COPY package*.json ./
RUN npm install

# คัดลอกซอร์สโค้ดทั้งหมด
COPY . .

# กำหนด Port สำหรับ Express Backend
EXPOSE 3001

CMD ["node", "index.js"]
