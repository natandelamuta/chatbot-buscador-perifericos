# Chatbot Buscador de Periféricos

Um chatbot interativo que utiliza a IA do Google Gemini para ajudar usuários a encontrar informações e preços de periféricos de computador.

## 📝 Sobre o Projeto

Este projeto consiste em um chatbot conversacional projetado para atuar como um assistente virtual na busca por periféricos de notebooks e PCs (como mouses, teclados, monitores, etc.). A interação com o usuário é impulsionada pelo poder do modelo de linguagem **Google Gemini**, garantindo respostas fluidas e naturais.

Para manter o chatbot focado em seu objetivo principal e evitar desvios de escopo, foi implementado um "roteiro" (através de técnicas de *prompt engineering*). Esse roteiro guia a IA para que ela se atenha à tarefa de buscar periféricos, tornando a conversa mais eficiente e direta.

A concepção original do projeto previa a utilização de uma API pública para consultar preços em tempo real. Devido à falta de uma API gratuita e robusta para essa finalidade, foi desenvolvido um **módulo de dados fictício**. Este módulo simula o comportamento de uma API real, permitindo que o chatbot demonstre toda a sua funcionalidade de consulta e apresentação de dados de forma eficaz.

## ✨ Funcionalidades

-   **Busca Conversacional:** Interaja com o chatbot usando linguagem natural.
-   **Foco Específico:** Especializado na busca por periféricos de notebooks e computadores.
-   **Inteligência Artificial com Gemini:** Respostas geradas pelo modelo de IA do Google.
-   **Conversa Guiada:** Um sistema de roteiro interno mantém a conversa no tópico.
-   **Simulação de API:** Demonstração funcional com um banco de dados fictício que simula uma consulta externa.

## 🚀 Tecnologias Utilizadas

-   **Linguagem Principal:** Python
-   **Modelo de IA:** Google Gemini API
-   **Bibliotecas:** (Adicione aqui as bibliotecas que você usou, como `google-generativeai`, `os`, etc.)

## ⚙️ Como Funciona

O fluxo de interação do chatbot pode ser resumido da seguinte forma:

1.  O usuário envia uma mensagem consultando um periférico.
2.  A aplicação combina a mensagem do usuário com um prompt pré-definido (o "roteiro").
3.  Este prompt completo é enviado para a API do Gemini.
4.  O Gemini processa a informação e gera uma resposta, identificando a intenção do usuário.
5.  O chatbot interpreta a resposta da IA e consulta sua base de dados **fictícia** para obter as informações do produto (preço, especificações, etc.).
6.  Finalmente, o chatbot formata e entrega a resposta final ao usuário.
