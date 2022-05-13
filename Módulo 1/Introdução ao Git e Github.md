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

![Organização de blob e Tree](<https://github.com/Gabijesumary/Bootcamp-Avanade-DIO/blob/3dc2581089b75397d91939906167a6098b298fc9/M%C3%B3dulo%201/Imagens/blobetree.png>)
  

3. **Commit**
O commit é um tipo de objeto "que junta tudo". Ele aponta para trees, para parentes (commits realizados antes deles), para o autor do aquivo, e uma mensagem sobre o commit realizado. Essa mensagem serve para explicar, dar significado para essa aglomerados de aquivos. Ele também leva todas as informações da data e hora da criação dele. O SHA1 desse commit também é interligado com os SHA1 dos blobs, trees e outros commits que estão relacionados a eles. 
  
![Organização de blob e Tree](<https://github.com/Gabijesumary/Bootcamp-Avanade-DIO/blob/3dc2581089b75397d91939906167a6098b298fc9/M%C3%B3dulo%201/Imagens/Commits.png>)
  

## Comandos com Git

Todos os comando são dados com a fonte em caixa baixa, aqui estão dispostos em caixa alta apenas para diferenciar e dar destaque do restante do texto.

1. **LS**
2. **CD**
    - cd/ +
    - cd ..
3. **MKDIR**
4. **RMDIR**
5. **GIT INIT**
6. **Is -a**
7. **GIT ADD**
    - git add * - 
8. **GIT STATUS**
9. **GIT COMMIT -M "MENSAGEM COMMIT"**
10. **MV** $ mv arquivo.txt ./pastanova/
11. **GIT CLONE**
12. **GIT REMOTE ADD ORIGIN** + URL
13. **GIT REMOTE -V**
14. **GIT PUSH ORIGIN MASTER (OU MAIN)**
15. **GIT PULL ORIGIN MASTER (OU MAIN)**


## Atalhos no Git
1. **Tab**
2. **Ctrl + L**

