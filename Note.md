# creating the project structure

## install project with bun
```
bun install
```

- remove folder '.cursor'

## install backend project with bun
```
cd package/server
bun install
bun add express
bun add -d @types/express
```
- remove folder '.cursor'
- run project `bun run dev`

## Managing-Openai-Api-Key
```
cd package/server
bun add dotenv
```
- create file .env

## creating the project for client
```
bun create vite .
bun i
```

- run project `bun run dev`

## Running-Both-Apps-Together
```
 bun add concurrently

```
- index.ts
```
import concurrently from "concurrently";

concurrently([
    {
        name: "server",
        command: "bun run dev",
        cwd: "packages/server",
        prefixColor: "cyan",
    },
    {
        name: "client",
        command: "bun run dev",
        cwd: "packages/client",
        prefixColor: "green",
    },
]);

```

# Setting-up-Tailwindcss
```
cd packages/client
bun add tailwindcss @tailwindcss/vite
```