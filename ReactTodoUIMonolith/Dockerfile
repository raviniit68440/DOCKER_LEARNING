FROM node:latest as Primary
WORKDIR /work 
COPY package*.json .
RUN npm install
COPY . .
RUN npm run build

FROM nginx:latest as Secondary
COPY --from=Primary /work/build /usr/share/nginx/html