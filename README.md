# Previsão da Demanda de Bicicletas Compartilhadas: Uma Abordagem Comparativa entre Modelos Lineares Regularizados e Algoritmos Baseados em Árvores de Decisão

Trabalho Final Individual apresentado à disciplina **Fundamentos e Ferramentas de Ciência de Dados (FFCD)**  
Programa de Pós-Graduação em Ciência de Dados — **Universidade Federal do Paraná (UFPR)**  
**Autor:** Pedro Henrique Barbosa  
**Docente Responsável:** Prof. Paulo Moreira  

---

## 📌 Descrição do Estudo
Este projeto investiga a capacidade preditiva da demanda horária de empréstimos utilizando o *Bike Sharing Dataset* (17.379 observações do Capital Bikeshare de Washington D.C., período 2011–2012). Sob a ótica do ciclo analítico de Ciência de Dados (*Explore, Refine, Model, Evaluate, Produce*) e do protocolo de integridade científica **REFORMS**, compara-se o desempenho de modelos lineares com regularização (Ridge e Lasso) com algoritmos não lineares em árvore (Random Forest e LightGBM).

## 🚀 Principais Resultados
* **Melhor Modelo:** LightGBM ($R^2 = 0,938$, $\text{MAE} = 26,1$ bicicletas/hora, $\text{RMSE} = 42,8$).
* **Redução de Erro:** Redução de 74% no erro absoluto em relação aos modelos lineares regularizados.
* **Padrões de Uso:** Identificação de comportamento bimodal em dias úteis (picos às 08:00 e 17:00–18:00) vs. perfil unimodal suave nos fins de semana (12:00 às 16:00).
* **Interpretabilidade (SHAP):** Hierarquia de sensibilidade dominada pelas componentes periódicas da hora do dia, seguida por temperatura ambiente, calendário de trabalho e umidade relativa.

## 🛠️ Como Reproduzir
1. Clone este repositório:
```bash
git clone https://github.com/pedro-h-barbosa/bike-sharing-ffcd-ufpr.git
cd bike-sharing-ffcd-ufpr
