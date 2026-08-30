# nextjs-lab

Simple steps I used to start this Next.js app.

## 1. Create the app

From `nextjs-lab`, I created the project with Next.js 13.4:

```bash
npx create-next-app@13.4
```

This installs React, Next.js, TypeScript, Tailwind, and ESLint.

![Installing dependencies](docs/create-next-app-install.png)

When it finished, the app was created at `next-app`:

![App created](docs/create-next-app-success.png)

## 2. Database

The app uses Prisma with MySQL. Add this to a `.env` file in `next-app`:

```
DATABASE_URL="mysql://USER:PASSWORD@localhost:3306/next_course"
```

Then run:

```bash
npx prisma generate
```

## 3. Run the app

```bash
cd next-app
npm run dev
```

Open [http://localhost:3000](http://localhost:3000).

![Dev server](docs/npm-run-dev.png)
