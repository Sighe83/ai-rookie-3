# Supabase + Vercel Integration Project

A Next.js project configured for deployment on Vercel with Supabase integration.

## Getting Started

### 1. Set up Supabase

1. Go to [supabase.com](https://supabase.com) and create a new project
2. In your project settings, find your:
   - Project URL (API URL)
   - Public API Key (anon key)

### 2. Configure Environment Variables

1. Copy `.env.example` to `.env.local`:
   ```bash
   cp .env.example .env.local
   ```

2. Update `.env.local` with your Supabase credentials:
   ```
   NEXT_PUBLIC_SUPABASE_URL=https://your-project.supabase.co
   NEXT_PUBLIC_SUPABASE_ANON_KEY=your-anon-key-here
   ```

### 3. Install Dependencies

```bash
npm install
```

### 4. Run Development Server

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to see your app.

### 5. Deploy to Vercel

1. Push your code to GitHub
2. Go to [vercel.com](https://vercel.com) and import your repository
3. In your Vercel project settings, add the same environment variables:
   - `NEXT_PUBLIC_SUPABASE_URL`
   - `NEXT_PUBLIC_SUPABASE_ANON_KEY`

## Project Structure

```
src/
├── app/
│   ├── page.tsx          # Main page with Supabase connection test
│   └── layout.tsx        # Root layout
├── lib/
│   └── supabase.ts       # Supabase client configuration
└── ...
```

## Features

- ✅ Next.js 15 with TypeScript
- ✅ Tailwind CSS for styling
- ✅ Supabase client integration
- ✅ Connection status indicator
- ✅ Vercel deployment configuration
- ✅ Environment variable setup

## Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run lint` - Run ESLint

## Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `NEXT_PUBLIC_SUPABASE_URL` | Your Supabase project URL | Yes |
| `NEXT_PUBLIC_SUPABASE_ANON_KEY` | Your Supabase anonymous/public key | Yes |
