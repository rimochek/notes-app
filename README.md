# Getting Started

Install the dependencies and run the project

```
npm install
npm start
```

Also, create the file called "firebase.js", and copy&past the next code:

```
import { initializeApp } from "firebase/app"
import { collection, getFirestore } from "firebase/firestore"

const firebaseConfig = {
  apiKey: "APIKEY",
  authDomain: "AUTH_DOMAIN",
  projectId: "PROJECT_ID",
  storageBucket: "STORAGE_BUCKET",
  messagingSenderId: "MESSAGING_SENDER_ID",
  appId: "APP_ID",
}

const app = initializeApp(firebaseConfig)
export const db = getFirestore(app)
export const notesCollection = collection(db, "notes")
```

Head over to https://vitejs.dev/ to learn more about configuring vite
