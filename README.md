# rank-math-api-manager
Manages Rank Math metadata update via HTTP request, including focus keyword.

# Rank Math API Manager Extended

Este é um plugin WordPress desenvolvido por **Hikelmy Henrich** que permite atualizar os campos de SEO do plugin **Rank Math** via REST API.

## ✨ Funcionalidades

- Atualiza título SEO (`rank_math_title`)
- Atualiza descrição SEO (`rank_math_description`)
- Atualiza canonical URL (`rank_math_canonical_url`)
- Atualiza palavra-chave de foco (`rank_math_focus_keyword`)

## 🛠 Requisitos

- WordPress 5.0 ou superior
- Plugin [Rank Math SEO](https://rankmath.com/) instalado
- Permissão de usuário com `edit_posts`

## 🚀 Como instalar

1. Faça o download deste repositório
2. Copie a pasta `rank-math-api-manager` para `wp-content/plugins/`
3. Ative o plugin no painel WordPress

## 🔌 Endpoint da API

POST /wp-json/rank-math-api/v1/update-meta


### Parâmetros:

| Campo | Tipo | Obrigatório | Descrição |
|-------|------|-------------|-----------|
| `post_id` | integer | ✅ | ID do post a ser atualizado |
| `rank_math_title` | string | opcional | Novo título SEO |
| `rank_math_description` | string | opcional | Nova descrição SEO |
| `rank_math_canonical_url` | string | opcional | Novo canonical |
| `rank_math_focus_keyword` | string | opcional | Palavra-chave foco |

## 📺 Vídeo explicativo

Leia neste artigo de como identifiquei o problema, desenvolvi a solução e a testei:
🔗 [Ler tutorial]([#](https://hikelmyhenrich.com/como-automatizei-o-rank-math-seo-no-wordpress-via-rest-api-e-n8n-uma-solucao-pratica-para-otimizacao-de-seo-em-massa/)) *(adicione o link do vídeo quando subir)*

---

Feito com 💚 por [Hikelmy Henrich](https://hikelmyhenrich.com)
