FROM node:16 AS builder
WORKDIR /frontend
COPY . /frontend/

RUN npm install
ENTRYPOINT ["npm"]
CMD ["run", "build"]
