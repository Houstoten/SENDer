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
  
- Authentication 🔒
  - **[Google OpenID](https://developers.google.com/identity/protocols/oauth2)** ([Code flow](https://openid.net/connect/) with Google OpenID specification with httpOnly cookies as transport)
 

## Build Backend

- create your own `.env` file from `.env.example`
- connect your own or start predefined `peerjs-server` and `postgres` with `docker-compose up`
- to start the server run `yarn start`

## Build Frontend

- create your own `.env` file from `.env.example`
- to start the server run `yarn build` and `yarn start`
