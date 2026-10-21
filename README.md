<h1 align="center">🍔 Site de Receitas com Django</h1>

<p align="center">
  Site de receitas feito com Django, usando templates reaproveitáveis (header, busca, cards e footer).
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Django_4.0-092E20?style=flat-square&logo=django&logoColor=white" alt="Django">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white" alt="CSS3">
  <img src="https://img.shields.io/badge/status-em_desenvolvimento-yellow?style=flat-square" alt="Em desenvolvimento">
</p>

---

## 📖 Sobre

Projeto de estudo de **Django**. A página inicial lista receitas em cards com imagem, título, autor, data, categoria e resumo. O layout foi organizado em **templates parciais** para reaproveitar componentes.

## ✨ O que já tem

- Projeto Django (`projeto`) com o app `receitas`
- Página inicial em `/`
- Templates parciais: `head`, `header`, `search`, `receitas` (card) e `footer`
- Ícones com Font Awesome

## 🗺️ Próximos passos

- [ ] Model `Receita` e `Categoria` no banco
- [ ] Página de detalhe da receita
- [ ] Filtro por categoria e busca funcional
- [ ] Cadastro de receitas pelo Django Admin
- [ ] Mover `SECRET_KEY` e `DEBUG` para variáveis de ambiente

## ▶️ Como executar

**Pré-requisito:** Python 3.8+

```bash
git clone https://github.com/GuiDobelin/Site_Django.git
cd Site_Django

python3 -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate

pip install "django>=4.0,<5"
python manage.py migrate
python manage.py runserver
```

Acesse **http://127.0.0.1:8000**.

## 📁 Estrutura

```
Site_Django/
├── manage.py
├── projeto/                     # Configurações do projeto (settings, urls, wsgi/asgi)
├── base_templates/global/       # Templates globais
└── receitas/                    # App de receitas
    ├── views.py
    ├── urls.py
    └── templates/receitas/
        ├── pages/home.html
        └── partials/            # head, header, search, receitas, footer
```

---

<p align="center">Feito por <a href="https://github.com/GuiDobelin">Guilherme Dobelin</a></p>
