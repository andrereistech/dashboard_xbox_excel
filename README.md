# 🎮 Dashboard de Análise de Vendas e Assinaturas - Xbox Game Pass

![Xbox Header](https://img.shields.io/badge/Xbox-Game%20Pass-107C41?style=for-the-badge&logo=xbox&logoColor=white)
![Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)

Este projeto consiste na construção de um Dashboard Executivo e Interativo no Microsoft Excel para análise de desempenho de vendas, receita e engajamento dos planos de assinatura do **Xbox Game Pass**. 

O projeto foi desenvolvido aplicando a metodologia estrutural **ABCDE** de organização de planilhas empresariais.

---

## 👥 Mentor & Autoria

* **Mentoria:** Felipe Aguiar (o Felipão)
  * **LinkedIn:** (https://www.linkedin.com/in/felipeaguiar-exe)
  * **Instagram** (https://www.instagram.com/felipeaguiar.exe)

* **Autor:** André Reis
  * **LinkedIn:** (https://www.linkedin.com/in/andre-reis-tech)
  * **GitHub:** (https://github.com/andrereistech)
  * **Instagram** (https://www.instagram.com/reis_dadosetech)

---

## 🏗️ Metodologia de Organização (Método ABCDE)

Para garantir uma arquitetura limpa, escalável e de fácil manutenção, a pasta de trabalho foi dividida em 5 abas padronizadas:

1. **`A` - Assets (Oculta):** Contém os elementos visuais do projeto, incluindo a paleta de cores oficial (tons de verde Xbox `#9BC848`, `#22C55E`, `#2AE6B1`, `#5BF6A8` e neutros para apoio `#E8E6E9`), logos, ícones e referências de layout.
2. **`B` - Bases (Oculta):** Contém a base de dados consolidada com as transações dos assinantes (ID, Nome, Plano, Data de Início, Auto Renovação, Valores, Passes de Temporada EA/Minecraft e Cupons).
3. **`C` - Cálculos (Oculta):** Contém as Tabelas Dinâmicas e fórmulas de apoio para estruturação das métricas cruciais e respostas às perguntas de negócio.
4. **`D` - Dashboard (Visível):** A tela executiva final projetada para a tomada de decisão do gestor, contendo visuais, cartões de KPI e Segmentadores de Dados (Slicers) interativos.
5. **`E` - Extras (Oculta):** Reservada para documentações complementares, versionamento ou dados adicionais de suporte.

---

## 📊 Pergunta de Negócio e Principais Achados (Aba Cálculos)

Abaixo estão as respostas técnicas desenvolvidas na aba de **Cálculos** para suporte ao gestor:

* **Pergunta 1 & 2: Qual o faturamento total e a separação por Auto Renovação (Yes/No) para os Planos Anuais/Trimestrais?**
  * *Plano Anual:* Total de R$ 1.754 (R$ 1.537 com Auto Renovação ligada vs. R$ 217 sem Auto Renovação).
  * *Plano Trimestral (Quarterly):* Total de **R$ 2.308** (R$ 1.502 com Auto Renovação vs. R$ 806 sem Auto Renovação).
* **Pergunta 3: Total de Vendas de Assinaturas do EA Play Season Pass?**
  * **R$ 990,00** acumulados exclusivamente pelos clientes do plano **Ultimate** (100% da receita de EA Play vem de usuários Ultimate).
* **Pergunta 4: Total de Vendas do Minecraft Season Pass?**
  * **R$ 1.140,00** (divididos entre R$ 480,00 no plano **Standard** e R$ 660,00 no plano **Ultimate**).

---

## ⚙️ Configurações Utilizadas na Planilha e no Dashboard

* **Ocultação de Abas de Apoio:** As abas `Assets`, `Bases`, `Cálculos` e `Extras` foram mantidas ocultas para proteger as regras de negócio e evitar edições acidentais por usuários finais.
* **Tabelas Dinâmicas Desconectadas do Layout:** Toda a inteligência de agregação fica isolada na aba `Cálculos`, e os gráficos do `Dashboard` consomem essas estruturas organizadas.
* **Segmentação de Dados (Slicers):** Conexão dos filtros interativos às tabelas dinâmicas para permitir navegação por tipo de plano, período ou status de renovação automática.
* **Formatação Condicional e Estilização:** Aplicação de cores dinâmicas alinhadas à identidade visual do Xbox para destacar métricas positivas e zonas de atenção.
* **Proteção e Linhas de Grade:** Desativação de cabeçalhos e linhas de grade na aba `Dashboard` para dar um aspecto de aplicação web/software executivo.

---

## 🛠️ Instruções para Reprodução e Uso

1. Faça o clone ou download deste repositório:
   ```bash
   git clone [https://github.com/seu-usuario/xbox-game-pass-dashboard.git](https://github.com/seu-usuario/xbox-game-pass-dashboard.git)
