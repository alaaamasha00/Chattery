Social Media App

A modern desktop-first social media platform built with Next.js 14 App Router, Clerk authentication, Prisma with PostgreSQL, and UploadThing for media uploads.
The app focuses on real-time-like interactions through server actions and cache revalidation, delivering a smooth, scalable user experience.

✨ Features

🔐 Authentication & User Sync

Clerk for sign-up/login

Automatic sync of Clerk users into the Prisma database

📝 Posts, Likes & Comments

Rich post creation with optional image upload

Nested comments & threaded discussions

Like system with instant UI updates

🤝 Follow System

Follow/unfollow users

Personalized feeds

🔔 Notifications

Automatic notifications for likes, comments, and follows

Excludes self-actions

Bulk “mark all as read”

🖼️ Image Uploads

Secure uploads using UploadThing

Auth middleware ensures only logged-in users can upload

🎨 Modern UI/UX

Built with shadcn/ui and TailwindCSS

Responsive, accessible, and clean

Toast feedback for user actions

🛠️ Tech Stack

Framework: Next.js 14 (App Router, Server Actions)

Auth: Clerk

Database: PostgreSQL + Prisma ORM

File Storage: UploadThing

UI Library: shadcn/ui + TailwindCSS

Utilities: date-fns, react-hot-toast

🚀 Getting Started
Prerequisites

Node.js 18+

PostgreSQL database

Clerk account & keys

UploadThing account & keys

Installation

Clone the repo

git clone https://github.com/yourusername/social-media-app.git
cd social-media-app


Install dependencies

npm install


Set up environment variables
Create a .env file with:

DATABASE_URL="your_postgres_url"
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY="your_clerk_publishable_key"
CLERK_SECRET_KEY="your_clerk_secret_key"
UPLOADTHING_SECRET="your_uploadthing_secret"
UPLOADTHING_APP_ID="your_uploadthing_app_id"


Run database migrations

npx prisma migrate dev


Start the dev server

npm run dev
