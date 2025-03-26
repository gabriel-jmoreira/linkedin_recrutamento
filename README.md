# Automação LinkedIn - Envio de Conexões

Este projeto é uma automação para enviar solicitações de conexão no LinkedIn com uma mensagem personalizada para recrutadores de tecnologia. Utilizando o Selenium WebDriver, o script simula ações no navegador para fazer pesquisas de recrutadores e enviar solicitações de conexão automaticamente.

## Funcionalidades

- **Login automático no LinkedIn**: O script realiza o login na sua conta LinkedIn.
- **Busca por Tech Recruiters**: O script pesquisa por "Tech Recruiter" na barra de pesquisa do LinkedIn.
- **Filtra o tipo de pessoas**: Filtra para exibir apenas pessoas nos resultados da pesquisa.
- **Envio de solicitações de conexão**: Envia até 50 solicitações de conexão com uma mensagem personalizada para recrutadores de tecnologia.
- **Personalização da mensagem**: O script envia uma mensagem personalizada, incluindo o nome do recrutador e informações sobre a sua experiência profissional.

## Tecnologias

- Python 3.x
- Selenium
- WebDriver Manager
- Chrome WebDriver
- dotenv

## Como configurar o ambiente

### 1. Clonar o repositório

Clone o repositório para sua máquina local:

git clone https://github.com/gabriel-jmoreira/linkedin_recrutamento.git

2. Instalar dependências
Certifique-se de ter o Python 3.x instalado na sua máquina. Em seguida, instale as dependências do projeto.

Primeiro, crie um ambiente virtual para o projeto (opcional, mas recomendado):
python -m venv venv

Ative o ambiente virtual:

Windows:
.\venv\Scripts\activate

Linux/macOS:
source venv/bin/activate

Agora, instale as dependências com o pip:
pip install -r requirements.txt

3. Configurar variáveis de ambiente
Para que o script funcione corretamente, é necessário configurar suas credenciais do LinkedIn, incluindo seu e-mail e senha.

Crie um arquivo chamado .env na raiz do projeto.

Adicione as seguintes variáveis ao arquivo .env:
LINKEDIN_EMAIL=seu_email_aqui
LINKEDIN_PASSWORD=sua_senha_aqui
Nota: Nunca compartilhe seu arquivo .env publicamente, pois ele contém informações sensíveis.

4. Executar o script
Depois de configurar o ambiente e as variáveis de ambiente, você pode rodar o script com o seguinte comando:
python seu_arquivo.py

O script abrirá uma instância do navegador Chrome, fará login na sua conta do LinkedIn, buscará por recrutadores de tecnologia e enviará solicitações de conexão até atingir o limite de 50.

.gitignore
O arquivo .env (que contém suas credenciais de login) foi adicionado ao arquivo .gitignore para garantir que não seja enviado para o repositório GitHub. Isso evita o vazamento de suas informações sensíveis. Certifique-se de que o arquivo .env está presente em seu projeto e nunca seja enviado para o repositório remoto.

Licença
Este projeto está licenciado sob a Licença MIT - veja o arquivo LICENSE para mais detalhes.
Personalizando o Script
Você pode personalizar o script da seguinte maneira:

Alterando o conteúdo da mensagem que é enviada aos recrutadores.

Ajustando a quantidade de conexões que o script enviará (atualmente está limitado a 50).

Modificando a pesquisa no LinkedIn para buscar por diferentes tipos de recrutadores ou outras palavras-chave.

Observação
O script faz uma busca automatizada e pode violar os Termos de Serviço do LinkedIn se for usado em grande escala. Use-o com cautela e em conformidade com as regras da plataforma.

