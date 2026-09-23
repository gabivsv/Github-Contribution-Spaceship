# 🚀 GitHub Contribution Spaceship
> **Transforme seu gráfico de contribuições do GitHub em uma viagem pelo espaço.** 🌌

Uma animação espacial personalizada para gráficos de contribuições do GitHub, desenvolvida com **JavaScript, Node.js, SVG, CSS e GitHub Actions**.

Em vez da tradicional cobrinha 🐍, este projeto transforma o calendário de contribuições em um **céu estrelado**, onde uma nave espacial percorre uma rota formada pelas semanas de maior atividade. ✨

---

## 🌌 Demonstração

<picture>
  <source
    media="(prefers-color-scheme: dark)"
    srcset="https://raw.githubusercontent.com/gabivsv/github-contribution-spaceship/output/github-contribution-spaceship-dark.svg?v=1">

<source
 media="(prefers-color-scheme: light)"
 srcset="https://raw.githubusercontent.com/gabivsv/github-contribution-spaceship/output/github-contribution-spaceship.svg?v=1">

<img
 alt="Nave espacial percorrendo o gráfico de contribuições"
 src="https://raw.githubusercontent.com/gabivsv/github-contribution-spaceship/output/github-contribution-spaceship.svg?v=1"> </picture>

---

## 🛰️ Como funciona?

O projeto consulta o **calendário de contribuições do GitHub** e transforma esses dados em uma visualização SVG animada, mantendo os dados reais do GitHub.

* ⭐ Cada contribuição é representada por uma estrela, de acordo com o nível de atividade;
* 🌠 Uma estrela de destaque é selecionada por semana para formar a rota;
* 🛸 A nave percorre essa rota e interage visualmente com as estrelas;
* ⚙️ O GitHub Actions gera automaticamente as versões do gráfico para os temas claro e escuro.

---

## 🧠 Tecnologias

| Tecnologia                  | Utilização                  |
| --------------------------- | --------------------------- |
| 🟨 **JavaScript / Node.js** | Lógica e geração do gráfico |
| 🎨 **SVG**                  | Construção da visualização  |
| ✨ **CSS**                   | Animações e efeitos visuais |
| ⚙️ **GitHub Actions**       | Automação da geração        |
| 🔗 **GitHub GraphQL API**   | Consulta das contribuições  |

---

## 📁 Estrutura do projeto

```text
github-contribution-spaceship/
│
├── .github/
│   └── workflows/
│       └── spaceship.yml       # Executa e publica o gerador
│
├── src/
│   ├── github.mjs              # Consulta as contribuições
│   ├── stars.mjs               # Cria estrelas, legenda e rota
│   ├── spaceship.mjs            # Desenha a nave
│   ├── animation.mjs            # Define as animações CSS
│   └── generate.mjs             # Junta os componentes e gera o SVG
│
├── README.md                    # Documentação
├── LICENSE                      # Licença do projeto
└── package.json                 # Configuração do projeto
```

---

## 🚀 Usar no próprio perfil

Faça um **fork** deste repositório e adapte-o ao seu perfil do GitHub.

O repositório de perfil deve ter o mesmo nome do seu usuário:

```text
SEU_USUARIO/SEU_USUARIO
```
Depois:

* Copie a pasta `src/` e o workflow `.github/workflows/spaceship.yml`.
* Crie uma branch chamada `output`.
* Em **Settings → Actions → General → Workflow permissions**, habilite **Read and write permissions**.
* Execute o workflow em **Actions → Generate contribution spaceship → Run workflow**.
---

## 👤 Adicionar ao README do perfil

Depois que o workflow terminar, adicione o seguinte trecho ao README do seu perfil.

Substitua `SEU_USUARIO` pelo seu nome de usuário do GitHub:

```html
<picture>
  <source
    media="(prefers-color-scheme: dark)"
    srcset="https://raw.githubusercontent.com/SEU_USUARIO/SEU_USUARIO/output/github-contribution-spaceship-dark.svg?v=1">

  <source
    media="(prefers-color-scheme: light)"
    srcset="https://raw.githubusercontent.com/SEU_USUARIO/SEU_USUARIO/output/github-contribution-spaceship.svg?v=1">

  <img
    alt="Nave espacial percorrendo o gráfico de contribuições"
    src="https://raw.githubusercontent.com/SEU_USUARIO/SEU_USUARIO/output/github-contribution-spaceship.svg?v=1">
</picture>
```

## 🧩 Arquitetura

O fluxo principal do projeto pode ser resumido assim:

```text
GitHub GraphQL API
        ↓
Calendário de contribuições
        ↓
Processamento dos dados
        ↓
Estrelas + níveis de atividade
        ↓
Definição da rota
        ↓
Nave espacial
        ↓
SVG + CSS
        ↓
GitHub Actions
        ↓
Imagem exibida no README
```

---

## 👩🏻‍🚀 Autoria

Este projeto foi idealizado e personalizado por **@gabivsv**, utilizando JavaScript, Node.js, SVG, CSS e GitHub Actions, com assistência de IA em partes da implementação.

---

## 📄 Licença

Este projeto está disponível sob a **MIT License**.

