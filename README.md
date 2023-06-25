## T3 Todo App with Authentication

### Purpose
To learn T3 stack

### Overview

This is a Todo app with authentication. The app allows users to add, edit, and delete Todo items, and it uses GitHub accounts for authentication. The user interface is built using Tailwind CSS, providing a responsive design.

I have already deployed the application, and you can access it [here]().

### App Screens

The main screens of the app are as follows:

1. **Home Page (Non-logged in)**
    - The home page displays a "Sign In" button.

2. **Login Page**
    - The login page displays a button for logging in and the GitHub logo.
    - Users can authenticate by clicking on "Sign in with GitHub."

3. **Home Page (Logged in)**
    - After logging in, the following elements are displayed:
        - Logged-in user's email address
        - Logout button
        - Form for creating a new Todo
        - Todo progress bar

4. **Creating a Todo (Optimistic Updates)**
    - The app utilizes optimistic updates, a technique explained in Chapter 15 of the documentation, to provide users with a seamless experience.
    - When I enter a Todo and click the "Create" button, the field is reset, and an optimistic Todo is added to the list, reflecting the progress ratio on the progress bar.
    - Eventually, when the server processes the request successfully, the optimistic Todo is replaced with the correct Todo. This demonstrates that the UI is updated without waiting for the server response.

The implementation of optimistic updates may be advanced, but I will follow the detailed explanations in the documentation to master it.

### Technologies and Stack

I have developed this app using the following technologies and stack:

- Next.js
- tRPC
- NextAuth.js
- Prisma
- Tailwind CSS
- TypeScript
- Supabase
- Vercel
- Docker

Now, let's take a closer look at each of these technologies.

#### Next.js

Next.js is an open-source web development framework developed by Vercel. It is based on React and offers a lightweight, flexible framework that supports server-side rendering and is SEO-friendly.

#### TypeScript

TypeScript is an open-source programming language that extends JavaScript. Unlike JavaScript, TypeScript is statically typed, meaning types are defined during development.

#### tRPC

tRPC (TypeScript Remote Procedure Call) is a lightweight library that allows remote calling of backend functions from the client. With tRPC, I can execute backend procedures defined on the server from the frontend and share TypeScript type information between the frontend and backend.

#### NextAuth.js

NextAuth.js is a library that makes it easy to implement authentication in Next.js applications. It supports email authentication as well as OAuth authentication with services such as Google, Twitter, Facebook, and GitHub.

#### Prisma

Prisma is an ORM (Object-Relational Mapping) for Node.js and TypeScript. It provides declarative data modeling, migration functionality through "Prisma Migrate," and a type-safe database client generated from the data model called "Prisma Client." Prisma also offers "Prisma Studio," a web-based UI for browsing tables.

#### Tailwind CSS

Tailwind CSS is a utility-first CSS framework designed to provide flexibility in styling by using utility classes instead of writing custom CSS.

#### Supabase

Supabase is a Backend as a Service (BaaS) platform that uses PostgreSQL as its database. It offers services such as database management, authentication, storage, and edge functions.

#### Vercel

Vercel is a serverless platform provided by the creators of Next.js, Vercel Inc. It enables easy deployment of Next.js applications.

#### Docker

Docker is an open platform for developing, shipping, and running applications using containerization. In this project, I have used Docker to set up the Supabase environment.

---

With the above technologies and stack, I have created an application similar to the one described. The deployment is done using Vercel and Supabase. I followed the T3 Stack, a technology stack proposed by Theo, which focuses on simplicity, modularity, and full-stack type safety.