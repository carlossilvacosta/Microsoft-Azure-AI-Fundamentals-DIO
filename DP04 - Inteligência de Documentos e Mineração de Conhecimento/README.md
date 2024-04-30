<h1>
    <a href="https://www.dio.me/">
     <img align="center" width="60px" src="https://hermes.dio.me/lab_projects/badges/619af8f8-d138-4e40-9d48-fec7b318e44d.png"></a>
    <span> 
Inteligência de Documentos e Mineração de Conhecimento</span>
</h1>

## Azure Cognitive Search: Utilizando AI Search para indexação e consulta de Dados

- **Desafio de Projeto:**
O desafio propõe que seja criada uma pesquisa que funcione juntamente com um serviço de inteligência artificial para identificar palavras chave, sentimentos, utilizando também o serviço de armazenamento do azure.

[Documentação](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/11-ai-search.html)

## Criação dos Recursos - Azure AI Search e Azure AI Services:
Inicialmente é necessário realizar a criação dos recursos. Na área de criação do recurso, pode-se ir na área de busca e procurar pelo serviço do Azure chamado: Azure AI Search e em seguida o Azure AI Services, realizma-se os procedimentos preenchendo com os dados necessários para a criação das respectivas instâncias.


- **Passo 01: Azure AI Search**
<img align="right" src="https://github.com/carlossilvacosta/Microsoft-Azure-AI-Fundamentals-DIO/blob/main/Imagens/Intelig%C3%AAncia%20de%20Documentos%20e%20Minera%C3%A7%C3%A3o%20de%20Conhecimento%20-%20DP04/gif00.gif" width=""/>

...

- **Passo 02: Azure AI Services**
<img align="right" src="https://github.com/carlossilvacosta/Microsoft-Azure-AI-Fundamentals-DIO/blob/main/Imagens/Intelig%C3%AAncia%20de%20Documentos%20e%20Minera%C3%A7%C3%A3o%20de%20Conhecimento%20-%20DP04/gif01.gif" width=""/>

...

- **Passo 03: Criando o Storage Account**
<img align="right" src="https://github.com/carlossilvacosta/Microsoft-Azure-AI-Fundamentals-DIO/blob/main/Imagens/Intelig%C3%AAncia%20de%20Documentos%20e%20Minera%C3%A7%C3%A3o%20de%20Conhecimento%20-%20DP04/gif02.gif" width=""/>

...

- **Passo 04: Permitindo Acesso Anônimo ao Blob**

...

O laboratório é apenas didático, para aprender os princípios da inteligência artificial com o Azure, precisamos permitir o acesso anônimo ao blob para simplificar e facilitar nossas implementações. Após criar o seu Storage, entre no mesmo e navegue até a guia SETTINGS > CONFIGURATION seguindo os passos abaixo:

<img align="right" src="https://github.com/carlossilvacosta/Microsoft-Azure-AI-Fundamentals-DIO/blob/main/Imagens/Intelig%C3%AAncia%20de%20Documentos%20e%20Minera%C3%A7%C3%A3o%20de%20Conhecimento%20-%20DP04/gif03.gif" width=""/>

...

- **Passo 03: Criando o Conteiner**
<img align="right" src="https://github.com/carlossilvacosta/Microsoft-Azure-AI-Fundamentals-DIO/blob/main/Imagens/Intelig%C3%AAncia%20de%20Documentos%20e%20Minera%C3%A7%C3%A3o%20de%20Conhecimento%20-%20DP04/gif04.gif" width=""/>

...

- **Passo 04: Carregando Arquivos**
<img align="right" src="https://github.com/carlossilvacosta/Microsoft-Azure-AI-Fundamentals-DIO/blob/main/Imagens/Intelig%C3%AAncia%20de%20Documentos%20e%20Minera%C3%A7%C3%A3o%20de%20Conhecimento%20-%20DP04/gif05.gif" width=""/>

...

- **Passo 05: Importar e Indexar Dados para o AZURE AI SEARCH**

Neste passo é precisa anexar / importar os dados que foram inseridos e configurados no seu STORAGE. No AI SEARCH, siga os passos abaixo:

<img align="right" src="https://github.com/carlossilvacosta/Microsoft-Azure-AI-Fundamentals-DIO/blob/main/Imagens/Intelig%C3%AAncia%20de%20Documentos%20e%20Minera%C3%A7%C3%A3o%20de%20Conhecimento%20-%20DP04/gif06.gif" width=""/>

...

Esta é a parte mais importante de todo o processo, assim como o bootcamp apresenta, são muitos passos que você precisa seguir a risca, achei apenas uma diferença da documentação oficial para o que achei quando configurei o meu.

Ao seguir a Documentação você chegará em INDEX DOCUMETS, o qual o gif acima mostra o início do processo, siga os topicos até chegar na sessão 4:

<img align="right" src="https://raw.githubusercontent.com/carlossilvacosta/Microsoft-Azure-AI-Fundamentals-DIO/main/Imagens/Intelig%C3%AAncia%20de%20Documentos%20e%20Minera%C3%A7%C3%A3o%20de%20Conhecimento%20-%20DP04/foto00.png" width=""/>

...

"4. In the Attach Cognitive Services section, select your Azure AI services resource."

Note que a instrução manda que selecionemos o recurso AI SERVICE configurado, porém para mim não mostrou nenhum, apenas uma informação dizend que meu acesso era gratúitoe que as configurações são limitadas, não se preocupe e pode passar para o passo 5 . In the Add enrichments section.

Siga todas as configurações terminando no passo 17: 'Select the indexer name to see more details'.

...

- **Passo 06: Consultar o índice:**

Realizadas todas as configurações vamos voltar ao AZURE AI SERVICES, entrar no nosso serviço e através do SEARCH EXPLORER testar se tudo foi indexado e se a consulta esta funcionando, utilizando os comandos:

<img align="right" src="https://raw.githubusercontent.com/carlossilvacosta/Microsoft-Azure-AI-Fundamentals-DIO/main/Imagens/Intelig%C3%AAncia%20de%20Documentos%20e%20Minera%C3%A7%C3%A3o%20de%20Conhecimento%20-%20DP04/foto01.png" width=""/>

...

<img align="right" src="https://raw.githubusercontent.com/carlossilvacosta/Microsoft-Azure-AI-Fundamentals-DIO/main/Imagens/Intelig%C3%AAncia%20de%20Documentos%20e%20Minera%C3%A7%C3%A3o%20de%20Conhecimento%20-%20DP04/foto02.png" width=""/>

...

```
search=*&$count=true    (  verifica se a indexação esta funcionando e mostra os documentos )
```
...

<img align="right" src="https://raw.githubusercontent.com/carlossilvacosta/Microsoft-Azure-AI-Fundamentals-DIO/main/Imagens/Intelig%C3%AAncia%20de%20Documentos%20e%20Minera%C3%A7%C3%A3o%20de%20Conhecimento%20-%20DP04/foto03.png" width=""/>

...
 
```
search=locations:'Chicago' ( Consulta as ocorrencias acontecidas em Chicado )
```
...

<img align="right" src="https://raw.githubusercontent.com/carlossilvacosta/Microsoft-Azure-AI-Fundamentals-DIO/main/Imagens/Intelig%C3%AAncia%20de%20Documentos%20e%20Minera%C3%A7%C3%A3o%20de%20Conhecimento%20-%20DP04/foto04.png" width=""/>

...

```
search=sentiment:'negative' ( Consulta as ocorrencias com sentimento negativo )
```

- **Considerações Finais**
As ferramentas de Machine Learning e Inteligência Artificial do Azure facilitam a consulta em documentos e pesquisas, agilizando ainda mais a consulta de satisfação de empresas sobre seus produtos e serviços.