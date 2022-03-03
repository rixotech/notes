# NestJS
### Install NestJS

Using NestJS CLI

```
npm i -g @nestjs/cli
nest new project-name
```

### Connet MongoDB
Packages:
* mongoose
* @nestjs/mongoose

```
pnpm install --save mongoose @nestjs/mongoose
```

Connection string add in app.module.ts file
```js
import { MongooseModule } from '@nestjs/mongoose'
import { ConfigModule } from '@nestjs/config';

imports: [ConfigModule.forRoot(), MongooseModule.forRoot(process.env.MONGODB_URI)]
```

