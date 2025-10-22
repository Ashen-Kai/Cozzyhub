# CosyHub - Premium E-Commerce Platform

A full-featured, production-ready e-commerce platform built with Next.js 14, Supabase, and TypeScript. Your cozy corner for comfort and style, featuring a stunning glassmorphic UI with advanced animations and a complete admin dashboard.

## 🌟 Features

### Customer Features
- 🏠 **Beautiful Homepage** - Premium glassmorphic design with smooth animations
- 🛍️ **Product Catalog** - Browse all products with responsive grid layout
- 🔍 **Product Details** - Detailed product pages with image galleries
- 🛒 **Shopping Cart** - Full cart functionality with quantity controls
- 💳 **Checkout Process** - Streamlined checkout with order creation
- 👤 **User Authentication** - Secure login and signup with Supabase Auth
- 📦 **Order History** - View past orders and track status
- 🎨 **Premium UI** - Glassmorphism effects, transparency, and Framer Motion animations

### Admin Features
- 📊 **Dashboard** - Overview with statistics and recent orders
- 📦 **Product Management** - Add, edit, delete products with image URLs
- 🏷️ **Category Management** - Organize products by categories
- 📋 **Order Management** - View and update order statuses
- 👥 **User Management** - Admin role-based access control
- 📈 **Sales Analytics** - Track revenue and order metrics

## 🚀 Tech Stack

- **Framework**: Next.js 14 (App Router)
- **Language**: TypeScript
- **Database**: Supabase (PostgreSQL)
- **Authentication**: Supabase Auth
- **Styling**: Tailwind CSS
- **Animations**: Framer Motion
- **Icons**: Lucide React

## 📋 Prerequisites

- Node.js 18+ and npm
- Supabase account (free tier works)
- Git

## 🛠️ Installation

### 1. Install Dependencies

```bash
npm install
```

### 2. Set Up Supabase

1. Create a new project at [supabase.com](https://supabase.com)
2. Go to **SQL Editor** and run the schema from `supabase/schema.sql`
3. Enable **Email Authentication** in Authentication > Providers

### 3. Configure Environment Variables

Update `.env.local` with your Supabase credentials:

```env
NEXT_PUBLIC_SUPABASE_URL=your-project-url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your-anon-key
SUPABASE_SERVICE_ROLE_KEY=your-service-role-key
```

Find these values in your Supabase project settings under **API**.

### 4. Run the Development Server

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000)

## 🔐 Creating an Admin User

After signing up:

1. Go to Supabase Dashboard > Table Editor > `profiles`
2. Find your user and set `is_admin` to `true`
3. Visit `/admin` to access the admin dashboard

## 📁 Project Structure

```
premium-ecommerce-platform/
├── app/                      # Next.js App Router pages
│   ├── admin/               # Admin dashboard
│   ├── cart/                # Shopping cart
│   ├── products/            # Product pages
│   ├── login/signup/        # Auth pages
│   └── page.tsx             # Homepage
├── components/              # React components
│   ├── admin/               # Admin components
│   └── storefront/          # Customer components
├── lib/supabase/            # Supabase clients
├── supabase/schema.sql      # Database schema
└── middleware.ts            # Auth middleware
```

## 🗃️ Database Schema

### Tables
- **profiles** - User profiles with admin flags
- **products** - Product catalog with pricing and stock
- **categories** - Product categories
- **cart** - Shopping cart items
- **orders** - Customer orders
- **order_items** - Order line items

All tables have Row Level Security (RLS) enabled.

## 🎨 Key Features

### Glassmorphic UI
The entire UI features a premium glassmorphic design with:
- Backdrop blur effects
- Semi-transparent backgrounds
- Smooth gradients and transitions
- Framer Motion animations

### Admin Dashboard
- Real-time statistics
- Product CRUD operations
- Order management
- Status updates

### Shopping Experience
- Add to cart functionality
- Quantity adjustments
- Persistent cart storage
- Order creation

## 📦 Deployment

### Deploy to Vercel

1. Push to GitHub
2. Import in Vercel
3. Add environment variables
4. Deploy!

## 🔒 Security

- Row Level Security on all tables
- Middleware protects admin routes
- Secure authentication with Supabase
- Environment variables for secrets

## 🎯 Next Steps

1. Add your Supabase credentials to `.env.local`
2. Run the SQL schema in Supabase
3. Create your first admin user
4. Add products via the admin dashboard
5. Start shopping!

## 📝 License

MIT License - Free to use for personal or commercial projects.

---

Built with ❤️ using Next.js 14 and Supabase
