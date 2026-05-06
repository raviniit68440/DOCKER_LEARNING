FROM nginx:latest

#remove default nginx content
RUN rm -rf /usr/share/nginx/html/*

# Copy your app into nginx folder
COPY . /usr/share/nginx/html
