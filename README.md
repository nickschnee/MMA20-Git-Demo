# MMA20-Git-Demo

Zum installieren bitte Button herunterladen drücken.

# Installation Tailwind Vue JS

```
vue create hello-world
```

```
 $ cd hello-world
 $ npm run serve
```

```
CTRL + C
CTRL + C
```

### Install Tailwind
```
npm install -D tailwindcss@latest postcss@latest autoprefixer@latest

```

### Create tailwind.config File
Zuerst initialisieren wir ein tailwind.config.js File mit diesem Befehl:

```
npx tailwindcss init -p
```

Nun **löschen** wir das eben erstellte tailwind.config.js File wieder (beispielsweise direkt in VS Code).

Und erstellen ein neues, volles tailwind.config.js
```
npx tailwindcss init --full
```


### Connect Configuration
Check if this is already in the following file:

tailwind.config.js
```
module.exports = {
  content: [
    "./src/**/*.{vue,js,ts,jsx,tsx}"
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

### Create Index.css
/src/index.css
```
@tailwind base;
@tailwind components;
@tailwind utilities;

```

### Import index.css into main.js
/src/main.js
```
import { createApp } from "vue";
import App from "./App.vue";
import router from "./router";
import './index.css'

createApp(App).use(router).mount("#app");

```

### Test Installation
terminal
```
npm run serve
```
