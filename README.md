

Criando uma Máquina Virtual na Azure ☁️🖥️
Descrição
Este projeto tem como objetivo demonstrar **como criar uma Máquina Virtual (VM) no Microsoft Azure**.  
Através deste guia, você aprenderá os passos essenciais para configurar uma VM do zero, utilizando o Azure Portal.
Tecnologias e Ferramentas
- Microsoft Azure Portal
- Azure CLI (opcional)
- Visual Studio Code (opcional)
- PowerShell ou Bash (opcional)
  Passo a Passo
 1. Acessar o Azure Portal
- Acesse: [https://portal.azure.com](https://portal.azure.com)
- Faça login com sua conta Microsoft.

 2. Criar uma Nova Máquina Virtual
- No painel do Azure, clique em **"Criar um recurso"** > **"Computação"** > **"Máquina Virtual"**.
- Preencha as informações básicas:
  - **Assinatura**: Escolha sua assinatura ativa.
  - **Grupo de Recursos**: Crie um novo ou selecione um existente.
  - **Nome da VM**: Ex.: `minhaVMExemplo`
  - **Região**: Escolha a mais próxima (ex.: `Brazil South`).
  - **Imagem**: Escolha o sistema operacional (ex.: `Ubuntu 20.04 LTS` ou `Windows Server`).
  - **Tamanho**: Selecione o tamanho de acordo com seu uso (B1s é uma opção gratuita no período de avaliação).
  - **Usuário e Senha**: Defina as credenciais para acesso.

3. Configurações de Rede
- **IP público**: Criar novo.
- **Portas de entrada**: Permitir `SSH` (Linux) ou `RDP` (Windows).

 4. Revisar e Criar
- Clique em **"Revisar + Criar"** para validar as configurações.
- Depois, clique em **"Criar"** e aguarde a implantação.

5. Acessar a Máquina Virtual
- Após criada, acesse pelo:
  - SSH(Linux):
    ```bash
    ssh usuario@ip-publico
    ```
  - RDP (Windows):  
    Baixe o arquivo `.rdp` fornecido e conecte usando seu usuário e senha.

 Estrutura do Projeto

```
/azure-vm-creation
│
├── screenshots/            # Prints das etapas no Azure Portal
├── scripts/                 # Scripts de criação por CLI (em breve)
└── README.md                # Este arquivo
```

 Objetivos de Aprendizado

- Criar uma VM usando o Microsoft Azure Portal.
- Compreender configurações básicas de rede e segurança.
- Acessar e gerenciar a máquina virtual criada.

 Autor

gabriel

