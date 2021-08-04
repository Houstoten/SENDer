# SENDer 📮

# Share files seamlessly with people around you using webrtc connection!

Available on [sndr.club](https://sndr.club)

## Technical stack
- Backend ⚙️
  - **Typescript, Node.js, Express**
  - **[Prisma](https://github.com/prisma/prisma), Postgres**
  - **Apollo-server, TypeGraphql**
  - **[Peerjs-server](https://github.com/peers/peerjs-server)** (WebRTC signaling server)
  
- Frontend 🖥️
  - **Typescript, Next.js**
  - **Chakra-ui** (Highly cusotmizable component library)
  - **Apollo-client** (Most popular graphql client)
  - **[Graphql-codegen](https://github.com/dotansimha/graphql-code-generator/)** (Code generation from graphql schema)
  - **[Peerjs-client](https://github.com/peers/peerjs)** (WebRTC client)
  - **[Dexie.js](https://github.com/dfahlander/Dexie.js)** (Minimalistic IndexedDB wrapper)
  - **[Rambda](https://github.com/selfrefactor/rambda)** (Blazing fast functional library)
  
- Authentication 🔒
  - **[Google OpenID](https://developers.google.com/identity/protocols/oauth2)** ([Code flow](https://openid.net/connect/) with Google OpenID specification with httpOnly cookies as transport)
 

## Build Backend

- go to `./sndr-server`
- create your own `.env` file from `.env.example`
- run `npx prisma generate` and `npx prisma migrate`
- connect your own or start predefined `peerjs-server` and `postgres` with `docker-compose up`
- to start the server run `yarn start`

## Build Frontend

- go to `./sndr-client`
- create your own `.env.local` file from `.env.local.example`
- to start the server run `yarn build` and `yarn start`
