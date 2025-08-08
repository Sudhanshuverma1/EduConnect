# EduConnect – Smart School Management System
EduConnect is a **modern, scalable, and responsive School Management System** built with **Next.js 15**, **Clerk Authentication**, **Prisma**, **PostgreSQL**, and **TailwindCSS**. Empower teachers, students, parents, and admins with a unified platform.

<h1></h1>
## 📸 Screenshots

**Admin Dashboard**  
![Admin Dashboard](https://via.placeholder.com/800x400.png?text=Admin+Dashboard)

**Student View**  
![Student View](https://via.placeholder.com/800x400.png?text=Student+View)

**Teacher View**  
![Teacher View](https://via.placeholder.com/800x400.png?text=Teacher+View)

**Parent View**  
![Parent View](https://via.placeholder.com/800x400.png?text=Parent+View)

<h1></h1>
## 🚀 Features

- 🔐 Secure authentication via Clerk
- 👤 Role-based dashboards: Admin, Teacher, Student, Parent
- 📚 Manage students, teachers, subjects, classes
- 📝 Assignments, Exams, and Results tracking
- 📅 Interactive calendar for events and lessons
- 📊 Attendance and performance visualization
- 📢 Announcement system
- ☁️ Cloudinary image upload
- 📱 Responsive UI using TailwindCSS
- 💾 PostgreSQL + Prisma ORM integration
- 🧠 Server actions via Next.js App Router
<h1></h1>

## 📂 Folder Structure
```
EduConnect/
├── prisma/                      # 🧬 Prisma schema & DB seeding
│   ├── migrations/              #    – Migration history
│   ├── schema.prisma            #    – DB schema
│   └── seed.ts                  #    – Sample seed data

├── public/                      # 🌐 Static assets & images
│   ├── *.png                    #    – UI icons and illustrations

├── src/                         # 🧠 Main app source
│   ├── app/                     #    – App routes (Next.js 15 App Router)
│   │   ├── dashboard/           #    – Role-based dashboards
│   │   │   ├── admin/           #      – Admin views (students, teachers, etc.)
│   │   │   ├── parent/          #      – Parent view
│   │   │   ├── student/         #      – Student view
│   │   │   └── teacher/         #      – Teacher view
│   │   ├── layout.tsx           #    – Root layout
│   │   ├── loading.tsx          #    – Loading state
│   │   └── [[...sign-in]]/      #    – Clerk auth page

│   ├── components/              # 🧩 Reusable UI components
│   │   └── forms/               #    – Feature-based UI components
│   │       ├── Charts, Tables, Forms, Calendars, Modals...
│   │       └── ...

│   ├── lib/                     # 🔧 Server utils & API logic
│   │   ├── actions.ts           #    – Server actions (create, update, delete)
│   │   ├── data.ts              #    – Static or fetched data
│   │   ├── formValidationSchemas.ts  # – Zod/Yup validation schemas
│   │   ├── prisma.ts            #    – Prisma client setup
│   │   ├── settings.ts          #    – App-level constants/settings
│   ├── middleware.ts            #    – Route guards & middlewares

├── .env                         # 🔐 Environment configuration
├── Dockerfile                   # 🐳 Docker config
├── docker-compose.yml           # 🐳 Docker services
├── next.config.mjs              # ⚙️ Next.js config
├── tailwind.config.ts           # 🎨 TailwindCSS config
├── postcss.config.mjs           # 💅 PostCSS config
├── tsconfig.json                # ✨ TypeScript config
├── package.json                 # 📦 Project metadata & scripts
├── .gitignore                   # 🚫 Git ignored files
├── .eslintrc.json               # 🧼 ESLint rules
└── README.md                    #  You're here 😄


```
<h1></h1>

## 🛠️ Tech Stack

![Next.js](https://img.shields.io/badge/Next.js-000?logo=nextdotjs&logoColor=white)
![Clerk](https://img.shields.io/badge/Clerk-Authentication-blueviolet)
![Prisma](https://img.shields.io/badge/Prisma-ORM-informational)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?logo=postgresql&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-38B2AC?logo=tailwindcss&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?logo=typescript&logoColor=white)
![Vercel](https://img.shields.io/badge/Deployed%20on-Vercel-black?logo=vercel)

<h1></h1>

## 💻 Getting Started

### Prerequisites

- Node.js ≥ 18
- PostgreSQL Database (Neon or Local)
- Clerk account for authentication
- Cloudinary account for image upload

### Installation

```bash
git clone https://github.com/Sudhanshuverma1/EduConnect.git
cd EduConnect
npm install
```
---

## ⚙️ Usage
### 🚀 Run Locally
- Install dependencies

```
npm install
```

- Start the development server

```
npm run dev
```
- Open your browser and navigate to:

```
http://localhost:3000
```


<h1></h1>

## 🔐 Environment Variables

### Create a .env file in the root:

```
DATABASE_URL=postgresql://<user>:<password>@<host>/<db>?sslmode=require
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your-publishable-key
CLERK_SECRET_KEY=your-secret-key
NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=your-cloud-name
NEXT_PUBLIC_CLOUDINARY_API_KEY=your-api-key
```

### 🤖 API Reference
Internal APIs are used via Server Actions and Prisma, e.g., for students, announcements, results, etc.

You can view them in:
```
src/lib/actions.ts
```
<h1></h1>
<h2>🔐 Access & Demo Credentials</h2>

> **Note:** Access is restricted to authenticated users.  

For demonstration purposes, use these credentials per dashboard:

| Role       | Username | Password  |
|------------|----------|-----------|
| Admin      | admin    | admin     |
| Teacher    | teacher  | teacher   |
| Student    | student  | student   |
| Parent     | parent   | parent    |

<h3> ⚠️ Please Do Not Delete or Alter Real Data </h3>

> **🙏 Humble Request:**  
> This project is open for community testing, learning, and collaboration. **Please do not intentionally delete, overwrite, or corrupt any actual or shared data** while using the platform.  
>  
> If you wish to perform destructive operations, kindly do so on your own fork/clone or with test accounts only. Help us keep the system clean and usable for everyone.

<h1></h1>

## 🧑‍💻 Contributing

We love contributions!

1. Fork the repo
2. Create your feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request 🚀

<h1></h1>


## ⭐ Acknowledgments

- Clerk.dev – Authentication
- Neon.tech – Postgres DB Hosting
- Vercel – Deployment Platform
- TailwindCSS – CSS Framework
- ShadCN/UI – UI Components

> **💡 Tip:** Star ⭐ this repo to stay updated!


**Enjoy using EduConnect!**  
Help us improve by reporting bugs or requesting features via Issues or Pull Requests.  
**Happy Learning!**

<h1></h1>

`Sudhanshu Verma ❤️ `
<h5> 📫 Contact: [sudhanshuuu01@gmail.com](mailto:sudhanshuuu01@gmail.com) </h5>
