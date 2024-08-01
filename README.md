# Atividade Prática - Pilares da Programação Orientada a Objetos

### Inicialização:
```bash
npm init -y
npm i -D typescript @types/node ts-node-dev
npx tsc --init
```

### Configurações:
`package.json` -> `scripts`  
```json
"start": "node ./dist/index.js",
"build": "tsc",
"dev": "ts-node-dev --respawn --transpile-only ./src/index.ts"
```

`tsconfig.json`  
```json
"target": "ES2022"
"rootDir": "./src"
"outDir": "./dist"
"exclude": ["node_modules"]
```

### Organização de Pastas:

>`.gitignore`   
> node_modules/
> dist/

>`dist`  
> Pasta para os arquivos javascript

>`scr`  
> Pasta para os arquivos typescript  

### Arquivos `src`:
***Classes***
> Cinema
>```typescript
>Ingresso.ts -> classe abstrata
>Normal.ts
>VIP.ts
>Camarote.ts

> Fazenda
>```typescript
>Animal.ts -> classe abstrata
>Cachorro.ts
>Cavalo.ts
>Gato.ts

> Imobiliaria
>```typescript
>Imovel.ts -> classe abstrata
>Novo.ts
>Velho.ts

***Chamadas e Testes***
```typescript
Index.ts
```
