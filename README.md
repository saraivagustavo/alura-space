# Alura Space

**Alura Space** é uma aplicação web desenvolvida com Django, parte da formação da Alura em Django. O projeto simula um CRUD para o envio de publicações sobre corpos celestes, permitindo aos usuários cadastrar, visualizar, editar e excluir imagens relacionadas ao espaço.
De acordo com minha progressão na formação, o respositório, assim como a documentação, serão atualizados de acordo com as novidades!

## 🚀 Tecnologias Utilizadas

- **Backend**: Python 3.10+, Django 4.x
- **Frontend**: HTML, CSS
- **Banco de Dados**: SQLite (para desenvolvimento)
- **Autenticação**: Sistema de login próprio

## 📁 Estrutura do Projeto

```
alura-space/
├── galeria/                # Aplicação principal
│   ├── templates/          # Templates HTML
│   └── views.py            # Lógica de visualizações
├── setup/                  # Configurações do projeto
│   ├── settings.py         # Configurações gerais
│   └── urls.py             # Rotas da aplicação
├── static/                 # Arquivos estáticos (CSS, JS)
├── manage.py               # Script de gerenciamento
└── requirements.txt        # Dependências do projeto
```

## ⚙️ Como Rodar o Projeto

1. **Clone o repositório**:

   ```bash
   git clone https://github.com/saraivagustavo/alura-space.git
   cd alura-space
   ```

2. **Crie e ative um ambiente virtual**:

   ```bash
   python -m venv venv
   source venv/bin/activate  # No Windows: venv\Scripts\activate
   ```

3. **Instale as dependências**:

   ```bash
   pip install -r requirements.txt
   ```

4. **Configure as variáveis de ambiente**:

   - Crie um arquivo `.env` na raiz do projeto com as seguintes variáveis:

     ```
     SECRET_KEY=gerar_uma_chave_secreta
     DEBUG=True
     ALLOWED_HOSTS=localhost 127.0.0.1
     AWS_ACCESS_KEY_ID=sua_chave_de_acesso
     AWS_SECRET_ACCESS_KEY=sua_chave_secreta
     AWS_STORAGE_BUCKET_NAME=nome_do_seu_bucket
     ```

5. **Realize as migrações do banco de dados**:

   ```bash
   python manage.py migrate
   ```

6. **Crie um superusuário para acessar o painel administrativo**:

   ```bash
   python manage.py createsuperuser
   ```

7. **Inicie o servidor de desenvolvimento**:

   ```bash
   python manage.py runserver
   ```

   O projeto estará disponível em [http://127.0.0.1:8000](http://127.0.0.1:8000).

## 📸 Funcionalidades

- **Cadastro de Imagens**: Usuários podem enviar imagens relacionadas ao espaço.
- **Visualização**: Exibição das imagens cadastradas com detalhes.
- **Edição e Exclusão**: Opções para modificar ou remover imagens.
- **Administração**: Acesso ao painel administrativo do Django para gerenciamento de dados.

## 🧢 Testes

Para rodar os testes automatizados:

```bash
python manage.py test
```

## 📦 Dependências (requirements.txt)

```
asgiref==3.9.1
Django==5.2.6
python-dotenv==1.1.1
sqlparse==0.5.3
tzdata==2025.2
```
---

## 📄 Licença

Este projeto está licenciado sob a [MIT License](LICENSE).


