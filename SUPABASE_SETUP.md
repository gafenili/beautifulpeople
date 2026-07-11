# Votação compartilhada

1. Crie um projeto no [Supabase](https://supabase.com/).
2. Em **Authentication > Providers**, habilite **Anonymous sign-ins**.
3. Abra o **SQL Editor**, cole e execute todo o conteúdo de `supabase-votacao.sql`.
4. Em **Settings > API**, copie a URL do projeto e a **Publishable key**. Em projetos antigos, a chave pode se chamar `anon`.
5. Cole os dois valores em `supabase-config.js`.

O site usa uma conta anônima por navegador e o banco impede dois votos da mesma conta na mesma pergunta. Se a pessoa apagar os dados do navegador ou usar outro dispositivo, poderá votar novamente. Para uma garantia de uma pessoa real por voto, seria necessário exigir login, por exemplo com Google ou e-mail.
