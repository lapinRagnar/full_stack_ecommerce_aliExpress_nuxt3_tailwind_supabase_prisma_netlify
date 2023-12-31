# Nuxt 3 Minimal Starter

Look at the [Nuxt 3 documentation](https://nuxt.com/docs/getting-started/introduction) to learn more.

## Setup

Make sure to install the dependencies:

```bash
# npm
npm install

# pnpm
pnpm install

# yarn
yarn install
```

## Development Server

Start the development server on `http://localhost:3000`:

```bash
# npm
npm run dev

# pnpm
pnpm run dev

# yarn
yarn dev
```

## Production

Build the application for production:

```bash
# npm
npm run build

# pnpm
pnpm run build

# yarn
yarn build
```

Locally preview production build:

```bash
# npm
npm run preview

# pnpm
pnpm run preview

# yarn
yarn preview
```

Check out the [deployment documentation](https://nuxt.com/docs/getting-started/deployment) for more information.

# site du tutoriel
https://www.youtube.com/watch?v=dVcCRFVhz74

# github du tuto
https://github.com/John-Weeks-Dev/aliexpress-clone


# les commandes pour le setups de l'application - installation de la dependance
 
 > npm create vite@latest 2_full_stack_ecommerce_aliExpress_nuxt3_tailwind_supabase_prisma_netlify --template vue
 
 > npm i @nuxtjs/supabase @nuxtjs/tailwindcss nuxt-icon @pinia-plugin-persistedstate/nuxt @pinia/nuxt @prisma/client @stripe/stripe-js nuxt-lodash prisma stripe


# supabase configuration

teny miafina ny supabase = Lapinragnar%%%

### les commandes pour prisma
> npx prisma init
> npx prisma generate
> npx prisma migrate dev --name init
> npx prisma db seed

apres la prochaine fois on fait ca pour reinitialiser la bdd
> npx prisma generate
> npx prisma reset

# google cloud pour la gestion des auth
https://console.cloud.google.com/welcome?hl=fr&pli=1&project=authentication-tuto-47f89

