# Bootcamp 01 Qualiters club
Teste de API Rest do manual a CI/CD

## O que é 
Este repositorio foi criado com o intuito de testar API Rest

## Tecnologias utilizadas
Postman for Web V11.69.7-251031-0540  Browser & OS Chrome 141, Windows 10
Newman V6.2.1
Node V24.10.0
Newman-reporter-htmlextra V1.23.1

## Documentação
Doc da API : [Consulte Swagger](https://serverest.dev/)

## Como instalar o ambiente
- 1º: Instalar o node [Link](https://nodejs.org/en/download)
- 2º: Realize a instalação do Newman de forma global. [Link da dependencia](https://www.npmjs.com/package/newman) 
- 3º: Instalar o reporter htmlextra (opcional) accesse o [Link](https://www.npmjs.com/package/newman-reporter-htmlextra)
```
npm install -g newman-reporter-htmlextra
```  
## Como rodar os testes

### Pelo Postman web ou desktop
- Importe a collection e o environment
- Execute os testes de forma manual ou automatizada
### Pelo newman
- Abra o console de preferencia
- Execute a seguinte linha de comando para rodar os testes
```
newman run ServeRest.postman_collection.json -e serveRest_env.postman_environment.json -r cli
```
- Execute os testes com relatório
```
newman run ServeRest.postman_collection.json -e serveRest_env.postman_environment.json -r cli,htmlextra
```
### Report
Se você optou por rodar os testes com o report htmlextra, você gerou um arquivo .html com o resutado dos testes e para verificar as validações, voce pode abrir a pasta **newman** que foi criada no local em que os arquivos de collection e environment se encontram.

## Entre em contato
email: emmanuelcahu@hotmail.com

redes sociais: https://www.linkedin.com/in/carlosemmanuelcahu/
