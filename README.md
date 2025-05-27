# Passo a Passo: Criar e Configurar uma Máquina Virtual Windows no Azure

## 1. Acesse o Portal Azure
- Entre no site: [https://portal.azure.com](https://portal.azure.com)
- Faça login com sua conta Microsoft.

## 2. Inicie a Criação da Máquina Virtual
1. No menu à esquerda, clique em **"Máquinas Virtuais"**.
2. Clique em **"Adicionar"** > **"Máquina virtual"**.

## 3. Configure as Informações Básicas
Preencha os campos obrigatórios:
- **Assinatura**: selecione sua assinatura.
- **Grupo de recursos**: escolha um existente ou clique em "Criar novo".
- **Nome da máquina virtual**: dê um nome identificável à sua VM.
- **Região**: escolha a localização (ex: Brazil South).
- **Imagem**: selecione **Windows Server** (ex: Windows Server 2022 Datacenter).
- **Tamanho**: clique em "Alterar tamanho" e escolha conforme a necessidade.
- **Usuário e Senha**: defina um nome de usuário e senha forte para acesso via RDP.
- **Portas de entrada públicas**: marque **Permitir portas selecionadas** e escolha **RDP (3389)**.

Clique em **Avançar: Discos >** para a próxima etapa.

## 4. Configure o Disco
- Selecione o tipo de disco do SO (SSD recomendado para melhor performance).
- Personalize discos adicionais, se necessário.

Clique em **Avançar: Rede >**.

## 5. Configure a Rede
- Por padrão, será criada uma nova rede virtual e um novo endereço IP público para a VM.
- Mantenha as configurações padrão, a menos que tenha necessidades específicas.

Clique em **Avançar** até chegar em **Revisar + criar**.

## 6. Revisar e Criar
- Revise todas as configurações.
- Clique em **Criar**.
- Aguarde o Azure provisionar a máquina virtual (pode levar alguns minutos).

## 7. Acessar a Máquina Virtual Windows
1. Após a implantação, vá para a página da VM recém-criada.
2. No painel superior, clique em **"Conectar"** > **"RDP"**.
3. Baixe o arquivo `.rdp` e abra-o.
4. Insira o usuário e senha definidos na criação.

## 8. Primeiros Passos Após o Acesso
- Atualize o Windows (Windows Update).
- Instale softwares e configure regras de firewall adicionais se necessário.
- Faça backup da VM, se for importante.

---

## Dicas de Segurança
- Altere a senha periodicamente.
- Considere utilizar regras de grupo de segurança de rede (NSG) para restringir o acesso ao RDP por IP.
- Mantenha o sistema operacional sempre atualizado.
