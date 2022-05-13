# Introdução ao Git e GitHub

O Git é um sistema de controle de versões distribuido. Que tem a função registrar qualquer alteração feita em um código de forma segura. Essa segurança se dá através do **SHA1**, que é um algoritimo de encriptação de segurança.

O função do SHA1 é pegar o arquivo, texto ou foto e "embaralhar" de forma bem específica, o resultado disso, ou seja, a saída é um conjunto de caracteres com 40 dígitos. Esses conjuntos são únicos e servem como identifição de forma rápida e segura. Cada arquivo possui uma chave, como uma assinatura, que garante e identifica se houve alguma modificação no arquivo, pois a cada modificação é gerada uma chave nova.

A forma de interagir com o Git é por linha de comando (CLI) e não Graphic User Interface (GUI).

**Benefício do uso do Git**

1. Controle de versões
2. Armazenamento na nuvem
3. Trabalho em equipe
4. Merlhoramento do código (é uma exposição do código para o mundo, as pessoas podem melhorá-lo e interagir com ele)
5. Reconhecimento (é uma espécie de rede social onde pessoas interagem)


## Objetos do Git

Pensando em uma visão do micro para o macro, o Git é dividido em 3 objetos: Blob, Tree e Commit. Ou seja, os Commits possuem Trees, que por sua vez possuem Blobs ou outras Trees.

1. **Blobs - bolhas**
- É um objeto que contém metadados, um bloco básico de composição que guardam apenas o tamanho e o SHA1 do arquivo.

2. **Trees - árvores**
- Elas armazenam blobs e apontem para tipos de blobs. A tree também contem metadados (\0), guardando o nome do aquivo, e é responsável por montar toda estrutura de localização do arquivo. Elas podem apontar para blobs ou para outras Trees. Cada tree também possui um SHA1 desse metadado, e esse SHA1 é interligado com o SHA1 do blob, ou seja, se mudar o arquivo da blob, consequentemente muda o SHA1 da tree.

![Organização de blob e Tree](<c:\workspace\Bootcamp DIO\Módulo 1\Imagens\blobetree.png>)
  
  
