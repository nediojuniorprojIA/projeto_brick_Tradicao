# 🪑 Brick Tradição - Catálogo Digital e Triagem Inteligente

![Bubble](https://imgshields.io/badge/Bubble.io-Primary?style=for-the-badge&logo=bubble&color=000000)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![API REST](https://img.shields.io/badge/API_REST-ViaCEP-2CA5E0?style=for-the-badge)

## 📖 Sobre o Projeto
O **Brick Tradição** é uma aplicação web desenvolvida para digitalizar o catálogo de produtos e automatizar o atendimento de um comércio local de móveis da região do Vale do Sinos (RS). O projeto foca em oferecer uma experiência de e-commerce acessível, responsiva e dinâmica, conectando o cliente diretamente ao setor de vendas de forma otimizada via WhatsApp.

---

## 🎓 Contexto Acadêmico
- **Instituição:** UniFECAF
- **Disciplina:** Padrões Web para No Code e Low Code
- **Desafio:** Personalização e Integração Web: Criando Experiências Visuais com No Code e Web Standards.

---

## 🚀 Funcionalidades Principais

- **Vitrine Dinâmica (Cards):** Catálogo de móveis gerado a partir de um banco de dados relacional, exibindo foto, nome, descrição e preço com formatação visual uniforme.
- **Autocompletar de Endereço:** Integração com banco de dados externo (ViaCEP) que preenche os campos de Rua, Bairro e Cidade instantaneamente.
- **Triagem de Frete Condicional:** Sistema que analisa a cidade do cliente e define, em tempo real, se a entrega é gratuita (Novo Hamburgo e São Leopoldo) ou se há cobrança de taxa de deslocamento.
- **Integração com WhatsApp:** Ação de redirecionamento (*Deep Link*) que envia o cliente para o aplicativo de mensagens com um texto pré-formatado, incluindo dados do endereço.

---

## 🛠️ Tecnologias e Padrões Web Utilizados

Este projeto foi construído utilizando a plataforma No-Code **Bubble.io**, aprimorada através da inserção manual de *Web Standards*:

- **CSS3 (Cascading Style Sheets):** Aplicação de pseudo-classes (`:hover`) e transições injetadas via elemento HTML para criar efeitos visuais interativos nos cartões.
- **HTML5 Embed:** Incorporação responsiva de um `iframe` do Google Maps para geolocalização.
- **APIs RESTful:** Consumo de API em formato JSON para automação de dados geográficos.
- **Flexbox (Responsividade):** Uso de *containers* flexíveis, margens dinâmicas (`gap`) e quebra automática de linha (`Wrap`) para adaptação *Mobile-First*.

### Exemplo de CSS Injetado no Projeto
```css
<style>
  [id="card-movel"] {
    transition: transform 0.3s ease, box-shadow 0.3s ease !important;
  }
  [id="card-movel"]:hover {
    transform: translateY(-5px) !important;
    box-shadow: 0 10px 20px rgba(0,0,0,0.15) !important;
    cursor: pointer !important;
  }
</style>

