FROM node:17.9.0-slim
LABEL maintainer="Ekangaki Njang"
RUN useradd userapi
WORKDIR /app
RUN chown userapi /app /home
COPY . .
RUN npm install 
EXPOSE 1004
USER userapi
ENV MONGO_URL=""
ENV ADMIN_EMAIL=""
CMD ["npm","start"]
