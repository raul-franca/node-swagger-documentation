# Instalação do Swagger
```bash
  npm install swagger-ui-express
  npm install @types/swagger-ui-express --save-dev
```

# Configuração do Middleware

```
import swaggerUi from 'swagger-ui-express';
import swaggerFile from './swagger.json';

private middleware(): void {
    this.express.use(express.json());
    this.express.use(
        "/api-docs",
        swaggerUi.serve,
        swaggerUi.setup(swaggerJson)
    );
```


# node-swagger-documentation
