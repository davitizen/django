# ⚽ Projeto Django - Times de Futebol

Este projeto é uma aplicação web desenvolvida com Django que permite cadastrar e visualizar times de futebol.

---

## 🚀 Funcionalidades

- Cadastro de times via painel administrativo
- Visualização dos times em página web
- Integração com banco de dados SQLite
- Interface simples e funcional

---

## 🧱 Estrutura do Projeto

O projeto segue o padrão MVT do Django:

- **Model** → Representa os dados (times)
- **View** → Lógica da aplicação
- **Template** → Interface HTML
- **URL** → Rotas do sistema

---

## 🗄️ Model

O model principal é:

```python
class Time(models.Model):
    nome = models.CharField(max_length=100)
    cidade = models.CharField(max_length=100)
    titulos = models.IntegerField()
