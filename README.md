<div align="center">
  
# 🤖Classificador MNINT👾

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![typescript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![jest](https://img.shields.io/badge/Jest-C21325?style=for-the-badge&logo=jest&logoColor=white)
![tensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)

</div>

Esta aplicação permite ao usuário desenhar um número na tela, e utiliza Inteligência Artificial para tentar adivinhar qual foi o número desenhado. O projeto faz uso de um classificador baseado no dataset MNIST, um modelo de aprendizado de máquina amplamente utilizado para reconhecer dígitos manuscritos em imagens.

> [Acesse a aplicação aqui.](https://mnist-classifier-eight.vercel.app/)

## 🎯 Objetivos

Este projeto integra um conjunto de iniciativas voltadas para o aprendizado em Inteligência Artificial. O foco principal é o desenvolvimento de competências em deep learning, e os objetivos a seguir refletem as metas já alcançadas e as que ainda estão em progresso:

- [x] Desenvolvimento de uma inteligência artificial funcional;
- [x] Elaboração de scripts e manipulação de datasets para aprendizado de máquina;
- [x] Implementação de rotas de comunicação entre a API e a IA;
- [x] Exploração da comunicação entre diferentes aplicações utilizando linguagens distintas;
- [x] Geração de imagens no frontend utilizando o Canvas;
- [x] Aprendizado sobre o envio de imagens via HTTP;

## 🏗️ Estrutura do Projeto

O projeto está organizado em três aplicações distintas, cada uma com uma responsabilidade específica:

### Frontend

Esta aplicação, desenvolvida em React, é responsável pela interface com o usuário e pela integração com as demais partes do projeto. Utiliza o Canvas para renderizar o componente de lousa, permitindo ao usuário desenhar livremente. Toda a lógica de interação é gerenciada via Context API. A imagem desenhada é convertida para o formato .png e enviada ao backend, que retorna a previsão do número reconhecido pelo modelo de IA, exibindo ao usuário o resultado mais provável.

> [Ver repositório](https://github.com/felipe-sant/FRONT-MNIST_Classifier)

### Backend

Esta camada, construída com Express, faz a ponte entre o usuário e a Inteligência Artificial. Sua principal função é intermediar a comunicação, recebendo as imagens do frontend por meio da rota `api/ia/predict` via método `POST` e encaminhando-as para o serviço de IA. Dessa forma, ela traduz as requisições entre o frontend e a camada de inteligência artificial, garantindo o fluxo correto de informações entre ambas.

> [Ver repositório](https://github.com/felipe-sant/BACK-MNIST_Classifier)

### Inteligência Artificial (AI)

Nesta aplicação, foi utilizado TensorFlow para o desenvolvimento do modelo de IA, o dataset MNIST para treinamento e validação, e FastAPI para expor os endpoints de comunicação. O projeto conta com três scripts principais: um para criação e treinamento do modelo, outro para testes e um terceiro para definição das rotas de comunicação. Ao receber uma imagem do backend, a aplicação utiliza o modelo treinado para prever qual número foi desenhado, retornando ao backend o valor com a maior probabilidade.

> [Ver repositório](https://github.com/felipe-sant/AI-MNIST_Classifier)

<hr>

<div align="center">
    developed by <a href="https://github.com/felipe-sant?tab=followers">@felipe-sant</a>
</div>
