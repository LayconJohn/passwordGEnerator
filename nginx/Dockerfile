FROM nginx:1.21-alpine

COPY nginx/nginx.conf /etc/nginx/conf.d

COPY --from=build /app/dist /usr/share/nginx/html

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]