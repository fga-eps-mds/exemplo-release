# Repositório de Exemplo

Esse repositório é um exemplo para utilização dos scripts de geração de release. Para a utilização dos scripts em outros projetos são necessárias as seguintes modificações:

## Scripts

É necessário copiar a pasta `scripts` completa, inclusive o package.json que é independente do package geral do projeto. A pasta deve ficar na raiz do projeto.

Também é preciso copiar o arquivo `release.yml` e o path dele deve ser **exatamente** assim: `.github/workflows/release.yml`

## Repository Secrets

Também é preciso configurar *secrets* para que seja possível o correto funcionamento. As secrets são:

* API_TOKEN_GITHUB = Token gerado pelo github por 1 usuário

* GIT_DOC_REPO = Nome do repositório de documentação, ex: 2023-1-Alectrion-DOC

* GIT_USER_EMAIL = Endereço de email do usuário do GitHub que gerou o API_TOKEN_GITHUB

* GIT_USER_NAME = Nome do usuário do GitHub que gerou o API_TOKEN_GITHUB

* SONAR_TOKEN = Token gerado pelo Sonar para possibilitar análises

## Labels de Pull Requests

* NOT RELEASE : #d73a4a

* MAJOR RELEASE : #11C955

* MINOR RELEASE : #BE059B

* FIX RELEASE : #cfd3d7

* DEVELOP : #0075ca