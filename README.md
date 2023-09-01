# Maturador-de-Chip
Maturador de chips é um pequeno programa para "esquentar" contas do whatssap e dessa forma, evitar banimento da rede social.

Instalação
Se você é usuário Windows, pode fazer download do instalador x64 ou siga as instruções abaixo para executar o código-fonte:

Clone o repositório
git clone https://https://github.com/iTsM4D/Maturador-de-Chip
Crie um ambiente virtual e ative-o

python -m venv .venv 
& .venv/scripts/activate.ps1
Instale as dependências
pip install -r requirements.txt
Inicie o programa
python main.py
Funcionalidades
Definir intervalo mínimo e máximo entre mensagens
Definir troca de conta após X mensagens
Definir máximo de mensagens
Parar em caso de bloqueio
Suporte até 10 contas
Roadmap
Permitir ao usuário escolher o nome da instância
Adicionar envio de arquivos
Remover o limite de contas
FAQ
Quais são as portas usadas por este programa?
A porta 5025 é usada pela API e a porta 5026 é usada pelo websocket.

Como apagar uma conta?
Como ainda não é possível escolher o nome da instância, não achei necessário ter a opção de apagar uma conta. Portanto, se você deseja trocar uma conta, pode simplesmente desconectá-la pelo próprio WhatsApp e reiniciar o programa.

Quais são os requisitos mínimos do sistema?
desenvolvi em uma maquina com processador i3 e 4GB de memoria RAM, portanto, se sua maquina possui configurações semelhantes ou superiores a essas, o maturador rodará sem problemas.

Como gerar meu próprio executável?
Este é o comando pyinstaller para gerar o executável do servidor websocket:

pyinstaller --noconfirm --onefile --windowed  "<PATH-DO-ARQUIVO-WEBSOCKET_SERVER.PY>"
Licença
distribuído sobre MIT Licença
