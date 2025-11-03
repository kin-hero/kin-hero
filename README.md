# Hi there, I'm Keane Putra Setiawan 👋

## 🚀 About Me

I'm a **Full-Stack Software Engineer** based in Osaka, Japan, with a passion for building scalable, cloud-native applications that solve real-world problems. I love the entire journey of software development—from architecting robust backend systems to crafting delightful user experiences on the frontend.

**🌟 Currently seeking new opportunities!** I'm actively looking for my next challenge where I can leverage my full-stack expertise, cloud architecture skills, and passion for building scalable systems. If you're hiring or know of interesting opportunities, I'd love to connect!

**What drives me:** I'm fascinated by the intersection of clean code, system design, and business impact. Whether it's optimizing API performance, designing event-driven architectures, or implementing AI-powered features, I thrive on technical challenges that push me to learn and grow.

**Why I love coding:** There's something magical about transforming an idea into a working application. I love the problem-solving aspect of engineering—identifying bottlenecks, weighing trade-offs, and designing systems that are not just functional, but scalable and maintainable. The best feeling? Seeing users interact with something I built from scratch.

---

## 💼 Professional Experience

**Software Development Engineer** @ [株式会社グラッドキューブ - Glad Cube](https://corp.glad-cube.com/)
📍 Osaka, Japan | 🗓️ Jul 2023 - Present

- Led the strategic migration of core API from Express.js to **Fastify**, achieving a **35% improvement** in API response times
- Spearheaded full migration of a **20,000-line JavaScript codebase to TypeScript**, catching **50+ potential bugs** pre-production
- Owned end-to-end development of a client collaboration project, single-handedly building both frontend and backend
- Conducted comprehensive **load testing** to identify and eliminate bottlenecks, ensuring **99.9% uptime** during peak traffic
- Engineered a hybrid rendering model (SSR for SEO + CSR for interactivity) for the company's main site

---

## 🛠️ Featured Projects

### 1. [Recipify](https://recipify.keanesetiawan.com/) 🍳

**A social recipe-sharing platform for food lovers to discover, create, and share culinary creations**

[![Live Demo](https://img.shields.io/badge/Live-Demo-brightgreen?style=flat-square)](https://recipify.keanesetiawan.com/)
[![GitHub](https://img.shields.io/badge/GitHub-Repo-blue?style=flat-square&logo=github)](https://github.com/kin-hero/Recipify/)
[![Case Study](https://img.shields.io/badge/📚_Case_Study-Read_Full_Details-orange?style=flat-square)](https://www.keanesetiawan.com/projects/recipify)

**Tech Stack:**

- **Frontend:** Next.js, React, TypeScript, Tailwind CSS, Zod
- **Backend:** Node.js, Fastify, TypeScript
- **Database:** PostgreSQL (Supabase), Prisma ORM
- **Cloud:** AWS Lambda, S3, CloudFront, API Gateway, Route 53, Amplify, SES
- **DevOps:** Git, GitHub Actions

**Key Features:**

- Full-stack recipe CRUD with secure authentication & JWT-based session management
- Asynchronous image processing pipeline with AWS S3 and CloudFront CDN
- Token-based email verification using AWS SES
- Achieved **99 Lighthouse Performance Score**

**Architecture Highlights:**

- Designed a v1 "Monolithic Lambda" architecture for rapid development
- Architected a production-grade v2 "Event-Driven Microservices" design addressing scalability bottlenecks:
  - Monolithic Lambda → Distributed Microservices pattern
  - Synchronous image processing → Asynchronous SQS queue processing
  - Direct database queries → L2 cache layer with ElastiCache
  - API Gateway payload limits → Pre-signed URLs for direct S3 uploads

**What I Learned:**

- Real-world trade-offs between monolithic vs. microservice architectures
- The critical importance of CDNs for global performance (reduced image latency from 2-3s to <300ms)
- Infrastructure as Code (IaC) with serverless.com for secure, repeatable deployments
- Full ownership of the application lifecycle from ideation to deployment and architectural evolution

---

### 2. [ChefGPT](https://chefgpt.keanesetiawan.com/) 🤖

**AI-powered recipe generation platform that transforms your ingredients into culinary magic using LLMs**

[![Live Demo](https://img.shields.io/badge/Live-Demo-brightgreen?style=flat-square)](https://chefgpt.keanesetiawan.com/)
[![GitHub](https://img.shields.io/badge/GitHub-Repo-blue?style=flat-square&logo=github)](https://github.com/kin-hero/ai-recipe)
[![Case Study](https://img.shields.io/badge/📚_Case_Study-Read_Full_Details-orange?style=flat-square)](https://www.keanesetiawan.com/projects/chefgpt)

**Tech Stack:**

- **Frontend:** Next.js, React, TypeScript, Tailwind CSS
- **Backend:** Next.js API Routes, Zod, OpenRouter AI, Clerk Authentication
- **Database:** AWS DynamoDB (NoSQL)
- **Cloud:** AWS Amplify, Route 53, IAM
- **DevOps:** GitHub Actions, Docker

**Key Features:**

- AI-powered recipe generation using OpenRouter API (access to 100+ LLM models)
- Smart rate limiting (1 generation/5 minutes) and quota management (max 10 recipes/user)
- Cost-effective architecture at **~$1.40/month for 100 MAU**
- DynamoDB TTL for automatic rate limit cleanup (no cron jobs needed)
- Client-side filtering for instant UI response
- Secure authentication with Clerk (SSO with Google)

**Technical Decisions:**

- Chose **DynamoDB over SQL** for unstructured recipe data with read-heavy patterns and single-digit millisecond latency
- Used **OpenRouter AI** instead of individual API keys for instant LLM experimentation across providers
- Implemented **Clerk** for production-ready auth instead of custom JWT flows, eliminating weeks of security implementation

**What I Learned:**

- Never trust LLM output format—implemented robust parsing with markdown cleanup, brace extraction, and fallback strategies
- Researched cloud platform reserved environment variables (AWS_ACCESS_KEY_ID conflicts in Amplify)
- Leveraged TypeScript's type inference from Zod schemas to maintain type safety across frontend/backend boundaries
- Used DynamoDBDocumentClient with marshallOptions for automatic bidirectional conversion

---

## 🧰 Tech Stack

### Frontend

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=next.js&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white)
![Framer Motion](https://img.shields.io/badge/Framer_Motion-0055FF?style=flat-square&logo=framer&logoColor=white)

### Backend

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-000000?style=flat-square&logo=express&logoColor=white)
![Fastify](https://img.shields.io/badge/Fastify-000000?style=flat-square&logo=fastify&logoColor=white)

### Database

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![DynamoDB](https://img.shields.io/badge/DynamoDB-4053D6?style=flat-square&logo=amazon-dynamodb&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white)

### Cloud & DevOps

![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazon-aws&logoColor=white)
![AWS Lambda](https://img.shields.io/badge/AWS_Lambda-FF9900?style=flat-square&logo=aws-lambda&logoColor=white)
![AWS S3](https://img.shields.io/badge/AWS_S3-569A31?style=flat-square&logo=amazon-s3&logoColor=white)
![CloudFront](https://img.shields.io/badge/CloudFront-8C4FFF?style=flat-square&logo=amazon-cloudfront&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white)

---

## 📫 Let's Connect!

I'm always excited to connect with fellow developers, discuss tech, or collaborate on interesting projects! **Currently open to new opportunities** - feel free to reach out if you're hiring or know of interesting roles!

[![Portfolio](https://img.shields.io/badge/Portfolio-keanesetiawan.com-brightgreen?style=flat-square&logo=google-chrome&logoColor=white)](https://keanesetiawan.com)
[![Resume](https://img.shields.io/badge/📄_Resume-Download_PDF-red?style=flat-square)](https://personal-portfolio-images.keanesetiawan.com/resume.pdf)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Keane_Putra_Setiawan-blue?style=flat-square&logo=linkedin)](https://www.linkedin.com/in/keane-putra-setiawan)
[![GitHub](https://img.shields.io/badge/GitHub-kin--hero-black?style=flat-square&logo=github)](https://github.com/kin-hero)
[![Twitter](https://img.shields.io/badge/Twitter-@buildwithKin-1DA1F2?style=flat-square&logo=twitter&logoColor=white)](https://x.com/buildwithKin)

---

**💡 Currently exploring:** System Design, AI/LLM integration patterns, Data Structures and Algorithm

**🎯 2025 Goals:** Build powerful projects that help me learn, Finish 100 Neetcode questions

---

_"The best code is the code that solves a real problem elegantly."_
