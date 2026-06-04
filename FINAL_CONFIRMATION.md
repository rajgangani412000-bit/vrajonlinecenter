# Vraj Online Center - Final Confirmation

## Project Status

The Vraj Online Center web application has been generated in this folder:

`C:\Users\ATMIYA\Documents\New project`

## Included Modules

- Public business website
- Hidden admin login at `/secure-admin-login`
- Protected admin dashboard at `/dashboard`
- Customer CRM
- Service tracking database model
- PVC card management
- Income management
- Expense management
- Profit analytics dashboard
- Reminder and follow-up system
- Blog system
- AI chat assistant with enquiry capture
- PDF and CSV reports
- SEO metadata, sitemap, robots, and schema markup
- Auth.js login system
- Owner and Staff role access
- Prisma PostgreSQL database schema
- Seed data and default owner account
- Deployment and security guides

## Default Admin Login

URL:

`/secure-admin-login`

Email:

`admin@vrajonlinecenter.in`

Password:

`Admin@123456`

Important: The app forces password change on first login.

## Required Environment Variables

Set these in `.env` locally and in Vercel project settings:

```text
DATABASE_URL
NEXTAUTH_SECRET
NEXTAUTH_URL
APP_BASE_URL
CLOUDINARY_CLOUD_NAME
CLOUDINARY_API_KEY
CLOUDINARY_API_SECRET
CLOUDINARY_UPLOAD_FOLDER
```

## Local Test Commands

```bash
npm install
npm run db:generate
npm run db:push
npm run db:seed
npm run dev
```

Open:

`http://localhost:3000`

## Final Build Check

```bash
npm run qa
```

This runs TypeScript check, lint, and production build.

## Direct Vercel Deploy

Recommended deployment flow:

1. Upload/push this folder to GitHub.
2. Import the GitHub repo in Vercel.
3. Add all environment variables.
4. Connect PostgreSQL database.
5. Deploy.
6. Run database seed once.
7. Login through `/secure-admin-login`.
8. Change the default password.

## Important Note

The codebase was generated and statically checked in this workspace. The current shell did not have working npm/pnpm access, so final `npm install`, Prisma generation, and production build must be run after Node.js/npm is available or inside Vercel.
