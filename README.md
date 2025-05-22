# Desafio DIO – Criação e Configuração de Máquina Virtual no Azure

## 🔍 Entendendo o Desafio
Este repositório documenta o **processo de criação e configuração de uma Máquina Virtual (VM)** na plataforma Microsoft Azure, aplicando os conceitos vistos no bootcamp “XP Inc. - Cloud com Inteligência Artificial”.

## 🎯 Descrição do Desafio
- Criar uma VM no Azure usando o **Portal** (sem pular etapas).   
- Entregar tudo em um repositório público no GitHub, com:  

> **Referência oficial**:  
> [Criar uma máquina virtual Windows no portal do Azure](https://learn.microsoft.com/pt-br/azure/virtual-machines/windows/quick-create-portal)

## 📝 Objetivos de Aprendizagem
- Aplicar conceitos de nuvem em um cenário prático.  
- Documentar processos técnicos de forma clara e estruturada.  
- Usar o GitHub como ferramenta de versionamento e compartilhamento.

## ⚙️ Ferramentas e Tecnologias
- **Microsoft Azure Portal**  
- **Azure CLI** (opcional)  
- **Visual Studio Code**  
- **Git & GitHub**  
- **Markdown** para documentação  

## 🚀 Passo a Passo Executado

1. **Login no Azure Portal**  
   - Acesse https://portal.azure.com e faça login com sua conta.

2. **Criação do Resource Group**  
   - Nome: `rg-desafio-vm`

3. **Criação da Máquina Virtual**  
   - Menu: **Máquinas Virtuais → + Adicionar → Máquina Virtual**  
   - **Basics**  
     - Nome da VM: `vm-desafio-dio`  
     - Região: `Brazil South`  
     - Imagem: `Windows 11 Pro`, `Windows Server` ou `Ubuntu Server` 
     - Tamanho: `Standard_B1s` (1 vCPU, 1 GiB RAM)  
     - Autenticação: usuário `azureuser` + senha forte (Windows) / chaves SSH (Linux)  
   - **Discos**  
     - Tipo de disco padrão  
   - **Networking**  
     - IP Público: habilitado  
     - Porta: **RDP (3389)** aberta (Windows) / **SSH (22)** (Linux)  

4. **Revisão e Criar**  
   - Revise todas as configurações e clique em **Criar**.

5. **Conexão e Testes**  
   - Acesse via **RDP** (Windows) ou **SSH** (Linux).
