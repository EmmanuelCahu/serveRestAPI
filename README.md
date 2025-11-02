# Teste de API Rest do manual a CI/CD

## O que é 
Este repositorio foi criado com o intuito de testar API Rest

## Tecnologias utilizadas
1. Postman for Web V11.69.7-251031-0540  Browser & OS Chrome 141, Windows 10
2. Newman V6.2.1
3. Node V24.10.0
4. Newman-reporter-htmlextra V1.23.1

## Documentação
Doc da API : [Consulte Swagger](https://serverest.dev/)

## Como instalar o ambiente
1. Instalar o node [Link](https://nodejs.org/en/download)
2. Realize a instalação do Newman de forma global. [Link da dependência](https://www.npmjs.com/package/newman) 
3. Instalar o reporter htmlextra (opcional) accesse o [Link](https://www.npmjs.com/package/newman-reporter-htmlextra)
```
npm install -g newman-reporter-htmlextra
```  
## Como rodar os testes

### Pelo Postman web ou desktop
1. Importe a collection e o environment
2. Execute os testes de forma manual ou automatizada
### Pelo newman
1. Abra o console de preferencia
2. Execute a seguinte linha de comando para rodar os testes
```
newman run ServeRest.postman_collection.json -e serveRest_env.postman_environment.json -r cli
```
3. Execute os testes com relatório
```
newman run ServeRest.postman_collection.json -e serveRest_env.postman_environment.json -r cli,htmlextra
```
### Report
Os testes com **htmlextra** geram um arquivo `.html` contendo o resultado completo dos testes.

- **Localização do relatório:** o arquivo é disponibilizado como **artifact** no GitHub Actions.  
- **Como acessar:**
  1. Acesse o seu repositório no GitHub.  
  2. Vá em **Actions → Newman run → Última execução → Artifacts → newman-report → Download**.  
  3. Descompacte o arquivo `.zip` baixado.  
  4. Abra o arquivo `.html` em seu navegador para conferir os resultados das validações.
 
## Entre em contato
email: emmanuelcahu@hotmail.com

redes sociais: https://www.linkedin.com/in/carlosemmanuelcahu/
