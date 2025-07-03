# Next.js + Drizzle + Neon + Better Auth Starter Template

A modern, production-ready starter template for building full-stack web applications with authentication, database management, and a beautiful UI out of the box.

## 🚀 Tech Stack

- **[Next.js 15](https://nextjs.org/)** - React framework with App Router and Turbopack
- **[TypeScript](https://www.typescriptlang.org/)** - Type-safe development
- **[Drizzle ORM](https://orm.drizzle.team/)** - Type-safe SQL ORM
- **[Neon](https://neon.tech/)** - Serverless PostgreSQL database
- **[Better Auth](https://www.better-auth.com/)** - Modern authentication library
- **[Tailwind CSS](https://tailwindcss.com/)** - Utility-first CSS framework
- **[Shadcn/ui](https://ui.shadcn.com/)** - Beautiful, accessible UI components
- **[Lucide React](https://lucide.dev/)** - Beautiful icons

## ✨ Features

### 🔐 Authentication
- **Social Login**: Pre-configured Google and GitHub OAuth
- **Session Management**: Secure session handling with Better Auth
- **Database Integration**: User data stored in PostgreSQL via Drizzle ORM
- **Type-Safe**: Full TypeScript support for auth flows

### 🗄️ Database
- **Serverless PostgreSQL**: Powered by Neon for scalable, serverless database
- **Type-Safe ORM**: Drizzle ORM with full TypeScript integration
- **Pre-built Schema**: User, session, account, and verification tables
- **Easy Migrations**: Simple schema updates with `npx drizzle-kit push`

### 🎨 UI/UX
- **Modern Design**: Clean, responsive interface with Tailwind CSS
- **Dark/Light Mode**: Theme switching with next-themes
- **Component Library**: Shadcn/ui components for consistent design
- **Beautiful Icons**: Lucide React icon library

### 🛠️ Developer Experience
- **TypeScript**: Full type safety across the entire stack
- **Hot Reload**: Fast development with Turbopack
- **ESLint + Prettier**: Code formatting and linting
- **Package Manager**: Optimized for pnpm

## 🚀 Quick Start

### Prerequisites
- Node.js 18+ 
- pnpm (recommended package manager)
- Neon database account
- Google OAuth app (optional)
- GitHub OAuth app (optional)

### 1. Clone and Install
```bash
git clone <your-repo-url>
cd nextjsdrizzlebetterauthneon
pnpm install
```

### 2. Environment Setup
Create a `.env.local` file:
```env
# Database
DATABASE_URL="your-neon-database-url"

# Authentication (Optional - for social login)
GOOGLE_CLIENT_ID="your-google-client-id"
GOOGLE_CLIENT_SECRET="your-google-client-secret"
GITHUB_CLIENT_ID="your-github-client-id"
GITHUB_CLIENT_SECRET="your-github-client-secret"
```

### 3. Database Setup
```bash
# Push the schema to your database
npx drizzle-kit push
```

### 4. Run Development Server
```bash
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) to see your application.

## 📁 Project Structure

```
├── app/                    # Next.js App Router
│   ├── api/auth/          # Authentication API routes
│   ├── globals.css        # Global styles
│   ├── layout.tsx         # Root layout
│   └── page.tsx           # Home page
├── components/            # Reusable UI components
├── db/                    # Database configuration
│   ├── index.ts          # Database connection
│   └── schema.ts         # Drizzle schema definitions
├── lib/                   # Utility libraries
│   ├── auth.ts           # Better Auth configuration
│   └── utils.ts          # Helper functions
└── drizzle.config.ts     # Drizzle configuration
```

## 🔧 Customization

### Adding Shadcn/ui Components
```bash
pnpm dlx shadcn@latest add button
pnpm dlx shadcn@latest add input
```

### Database Schema Changes
1. Update `db/schema.ts`
2. Run `npx drizzle-kit push` to apply changes

### Adding Authentication Providers
Edit `lib/auth.ts` to add more social providers or configure email/password auth.

## 📚 Learn More

- [Next.js Documentation](https://nextjs.org/docs)
- [Drizzle ORM Documentation](https://orm.drizzle.team/)
- [Better Auth Documentation](https://www.better-auth.com/)
- [Neon Documentation](https://neon.tech/docs)
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)

## 🚀 Deploy

### Vercel (Recommended)
1. Push your code to GitHub
2. Connect your repository to [Vercel](https://vercel.com)
3. Add your environment variables
4. Deploy!

### Other Platforms
This template works with any platform that supports Node.js applications (Railway, Render, DigitalOcean, etc.).

## 📄 License

This template is open source and available under the [MIT License](LICENSE).

---

**Ready to build something amazing?** This starter gives you everything you need to create a modern web application with authentication, database, and beautiful UI components. Happy coding! 🎉
