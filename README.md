# 🗄️ Banco de Dados SQL no Azure - Documentação Técnica e Anotações

Este repositório tem como objetivo documentar o processo de criação, configuração e gerenciamento de uma instância de **banco de dados SQL na plataforma Microsoft Azure**. Além disso, reúne anotações, dicas práticas e conceitos fundamentais relacionados à computação em nuvem com foco em **bancos de dados como serviço (DBaaS)**.

---

## 🎯 Objetivos

- Praticar a criação de uma instância gerenciada de SQL no Azure.
- Aplicar conceitos aprendidos em um ambiente real.
- Registrar de forma clara os passos técnicos envolvidos.
- Criar um material de apoio útil para estudos futuros e possíveis projetos profissionais.
- Utilizar o GitHub como ferramenta de versionamento e portfólio técnico.

---

## 🧠 Conceitos Envolvidos

- **DBaaS (Database as a Service)**: Modelo onde o provedor gerencia toda a infraestrutura e você foca apenas nos dados.
- **Instância Gerenciada de SQL**: Ambiente pronto no Azure para rodar SQL Server com alta disponibilidade, segurança e escalabilidade.
- **Provisionamento e Configuração**: Etapas práticas para criar, proteger e acessar o banco de dados.
- **Conectividade Segura**: Autenticação via credenciais e configuração de firewall no Azure.

---

## 🛠️ Requisitos

- Conta ativa na plataforma [Azure Portal](https://portal.azure.com/)
- Navegador moderno atualizado
- Ferramentas para conexão (como **SQL Server Management Studio (SSMS)** ou **Azure Data Studio**)
- Git instalado e conta no GitHub (para documentação técnica)

---

## 📌 Etapas da Criação da Instância SQL no Azure

### 1. Acessar o Portal do Azure

- Faça login no [Azure Portal](https://portal.azure.com/)
- No menu lateral, procure por **SQL Database** ou **Banco de Dados SQL**
- Clique em **Criar**

📷 *![Portal SQL: ](/images/1-portal-sql.png)*

---

### 2. Preencher os Dados da Instância

- Selecione um grupo de recursos (ou crie um novo)
- Escolha um nome para o banco de dados
- Defina o servidor (crie um se necessário, com usuário e senha)
- Região: escolha a mais próxima (ex: Brazil South)

📷 *![Configuração](/images/2-configuracao.png)*

---

### 3. Selecionar Plano e Camada de Preço

- Para testes, pode-se escolher a camada **Gratuita** (quando disponível) ou **Basic**
- Escolher o tamanho da instância de acordo com sua necessidade (DTUs ou vCores)

📷 *![Seleção de Plano](/images/3-plano.png)*

---

### 4. Configurar Regras de Firewall

- Permitir acesso ao IP atual
- Opcional: permitir outras faixas de IP ou uso interno (VNet)

📷 *![Firewall](/images/4-firewall.png)*

---

### 5. Criar e Conectar

- Clique em **Revisar + Criar**
- Após a implantação, acesse os dados de conexão e configure seu cliente (SSMS, Azure Data Studio etc.)

---

## 🧾 Notas e Dicas

- Salve as credenciais e **NUNCA** compartilhe publicamente o `string de conexão` completo.
- Em ambientes de produção, utilize **Azure Key Vault** para guardar credenciais.
- Use **firewalls restritivos e autenticação multifator** sempre que possível.
- A instância gerenciada tem suporte à replicação, backups automáticos e alta disponibilidade integrada.
- Utilize **Monitoramento (Azure Monitor)** para acompanhar métricas de desempenho.

---

## 📁 Estrutura do Repositório

📦 azure-sql-study
┣ 📂 images
┃ ┣ 📜 1-portal-sql.png
┃ ┣ 📜 2-configuracao.png
┃ ┣ 📜 3-plano.png
┃ ┣ 📜 4-firewall.png
┃ ┗ 📜 5-finalizacao.png
┣ 📜 README.md
┗ 📜 anotações.md

---

## 📚 Referências e Leitura Recomendada

- [Documentação Oficial do Azure - SQL Database](https://learn.microsoft.com/pt-br/azure/azure-sql/database/sql-database-overview)
- [SQL Server Management Studio (SSMS)](https://aka.ms/ssms)
- [Azure Data Studio](https://learn.microsoft.com/pt-br/sql/azure-data-studio/)

---

## ✍️ Autor

**Felipe**  
Estudante de Análise e Desenvolvimento de Sistemas  
Apaixonado por desenvolvimento full-stack, infraestrutura e tecnologia em nuvem.

---

> “Documentar é programar em voz alta: sua experiência pode ser útil para você e para muitos outros.
