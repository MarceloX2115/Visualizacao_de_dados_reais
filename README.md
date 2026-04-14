# Desafios de Refatoração Estatística e Visual 📊

Este projeto apresenta a refatoração de três visualizações de dados baseadas no dataset *Students Performance in Exams*. O objetivo foi corrigir problemas de design e comunicação estatística utilizando princípios de especialistas como Edward Tufte e Cleveland-McGill.

## 🎯 Objetivo da Atividade

Identificar falhas de design em gráficos Python (Seaborn/Matplotlib) e aplicar melhorias focadas em:
- **Data-Ink Ratio:** Eliminar ruído e elementos que não trazem informação.
- **Eficácia Visual:** Melhorar a comparação entre grupos e a perceção de densidade.
- **Honestidade Estatística:** Evitar distorções na interpretação dos dados.

---

## 🛠️ Refatorações Realizadas

### 1. Distribuição por Etnia (Sobrecarga Visual)
* **Problemas:** Uso redundante de cores e falta de ordenação lógica entre as categorias.
* **Melhoria:** Implementação de um `boxplot` ordenado pela mediana com paleta monocromática, facilitando o ranking visual de desempenho.

### 2. Correlação Matemática vs. Leitura (Sobreposição)
* **Problemas:** *Overplotting* (pontos sobrepostos) que impedia identificar a real concentração de alunos.
* **Melhoria:** Uso de `jointplot` com `hexbin` para mostrar a densidade através da intensidade da cor, além de incluir distribuições marginais.

### 3. Curso de Preparação (Gráfico de Pizza)
* **Problemas:** Uso de gráfico de pizza para comparar médias e simplificação excessiva dos dados.
* **Melhoria:** Substituição por um gráfico de barras agrupado, permitindo comparar o impacto do curso detalhadamente por cada disciplina.

---

## 💻 Tecnologias
- **Linguagem:** Python
- **Bibliotecas:** Pandas, Seaborn, Matplotlib

---
*Este projeto foi desenvolvido para exercitar a capacidade crítica na criação de dashboards e relatórios de dados.*
