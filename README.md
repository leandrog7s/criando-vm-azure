# criando-vm-azure
Este repositório faz parte do treinamento DIO - Criando uma VM no Azure

Resumo: Criar e Acessar uma VM no Azure (Trial + PuTTY)
1. Criar conta gratuita no Azure
- Acesse: https://azure.microsoft.com/pt-br/free
- Crie uma conta com e-mail e cartão de crédito (apenas para verificação)
- Ganhe até R$1.000 em crédito por 30 dias
- NÃO remova o limite de gastos para evitar cobranças
2. Criar uma Máquina Virtual Linux (Ubuntu)
1. Acesse o Portal do Azure: https://portal.azure.com
2. Vá em 'Máquinas virtuais' > 'Criar' > 'Máquina virtual'
3. Configure:
- Nome: ex. vmlab-teste
- Imagem: Ubuntu 20.04 LTS
- Tamanho: B1s (750h/mês grátis)
- Usuário: ex. leandro
- Autenticação: Chave pública SSH (gerar nova chave)
4. Clique em 'Revisar + criar' > 'Criar'
5. Baixe a chave privada (.pem) e salve com segurança
3. Converter a chave .pem para .ppk (PuTTYgen)
1. Abra o PuTTYgen
2. Clique em 'Load' e selecione o arquivo .pem (mude tipo para All Files)
3. Clique em 'Save private key' para salvar como .ppk
4. Obter IP público da VM
1. No portal do Azure, vá em Máquinas Virtuais > Sua VM
2. Copie o campo 'Endereço IP público'
5. Conectar à VM via PuTTYResumo: Criar e Acessar uma VM no Azure (Trial + PuTTY)
1. Abra o PuTTY
2. Em 'Host Name', digite: leandro@IP_PUBLICO
3. Vá em Connection > SSH > Auth e selecione o arquivo .ppk
4. Clique em 'Open' para iniciar a conexão via SSH
5. Confirme a conexão e pronto!
