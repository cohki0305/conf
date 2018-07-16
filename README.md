# conf

## Project setup
```
npm install
```

## Setup firebase

visit [firebase](https://firebase.google.com/) and create new project to get config information.

create file `src/firebase.config.js` like following code.

```javascript

const config = {
  apiKey: '...',
  authDomain: '...',
  databaseURL: '...',
  projectId: '...',
  storageBucket: '',
  messagingSenderId: '...'
}

export default config
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```
