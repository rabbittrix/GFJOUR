## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

## env.exemple

# Kinde for secure, fast authentication - https://link.joshtriedcoding.com/kinde
KINDE_CLIENT_ID=
KINDE_CLIENT_SECRET=
KINDE_ISSUER_URL=https://<KINDE-PROJECT-NAME>.kinde.com
KINDE_SITE_URL=http://localhost:3000
KINDE_POST_LOGOUT_REDIRECT_URL=http://localhost:3000
KINDE_POST_LOGIN_REDIRECT_URL=http://localhost:3000/dashboard

# Database for storing everything except PDF files - (Provider up to you, I like PlanetScale)
DATABASE_URL=

# Uploadthing for storing PDF files - https://uploadthing.com/dashboard
UPLOADTHING_SECRET=
UPLOADTHING_APP_ID=

# OpenAI for answering PDF questions - https://platform.openai.com/
OPENAI_API_KEY=

# Stripe for payment processing - https://stripe.com/
STRIPE_SECRET_KEY=
STRIPE_WEBHOOK_SECRET=

# Pinecone for long-term vector storage - https://www.pinecone.io/
PINECONE_API_KEY=

## Setup Prisma
npx prisma db push

npm i --save-dev prisma@latest
npm i @prisma/client@latest
