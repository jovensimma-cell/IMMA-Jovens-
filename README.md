# I.M.M.A. · Coordenadoria de Jovens (app)

Aplicação web instalável (PWA) com base de dados Supabase e código no GitHub.

## 1. Supabase
1. Crie um projecto em supabase.com.
2. Abra **SQL Editor**, cole o conteúdo de `supabase/schema.sql` e execute.
3. Em **Project Settings → API**, copie o **Project URL** e a chave **anon public**.
4. Em **Authentication → URL Configuration**, ponha o endereço final da app (passo 3) em *Site URL*.
5. Crie a sua conta na app. Depois, no SQL Editor, execute a última linha comentada do `schema.sql` (com o seu email) para se tornar administrador.

## 2. Ligar a app
Em `index.html`, substitua `SUPABASE_URL` e `SUPABASE_KEY` pelos valores do passo 1.3.
Use apenas a chave **anon**. Nunca coloque a chave `service_role` no código.

## 3. GitHub
```
git init && git add . && git commit -m "I.M.M.A. app"
git branch -M main
git remote add origin https://github.com/SEU_UTILIZADOR/imma-app.git
git push -u origin main
```
No repositório: **Settings → Pages → Branch: main / root**. O endereço fica `https://SEU_UTILIZADOR.github.io/imma-app/`.

## 4. Instalar como app
- Android (Chrome): menu ⋮ → **Instalar aplicação**.
- iPhone (Safari): Partilhar → **Adicionar ao ecrã principal**.
- Ficheiro APK: gere em pwabuilder.com colando o endereço do GitHub Pages.

## O que já está pronto
- Base de dados, permissões por função (membro, igreja, região, província, administrador) e promover/despromover, tudo validado no servidor.
- Entrar/criar conta, ficha de cadastro, lista de jovens com pesquisa em todos os campos, detalhe e contactos (ligar, WhatsApp, redes sociais).

## Falta ligar (a base de dados já suporta)
Actividades, relatos de gratidão, canal de publicações com aprovação e ficheiros, ecrã de promover/despromover, eliminar fichas.
