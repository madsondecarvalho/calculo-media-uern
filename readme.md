# Calculadora de Média Acadêmica - UERN 🎓

Aplicação web simples (*Single Page Application*) desenvolvida para automatizar o cálculo de médias parciais e finais, seguindo rigorosamente as normas estatutárias da **Resolução Nº 01/2022 - CONSUNI** da Universidade do Estado do Rio Grande do Norte (UERN).

## 📋 Funcionalidades

- **Seleção Dinâmica de Créditos:** Alterna automaticamente a interface e a fórmula de cálculo entre disciplinas de 02 créditos e 03 ou mais créditos.
- **Cálculo de Média Ponderada (MP):**
  - *3 ou mais Créditos:* (A1×4 + A2×5 + A3×6) / 15.
  - *2 Créditos:* (A1×4 + A2×5) / 9.
- **Arredondamento Oficial:** Implementa a regra de arredondamento para uma casa decimal conforme o Art. 146.
- **Análise de Situação:** Identifica instantaneamente se o discente está **Aprovado**, em **Exame Final** ou **Reprovado**.
- **Cálculo de Necessidade para Final:** Caso o aluno fique em exame, o sistema calcula a nota exata necessária no Exame Final (EF) para atingir a Média Final 6.0.

## ⚖️ Regras de Negócio Implementadas

O algoritmo (“Core Business Logic”) foi desenvolvido baseando-se nos seguintes artigos da Resolução Nº 01/2022:

| Artigo | Descrição da Regra |
| :--- | :--- |
| **Art. 142** | Define pesos 4, 5 e 6 para disciplinas de 03 ou mais créditos. |
| **Art. 143** | Define pesos 4 e 5 para disciplinas de 02 créditos (sem nota A3). |
| **Art. 144** | Estabelece que MP >= 4.0 e < 7.0 leva a Exame Final. |
| **Art. 145** | Define que a aprovação pós-final exige Média Final >= 6.0 (`MF = (MP + EF) / 2`). |
| **Art. 146** | Determina o arredondamento da segunda casa decimal para manter apenas uma casa. |

## 🚀 Como Executar

Este projeto não requer instalação de dependências (npm, node, etc). É uma aplicação estática pura.

1. Baixe o arquivo `index.html`.
2. Dê um duplo clique para abrir em qualquer navegador moderno (Google Chrome, Firefox, Edge, Safari).

## 🛠️ Tecnologias Utilizadas

- **HTML5:** Estrutura semântica.
- **CSS3:** Estilização limpa, responsiva e uso de variáveis (CSS Variables) para facilitar manutenção.
- **JavaScript (Vanilla):** Manipulação do DOM e lógica matemática sem uso de frameworks externos.

## 👤 Autor

Desenvolvido por **Madson Gustavo Fagundes Pinto de Carvalho**.
*Discente do curso Tecnólogo em Sistemas para Internet - UERN.*

---
*Projeto de código aberto para fins de produtividade acadêmica.*