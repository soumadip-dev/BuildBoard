<h1 align="center">BuildBoard ⚡</h1>

<p align="center">
  A community platform where builders showcase their projects, discover new launches, and connect with fellow creators.
</p>

<div align="center">
  <img src="https://github.com/soumadip-dev/InkBit/blob/main/public/banner.png" alt="Banner" width="900">
</div>

---

## 🔋 Features

- 🛠️ **Product Showcase** – Share apps, AI tools, SaaS, and creative projects with detailed listings
- 🔐 **Secure authentication** with Clerk (Passkeys, GitHub, Google)
- ⚡ **Real-time voting** – Upvote and downvote products to boost visibility
- 📱 **Fully responsive** – Optimized for mobile and desktop
- 🔔 **Toast notifications** – Real-time status updates for submissions and actions
- 📊 **Admin panel** – Full moderation and product management tools
- 🏷️ **Smart categorization** – Tag-based filtering and intelligent organization
- 🎯 **SEO-optimized** – Product pages built for discoverability
- 🚀 **Performance focused** – Optimized for speed and smooth interaction

## ⚙️ Tech Stack

- **🎨 Frontend**: Next.js 16 App Router, React 19, TypeScript, TailwindCSS 4
- **🗄️ Database**: NeonDB (PostgreSQL) with Drizzle ORM
- **🎭 UI Components**: Shadcn UI
- **🔐 Authentication**: Clerk
- ✅ **Validation**: Zod
- 📝 **Forms**: React Hook Form
- 🔧 **Package Manager**: pnpm

## 🤸 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/soumadip-dev/BuildBoard.git
cd BuildBoard
```

### 2. Install Dependencies

```bash
pnpm install
```

### 3. Environment Setup

Create a `.env.local` file in the root directory:

```env
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=<your_clerk_publishable_key>
CLERK_SECRET_KEY=<your_clerk_secret_key>
DATABASE_URL=<your_neondb_connection_string>
NEXT_PUBLIC_APP_URL=http://localhost:3000
```

### 4. Database Setup

```bash
# Push database schema
pnpm dlx drizzle-kit push

# Or run migrations
pnpm dlx drizzle-kit migrate
```

### 5. Run the Application

```bash
# Development
pnpm run dev

# Build for production
pnpm run build

# Start production server
pnpm start
```

Open [http://localhost:3000](http://localhost:3000) to see your community platform in action!

## 📁 Project Structure

```
BuildBoard/
├── app/                 # Next.js 16 App Router pages & layouts
├── components/          # React components (UI, product cards, forms)
├── lib/                 # Utilities, database client, auth helpers
├── public/              # Static assets
├── drizzle/             # Database schema and migrations
└── types/               # TypeScript definitions
```
