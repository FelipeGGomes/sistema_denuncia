
🛡️ Sistema de Denúncias Anônimas Comunitárias

📝 Descrição do Projeto
O Sistema de Denúncias Anônimas Comunitárias é uma aplicação web desenvolvida em Django que visa facilitar e centralizar a comunicação de problemas urbanos e de segurança dentro de bairros e comunidades. O foco principal é garantir o anonimato e a segurança do cidadão, ao mesmo tempo em que oferece uma ferramenta eficaz para o acompanhamento e resolução de problemas pela administração local.

✨ Funcionalidades Principais
Registro de Denúncia Anônima: Permite que qualquer cidadão registre um problema (como buracos na rua, iluminação queimada, descarte irregular de lixo, etc.) sem a necessidade de login.

Envio de Evidências: Suporte para upload de fotos para documentar o problema (funcionalidade de FileField).

Módulo de Acompanhamento (Tracking): Após o registro, o usuário recebe um Protocolo Único (DEN-XXXXXX) que pode ser usado para consultar o status da denúncia de forma totalmente anônima.

Gestão de Status e Prioridade: Painel administrativo completo para a equipe técnica alterar o status (e.g., "Em Análise", "Em Resolução", "Resolvido") e definir a prioridade do atendimento.

Geração de PDF do Protocolo: Emissão de um documento PDF do protocolo (usando Xhtml2pdf), garantindo o registro oficial e facilitando a impressão e o arquivamento pelo cidadão.

Sistema de Logs (Auditoria): Rastreamento de todas as alterações feitas na denúncia (quem alterou, quando e o quê) através do modelo LogDenuncia.

🚀 Tecnologias Utilizadas
Categoria	Tecnologia	Uso
Backend	Python 3.x, Django 5.x	Core da aplicação, ORM, Views e Rotas.
Frontend	HTML5, CSS3, JavaScript	Interface responsiva e interações.
Banco de Dados	SQLite3 (Desenvolvimento)	Armazenamento de dados de denúncias e categorias.
PDF	xhtml2pdf	Geração robusta de relatórios e protocolos a partir de templates HTML.
Estilização	CSS nativo (Design Customizado)	Layout limpo, focado na experiência do usuário.

Exportar para as Planilhas
⚙️ Como Executar o Projeto
Para rodar este projeto em sua máquina local, siga os passos abaixo:

Clone o repositório:

Bash

git clone cd sistema_denuncias
Crie e ative o ambiente virtual:

Bash

python -m venv .venv
.venv\Scripts\activate
Instale as dependências:

Bash

pip install -r requirements.txt 
pip install django xhtml2pdf Pillow
Execute as migrações:

Bash

py manage.py makemigrations
py manage.py migrate
Crie um superusuário (para acesso ao Admin):

Bash

py manage.py createsuperuser
Inicie o servidor de desenvolvimento:

Bash

py manage.py runserver
Acesse o endereço http://127.0.0.1:8000/ no seu navegador.
