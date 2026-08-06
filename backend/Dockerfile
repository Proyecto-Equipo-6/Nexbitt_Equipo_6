FROM node:20-alpine

WORKDIR /app

COPY package.json package-lock.json ./
RUN npm ci --only=production

COPY prisma ./prisma
RUN npx --no-install prisma generate

# Copia selectiva: solo lo que el runtime necesita (no se copia .env ni el resto)
COPY routes ./routes
COPY controllers ./controllers
COPY config ./config
COPY middleware ./middleware
COPY utils ./utils
COPY templates ./templates
COPY app.js server.js socket.js swagger.json ./

# Ejecutar sin privilegios de root
USER node

EXPOSE 3000

CMD ["node", "server.js"]