# Gerenciador de Pedidos Automatizado no Google Sheets

Este é um projeto de automação desenvolvido em Google Apps Script para otimizar o controle de pedidos de uma plataforma de entregas. A planilha automatizada organiza informações como entregadores, formas de pagamento e plataformas utilizadas, aplicando validações de dados e formatações dinâmicas para facilitar a visualização e o acompanhamento dos pedidos.

---

## 🎯 **Objetivo**
Criar uma ferramenta eficiente e prática para gerenciar pedidos, automatizando tarefas repetitivas e melhorando a organização dos dados, especialmente em operações que lidam com alta demanda e diversas plataformas.

---

## 🎨 Layout do Aplicativo

Segue abaixo uma visualização do layout do aplicativo:

![CONTOLE LAYOUT](CONTROLE%20LAYOUT.png)

---

## 🚀 **Funcionalidades**
1. **Atualização automática de horário:**
   - Preenche automaticamente a coluna "HORÁRIO" com o dia e a hora de criação do pedido, desde que todas as colunas críticas (entregador, pagamento e plataforma) estejam preenchidas.

2. **Criação automática de abas mensais:**
   - Gera automaticamente uma nova aba para cada mês, formatada e preparada com os cabeçalhos necessários.

3. **Validação de dados:**
   - Restringe as entradas nas colunas relevantes, permitindo apenas valores pré-definidos para evitar erros de digitação e inconsistências.

4. **Formatação condicional com cores:**
   - Aplica cores distintas às células de acordo com os valores inseridos:
     - **Pagamento:** Cartão (azul claro), Pago (verde claro), Dinheiro (vermelho).
     - **Plataforma:** iFood (vermelho claro), App Yok (amarelo claro), TEL (laranja claro).

5. **Foco na última célula editada:**
   - Move o foco automaticamente para a última célula editada ao abrir a planilha, facilitando a continuidade do trabalho.

6. **Backup automatizado de abas:**
   - Abas do **ano atual** são movidas automaticamente para um arquivo de backup específico do ano, com exceção da aba do mês atual, que permanece na planilha principal.

7. **Proteção da estrutura da planilha:**
   - Protege automaticamente as abas contra edições acidentais, mantendo a integridade do formato.

---

## 🛠️ **Tecnologias Utilizadas**
- **Google Apps Script:** Para desenvolver as funcionalidades de automação e manipulação da planilha.
- **Google Sheets:** Como interface de entrada de dados e exibição das informações organizadas.

---

## 🗂️ **Processo de Desenvolvimento**
O desenvolvimento deste projeto seguiu as seguintes etapas:

1. **Identificação de Requisitos:**
   - Mapear as principais necessidades da operação, incluindo a organização por mês, validação de dados e rastreamento eficiente de informações.

2. **Prototipação:**
   - Criar uma estrutura inicial da planilha, definindo os cabeçalhos e os fluxos básicos de dados.

3. **Automação com Google Apps Script:**
   - Implementar scripts para as seguintes funcionalidades:
     - Preenchimento automático de horários.
     - Validações de dados em colunas específicas.
     - Criação dinâmica de abas mensais com formatações e proteções aplicadas.
     - Aplicação de cores personalizadas para melhorar a leitura.
     - Movimentação automatizada de abas do ano atual para arquivos de backup organizados por ano.

4. **Melhorias e Ajustes:**
   - Adicionar lógica para salvar e restaurar o foco na última célula editada.
   - Refatorar o código para maior modularidade e clareza.
   - Testar as funcionalidades com dados reais, garantindo precisão e estabilidade.

5. **Documentação:**
   - Preparar este arquivo `README` para explicar o funcionamento e o propósito do projeto.

---

## 📂 **Como Usar**
1. **Configuração Inicial:**
   - Copie o código para o editor de Apps Script vinculado à sua planilha no Google Sheets.
   - **Personalize os valores das validações de dados no código:**
     - Altere a lista de entregadores, formas de pagamento e plataformas no script para refletir as necessidades específicas da sua operação.
   - Salve e ative os gatilhos de execução automática (`onEdit` e `onOpen`).

2. **Utilização:**
   - Insira dados na planilha seguindo os valores válidos para cada coluna.
   - Observe o preenchimento automático de horários e a aplicação de cores com base nos valores.

3. **Backup Automatizado:**
   - No início de cada mês, abas do ano atual (exceto a do mês atual) serão movidas automaticamente para um arquivo de backup dedicado, garantindo organização e espaço na planilha principal.

---

## 📈 **Possíveis Melhorias Futuras**
- Implementação de gráficos automáticos para análise de desempenho.
- Integração com APIs externas, como iFood, para sincronização de pedidos.
- Relatórios automáticos ao final de cada mês, exportados em formato PDF.

---

## 📝 **Licença**
Este projeto é open-source e está disponível sob a licença MIT. Sinta-se à vontade para modificar e adaptar conforme suas necessidades.

---

## 📬 **Contato**
Para dúvidas ou sugestões, entre em contato:
- **Autor:** Carlos
- **Linkedin** [linkedin](https://www.linkedin.com/in/carlos-nogueira-80b47b96)
- **E-mail:** [carloshhnai@gmail.com]
