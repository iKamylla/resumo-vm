# resumo-vm
Este repositório contém resumo e dicas práticas sobre o processo de criação e configuração de uma máquina virtual  na plataforma Microsoft Azure.

Criação e configuração de máquina virtual no Microsoft Azure
A criação de uma máquina virtual (VM) no Microsoft Azure permite executar sistemas operacionais e aplicativos em um ambiente baseado em nuvem, com flexibilidade de configuração, escalabilidade e segurança.

Durante o laboratório, pratiquei a criação e configuração de uma máquina virtual no Microsoft Azure, o que me permitiu entender melhor os serviços de infraestrutura em nuvem. O processo envolveu escolher o sistema operacional, tamanho da VM, autenticação e configurações de rede. Aprendi a importância de boas práticas, como configurar o desligamento automático para evitar cobranças, e usar grupos de segurança para proteger a VM. A experiência ajudou a consolidar conhecimentos sobre computação em nuvem e mostrou como o Azure pode ser uma ferramenta prática e acessível para simular ambientes reais de trabalho.

Etapas do Processo
  1 - Acessar o Portal Azure
    Entrar no site portal.azure.com com sua conta Microsoft.
  
  2 - Criar um Grupo de Recursos
    Um contêiner lógico que agrupa os recursos relacionados (como a VM, discos, rede etc.).

  3 - Criar a Máquina Virtual
    Clicar em “Máquinas Virtuais” > “Criar”
    Escolher a assinatura e o grupo de recursos
    Definir o nome da VM, região, sistema operacional (Windows ou Linux) e tamanho (SKU)
    Criar ou inserir credenciais de acesso (usuário/senha ou chave SSH)
  
  4 - Configurar Rede e Segurança
    Definir ou criar uma rede virtual (VNet)
    Selecionar uma sub-rede
    Configurar regras de entrada: por exemplo, liberar porta 22 (SSH) ou 3389 (RDP) para acesso remoto
  
  5 - Revisar e Criar
    Validar todas as configurações
    Clicar em “Criar” para que o Azure provisionar a VM
  
  6 - Acessar a VM
    Copiar o endereço IP público fornecido
    Acessar a máquina via RDP (Windows) ou SSH (Linux)

Dicas Úteis
- Use máquinas da camada gratuita (ex: B1s ou B1ms) para evitar cobranças durante testes.
- Prefira chave SSH para acesso a VMs Linux — mais seguro do que senhas.
- Evite deixar portas abertas (como RDP ou SSH) para todos os IPs; use regras de firewall específicas.
- Agrupe recursos no mesmo grupo de recursos para facilitar o gerenciamento e a exclusão.
- Desligue ou exclua a VM após o uso para evitar custos com processamento e armazenamento.
