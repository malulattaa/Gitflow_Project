# Formulário — Histórico de Versões (GitFlow)

## Descrição
Projeto de formulário de contato em HTML e CSS usado para praticar GitFlow (features → releases → hotfix).

---

## Versão 1 — v1.0.0
**Objetivo:** Estrutura básica do formulário HTML.  
**Arquivos principais:** `index.html`, `style.css` (versão simples).  
**Comandos:**
git flow feature start versao1-html
git add index.html style.css
git commit -m "feat(versao1-html): estrutura básica do formulário (HTML + CSS simples)"
git flow feature finish versao1-html
git flow release start v1.0.0
git flow release finish v1.0.0

## Versão 2 - v2.0.0
**Objetivo:** Melhorar o design com um visual moderno, sombras e responsividade.
git flow feature start melhora-css
git add style.css
git commit -m "feat(melhora-css): adiciona design moderno, sombras e responsividade"
git flow feature finish melhora-css
git flow release start v2.0.0
git flow release finish v2.0.0

## Versão 3 - v3.0.0
**Objetivo:** Melhorar a estrutura HTML com elementos semânticos (header, main, footer).
git flow feature start melhora-html
git add index.html
git commit -m "feature(melhora-html): adiciona header, main e footer, estrutura semântica"
git flow feature finish melhora-html
git flow release start v3.0.0
git flow release finish v3.0.0

## Hotfix - v3.0.1
**Problema:** O botão de envio foi alterado por engano para type="button", impedindo o envio do formulário.
**Solução:** Restaurar o tipo correto (type="submit") para reativar o envio.
# simular bug no main 
git flow hotfix start corrigir-botao-envio
# editar index.html (restaurar type="submit")
git add index.html
git commit -m "hotfix(corrigir-botao-envio): restaura type=submit para permitir envio do formulário"
git flow hotfix finish corrigir-botao-envio

