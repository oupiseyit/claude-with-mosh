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
