FROM nginx:latest
RUN usermod -u 1001 nginx && groupmod -g 1001 nginx
COPY nginx.conf /etc/nginx/conf.d/default.conf
WORKDIR app
RUN 	chown -R nginx:nginx /app && \
	chmod -R 755 /app
COPY homework.html /app
EXPOSE 8000

