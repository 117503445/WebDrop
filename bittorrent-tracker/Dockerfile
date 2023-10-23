FROM node:20-bookworm as build
WORKDIR /app
COPY . .
RUN yarn install
# ENTRYPOINT [ "sh" ]

FROM gcr.io/distroless/nodejs20-debian12
WORKDIR /app
COPY --from=build /app /app
EXPOSE 5000
CMD [ "tracker.js" ]