FROM gcr.io/distroless/nodejs20-debian12
WORKDIR /app
COPY . .
RUN yarn install
EXPOSE 5000
ENTRYPOINT [ "node", "tracker.js"]