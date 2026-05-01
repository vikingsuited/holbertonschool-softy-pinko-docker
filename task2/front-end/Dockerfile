FROM nginx:latest

# Front-end fayllarını kopyalayırıq
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Öz konfiqurasiya faylımızı standart Nginx konfiqurasiyası ilə əvəzləyirik
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
