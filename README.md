# 👗🌤️ Agente de Recomendações de Vestuário e Cuidados Pessoais

## 📝 Introdução

Bem-vindo ao repositório do **Agente de Recomendações de Vestuário e Acessórios**, desenvolvido no **Azure AI Foundry**! ✨

Este agente foi criado para ajudar pessoas no seu dia a dia, de forma prática e simpática. Ele utiliza informações de **localização** e das **cidades pelas quais o usuário passa diariamente**, combinando esses dados com as **previsões do tempo fornecidas pelo GetweatherMSN_Tool**.

A partir disso, o agente oferece sugestões personalizadas sobre:

* 👕 **O que vestir** (roupas leves, casacos, tecidos recomendados etc.)
* 🕶️ **Quais acessórios usar** (óculos de sol, guarda-chuva, gorro e muito mais)
* 💄 **Quais cosméticos são adequados** (protetor solar, hidratantes, produtos antioleosidade etc.)

Tudo isso para garantir mais conforto, cuidado e praticidade na rotina do usuário, independentemente das mudanças climáticas! 🌦️

## 🧭 Detalhes de Desenvolvimento

Esta seção descreve de forma mais completa como o agente trabalha com **informações de localização** e a **previsão do tempo** e como você pode registrar ou visualizar testes.

### 📍 Informações de Localização

O agente utiliza dados de localização para identificar:

* A cidade atual do usuário
* As cidades pelas quais o usuário costuma passar diariamente
* Possíveis variações climáticas entre diferentes regiões
  
O texto é o seguinte: Eu moro no brasil, região sudeste na cidade de Sumaré. Porém, no meu dia eu passo pela cidade de Campinas e Indaiatuba, pois trabalho em Indaiatuba e Campinas está no meu percurso.
Eu trabalho de segunda a sexta, portanto nesses dias eu passo por Campinas e Indaiatuba, porém de final de semana eu fico em Sumaré. Um arquivo **.txt** e anexado como **Conhecimento** ao agente.

### 🌦️ Informações sobre o tempo.

Para a previsão do tempo, o agente usa a ação ⚙️ GetweatherMSN_Tool  fornecida como ferramenta de aplicativo lógico do Azure para ajudar nas ações do agente.


### 🖼️ Espaço para Prints de Testes

Abaixo você pode inserir capturas de tela dos testes realizados:

* **Print 1:**
  
  Configurações do agente:
  
  <img width="618" height="665" alt="image" src="https://github.com/user-attachments/assets/a6f759c7-0c4e-41ea-be27-af4954c47ab7" />


  <img width="649" height="650" alt="image" src="https://github.com/user-attachments/assets/39d47845-e49c-4d56-b027-1d9dd06998fe" />
  
  
* **Print 2:**
  
  Testes do Playground:
  
  Essas são as intruções completas do agente 📝: Quero que você faça uma pesquisa sobre o tempo na região em que estou fornecida em um documento na aba conhecimentos. Inicialmente, acesse o aplicativo lógico das ações e obtenha as informações do clima. Posteriormente, forneça informações sobre roupas (roupas leves, casacos, tecidos recomendados etc.), cosméticos (protetor solar, hidratantes, produtos antioleosidade etc.) e acessórios (óculos de sol, guarda-chuva, gorro e muito mais) que devo usar para estar preparada e protegida para qualquer problema que eu possa enfrentar no meu dia relacionado às questões do clima. Quero que para a previsão do tempo você utilize apenas o GetweatherMSN_Tool e as informações pessoais, apenas o arquivo que forneço no conhecimento. Você só pode responder a essas ações, qualquer outra informação solicitada você responde: não tenho permissão para responder isso!
Podem ser perguntas do tipo: como me preparo para o dia de hoje, o que devo usar, o que me espera hoje e variações dentro desse contexto.

  Usei a seguinte pergunta 🤔 ❓ :

  
  <img width="1135" height="110" alt="image" src="https://github.com/user-attachments/assets/755bcf7f-2826-4ec6-901d-228ec67480bf" />
  

* **Print 3:** *Resultado Obtido*

  
  <img width="1018" height="482" alt="image" src="https://github.com/user-attachments/assets/e71657c1-eb15-4fec-bfb3-52cdb55b7ccd" />
  

### ✨ Espaço para Complementos

  Use esta área para adicionar notas, melhorias, diagramas de arquitetura ou qualquer outra informação relevante:

**Fluxo de funcionamento 🔄**

  Dentro das instruções são fornecidas informações de qual a linha de fluxo o agente deve assumir. Ele deve pegar as informações de localidade, pegue as informações do clima pelo aplicativo lógico e crie instruções com conselhos. Portanto a ideia é que ele sempre siga esse fluxo. Ainda, é passada a informação que ele deve dizer "não tenho permissão para responder isso!". Abaixo temos um exemplo de informações que ele se nega a responder:

  <img width="1119" height="214" alt="image" src="https://github.com/user-attachments/assets/16ac33e3-c05c-4dd9-994f-9f74a1e24733" />

  Ou uma possibilidade que envolva tempo:

  <img width="1109" height="192" alt="image" src="https://github.com/user-attachments/assets/72ccb0a1-69d9-4b18-aa7e-5f8d49a1a260" />

  A ideia é que ele apenas seja um conselheiro de preparação para as ações do tempo no dia.

**Melhorias ✨**

 Ainda como forma de melhoria, é interessante incluir mais ferramentas que facilitem o dia a dia da pessoa, como a inclusão de envio de e-mail com as informações criadas, um aplicativo mais completo que inclua um Trigger de ação diária, com obtenção das informações do agente e o envio do e-mail. Porém não tive acesso a muitas funcionalidades o que prejudicou o aprimoramento da ferramenta.

 # Referências:
 
  *➤ ai.azure.com*
  *➤ https://azure.microsoft.com/en-us/products/logic-apps/*
  
 # Agradecimentos:

🎉  **WoMakerCode**
🎉  **Microsoft**

 


