# Fluxograma e Dados Curriculares - Bacharelado em Física  
**Centro Acadêmico de Física – UFCG**

Este repositório mantém os **dados estruturados e oficiais** do fluxograma do curso de **Bacharelado em Física** do Centro de Ciências e Tecnologia (CCT) da Universidade Federal de Campina Grande (UFCG).

Os arquivos JSON foram extraídos, organizados e validados a partir do documento oficial **PPC_FLUXO-Bacharelado-Revisado.pdf** (versão revisada 2026), com o objetivo de apoiar:

- o acompanhamento curricular pelos estudantes
- o desenvolvimento de ferramentas digitais (sites, aplicativos, planilhas de progresso)
- a atualização contínua das informações pelo Centro Acadêmico

## Conteúdo do repositório

| Arquivo                          | Descrição                                                                 |
|----------------------------------|---------------------------------------------------------------------------|
| `metadata.json`                  | Informações gerais do curso: cargas horárias totais, mínimos exigidos e regras curriculares |
| `obrigatorias.json`              | Disciplinas obrigatórias (1º ao 8º período), incluindo códigos, pré e co-requisitos, carga horária e créditos |
| `comp-obrigatorias.json`         | Disciplinas complementares obrigatórias (mínimo 16 créditos / 240 horas), com pré-requisitos |
| `comp-optativas.json`            | Disciplinas complementares optativas, organizadas por área de formação (I a VIII) |

**Carga horária total exigida** (conforme PPC revisado): **2640 horas**  
- Obrigatórias: 1860 horas  
- Complementares obrigatórias: 240 horas (mínimo 16 créditos)  
- Complementares optativas: 240 horas (mínimo 16 créditos)  
- Curriculares flexíveis: 300 horas  
- Extensão obrigatória: 260 horas  

**Integração curricular**: mínimo de 8 períodos, máximo de 12 períodos.

## Como usar os dados

Os arquivos são públicos e podem ser consumidos diretamente via URLs raw do GitHub.

Exemplo em JavaScript:
```js
const url = 'https://raw.githubusercontent.com/ca-fisica-ufcg/fluxograma-fisica-bacharelado-dados/main/obrigatorias.json';
fetch(url)
  .then(res => res.json())
  .then(data => console.log('Disciplinas obrigatórias:', data));