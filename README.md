# 📚 API ESCOLA

Esse projeto é uma API de uma escola construída com **Django REST Framework**. A ideia aqui é simular um sistema simples de gestão escolar — com cursos, estudantes e matrículas — do jeito que se faz no mundo real: organizado, funcional e pronto pra evoluir.

Se quiser acompanhar o andamento ou entender melhor o contexto do projeto, dá uma olhada no Trello:
👉 https://trello.com/b/jpsMUMxV/django-rest-framework-escola-curso-04

---

## ⚙️ Preparando o ambiente

Antes de sair rodando tudo, bora fazer do jeito certo: ambiente isolado pra evitar dor de cabeça.

### 1. Criar o ambiente virtual

Dentro da pasta do projeto:

```bash
python -m venv venv
```

### 2. Ativar o ambiente

* **Windows:**

```bash
venv\Scripts\activate
```

* **Linux/macOS:**

```bash
source venv/bin/activate
```

Se apareceu `(venv)` no terminal, tá no caminho certo.

---

## 📦 Instalando as dependências

Com o ambiente ativo:

```bash
pip install -r requirements.txt
```

Sem segredo. Isso aqui puxa tudo que o projeto precisa pra rodar.

---

## 🗄️ Banco de dados (migrações)

Agora vamos preparar o banco:

```bash
python manage.py makemigrations
python manage.py migrate
```

Aqui você basicamente cria e aplica a estrutura do banco. Sem isso, nada funciona.

---

## 🚀 Rodando o projeto

Hora de colocar a API no ar:

```bash
python manage.py runserver
```

Acesse no navegador:
👉 http://localhost:8000/

Se abriu, já era. Tá rodando.

---

## 🌱 Populando o banco (dados de teste)

Pra não ficar tudo vazio, já tem script pronto:

```bash
python popular_banco_cursos.py
python popular_banco_estudantes.py
```

Isso cria cursos e estudantes automaticamente.

Depois disso, você já pode:

* Criar matrículas
* Testar endpoints
* Usar ferramentas tipo Thunder Client ou Postman

---

## 💡 Dica direta

Projeto backend não é só fazer endpoint — é organização, padrão e clareza. Esse README aqui já é parte disso. Se outra pessoa bater no teu repositório, ela precisa conseguir rodar sem te chamar no WhatsApp.

---

Se quiser, posso te ajudar a deixar isso ainda mais profissional (tipo padrão de empresa mesmo, com Docker, variáveis de ambiente, deploy, etc).
