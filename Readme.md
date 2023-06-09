1. Project setup [gitignore]
2. Eslint & Pretier
3. Huisky & Lint stage

## today lesson

**Module-11.1**

- login jira software management and create project backlog {stramp template}
- init json file

**Module-11.2**

- npm init --y
- npm install typescript --save-dev
- tsc --init
- install express mongoose dotenv
- npm i express mongoose dotenv

## **Module -11.3 setup dotenv**

- npm i dotenv
- create config folder
- index.ts

```ts
import dotenv from 'dotenv';
import path from 'path';
dotenv.config({ path: path.join(process.cwd(), '.env') });
export default {
	port: process.env.PORT,
	dataBaseUrl: process.env.DATABASE_URL,
};
```

**ts node dev**

```
 npm i ts-node-dev --save-dev
 ts-node-dev --respawn --transpile-only server.ts
```

## Module 11.4

- cors
- purser

```js
app.use(cors());
app.use(express.json());
// if url encode data come
app.use(express.urlencoded({ extended: true }));
```
