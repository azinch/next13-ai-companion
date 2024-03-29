# next13-ai-companion

### AI Companion Chatbot (create/chat with LLM-powered heroes)

## Features:

- Conversation generation (chatgpt LLM)
- Typescript
- Tailwind CSS
- Customizable components shadcn/ui
- Folder structure of Next 13 App Router
- Clerk Authentication (Email, Google)
- Server error handling using react-toast
- Stripe monthly subscription
- Free tier with API limiting
- POST, DELETE, GET in route handlers (app/api)

## Development Env

### Install packages

```shell
npm i
```
### Setup .env file

```js
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=

NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/dashboard
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/dashboard

OPENAI_API_KEY=
REPLICATE_API_TOKEN=

PINECONE_API_KEY=
PINECONE_ENVIRONMENT=
PINECONE_INDEX=

UPSTASH_REDIS_REST_URL=
UPSTASH_REDIS_REST_TOKEN=

NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=

DATABASE_URL=

STRIPE_API_KEY=
STRIPE_WEBHOOK_SECRET=

NEXT_PUBLIC_APP_URL="http://localhost:3000"
```

### Setup Prisma and update your DB

```shell
npx prisma db push

```

### Seed Companion categories

```shell
node scripts/seed.ts
```

### Start the app

```shell
npm run dev
```

### Available commands

Running commands with npm `npm run [command]`

| command         | description                              |
| :-------------- | :--------------------------------------- |
| `dev`           | Starts a development instance of the app |
