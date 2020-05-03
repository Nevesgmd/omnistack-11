# Semana Omnistack 11 - Be The Hero

An application produced on a  [Rocketseat](https://rocketseat.com.br/) workshop to help nonprofit organizations to achieve their goals.

## Technologies Used
* [Node.js](https://nodejs.org/en/)
* [React JS](https://pt-br.reactjs.org/)
* [React Native](https://reactnative.dev/)

## How to Run the Project
After cloning all the files in this repository, follow each one of the next steps to run the back-end, front-end and mobile.

### Back-end
Move into the back-end directory with the `terminal`/`cmd` and run the following lines of code.
```
npm install
npx knex migrate:latest --env development
npm run start
```

### Front-end
Edit `src/services/api.js` and add your back-end URL (or use the default: `http://localhost:3333`).
```
import axios from 'axios';

const api = axios.create({
  baseURL: 'http://localhost:3333',
});

export default api;
```
Move into the front-end directory with the `terminal`/`cmd` and run the following lines of code:
```
yarn
yarn run start
```

### Mobile
Edit `src/services/config.js` and add your back-end URL (or use the default: `http://127.0.0.1:3333`).
```
import axios from 'axios';

const api = axios.create({
  baseURL: 'http://127.0.0.1:3333',
});

export default api;
```
Move into the mobile directory with the `terminal`/`cmd` and run the following lines of code:
```
yarn
yarn run start
```
Metro Bundler will open with your run options.
