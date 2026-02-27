# Kingdom Fight School – KFS System

Plataforma de gestão e ensino da Kingdom Fight School (MVP). Mobile First.

## Stack

- **Next.js 14** (App Router) + TypeScript
- **Tailwind CSS** + design tokens (DOCS)
- **Supabase** – autenticação + PostgreSQL
- **Prisma** – ORM (base de dados no Supabase)
- **Vercel** – deploy

## Começar

1. **Dependências**
   ```bash
   npm install
   ```

2. **Variáveis de ambiente**
   - Copiar `.env.example` para `.env`
   - Preencher `NEXT_PUBLIC_SUPABASE_URL` e `NEXT_PUBLIC_SUPABASE_ANON_KEY` (Supabase → Project Settings → API)
   - Preencher `DATABASE_URL` (Supabase → Project Settings → Database → connection string)
   - **Login com Google**: ver **DOCS/Login_Google_Supabase.md**

3. **Base de dados**
   ```bash
   npx prisma generate
   npx prisma db push
   ```

4. **Desenvolvimento**
   ```bash
   npm run dev
   ```
   Abrir [http://localhost:3000](http://localhost:3000).

## Deploy (Vercel + kingdomfight.com)

Guia em **DOCS/Deploy_Vercel_kingdomfight.md**.

## Documentação

Ver pasta **DOCS/**.