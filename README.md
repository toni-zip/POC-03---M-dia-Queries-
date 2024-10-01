# 🌐 Prova de Conceito - Media Queries 🌐

> Este projeto demonstra o uso de **Media Queries** no CSS para criar layouts responsivos, adaptados a diferentes tamanhos de tela e dispositivos.

---

## 📋 Descrição do Projeto

Esta Prova de Conceito (POC) foi desenvolvida para demonstrar a utilização de **Media Queries** no CSS, permitindo que a página web se ajuste automaticamente conforme o dispositivo utilizado pelo usuário, seja um smartphone, tablet ou desktop. O projeto é um exemplo prático de como adaptar o layout, utilizando HTML e CSS.

A página inclui uma interface simples, com elementos que se reorganizam e alteram o estilo dependendo do tamanho da tela ou da orientação do dispositivo.

## 🚀 Funcionalidades

- **Design Responsivo**: O layout adapta-se automaticamente para telas pequenas (smartphones), médias (tablets) e grandes (desktops).
- **Ajustes por Orientação**: O conteúdo muda de acordo com a orientação do dispositivo (retrato ou paisagem).
- **Compatibilidade com Impressão**: A página também possui um estilo específico para impressão, ocultando elementos desnecessários.

## 🎨 Layout

A estrutura do layout é composta por:

- **Cabeçalho e Navegação**: Inclui links de navegação ajustados conforme o dispositivo.
- **Banner de Boas-vindas**: Apresenta uma mensagem de introdução ao projeto.
- **Quadro de Imagens**: Exibe itens que se reorganizam conforme o tamanho da tela.
- **Conteúdo Informativo**: Explica o propósito da POC com responsividade.

### Exemplo de Estilo Dinâmico:
- No **desktop**, o quadro exibe quatro colunas.
- No **tablet**, o layout muda para duas colunas.
- Em **smartphones**, os itens são exibidos em uma única coluna.

---

## 🛠️ Tecnologias Utilizadas

- **HTML**: Estrutura da página.
- **CSS (Media Queries)**: Estilos responsivos que ajustam a apresentação da interface conforme o dispositivo.

---

## 🖥️ Como Funcionam as Media Queries

No arquivo CSS, utilizamos Media Queries para detectar a largura da tela e a orientação do dispositivo, aplicando estilos específicos para cada situação.

### Exemplo de Media Query para Tablet:

```css
@media (min-width: 601px) and (max-width: 900px) {

    header {
        background-color: var(--quadrocolortablet); 
    }

    .quadro {
        grid-template-columns: 1fr 1fr;
    }

    .conteudo {
        font-size: 16px;
    }

    footer {
        background-color: var(--quadrocolortablet);
    }

}
```

Neste exemplo, quando a largura da tela é de no máximo 900px (smartphones), o cabeçalho muda de cor, o layout do quadro é reorganizado em duas coluna e o tamanho da fonte é alterado.

### Exemplo de Media Query para Smartphone:

```css
@media (max-width: 600px) {
    header {
        background-color: var(--quadrocolormobile);
    }

    .quadro {
        grid-template-columns: 1fr;
    }

    .conteudo {
        font-size: 14px;
    }
}
```

Neste exemplo, quando a largura da tela é de no máximo 600px (smartphones), o cabeçalho muda de cor, o layout do quadro é reorganizado em uma única coluna e o tamanho da fonte é reduzido.

### Exemplo de Estilos para Impressão:

```css
@media print {
    header, nav, footer {
        display: none;
    }

    .conteudo {
        font-size: 10pt;
    }
}
```

Aqui, ao imprimir a página, o cabeçalho, navegação e rodapé são ocultados, enquanto o conteúdo principal recebe um ajuste no tamanho da fonte.

---

## 💻 Como Executar

1. Abra o arquivo `index.html` em um navegador.
2. Redimensione a janela ou use ferramentas de desenvolvedor para testar o comportamento responsivo em diferentes tamanhos de tela e orientações.
3. Use a opção de impressão do navegador para verificar o estilo específico de impressão.

---
Os resultado devem ser algo parecido com:
![Media_Querie_Desktop](https://github.com/user-attachments/assets/b2dcc000-7429-4907-97e0-9e1b29822ec6)
Para Desktop

![Midia_Querie_Tablet](https://github.com/user-attachments/assets/71103fe3-18bf-405c-a7d4-f5e471b09deb)
Para Tablets

![Midia_Querie_Smartphone](https://github.com/user-attachments/assets/a5222681-3179-4f6e-a721-cbae9c041a59)
Para Celulares

