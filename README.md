This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Live Preview of the Application

[Netflix Clone Live Preview](https://netflix-clone.dasci.dev)

## Environment Setup

This project requires certain environment variables to be set for proper functioning. Create a `.env` file in the root of the project and add the following variables:

```plaintext
# Database Configuration
DATABASE_URL=mongodb://yourMongoDBURLHere

# Authentication
NEXTAUTH_JWT_SECRET=yourJWTSecretHere
NEXTAUTH_SECRET=yourNextAuthSecretHere

# OAuth Configuration for GitHub
GITHUB_ID=yourGitHubClientIdHere
GITHUB_SECRET=yourGitHubClientSecretHere

# OAuth Configuration for Google
GOOGLE_CLIENT_ID=yourGoogleClientIdHere
GOOGLE_CLIENT_SECRET=yourGoogleClientSecretHere
```

## Movies Setup

Populating the Movies Database

The project includes a movies.json file containing a collection of movie data. You can use this file to populate the movies table in your database. Here's how to do it:

    Ensure you have set up your database correctly and have the necessary environment variables in your .env file, especially the DATABASE_URL.

    Use a script or a database management tool to import the data from movies.json into your movies table. The exact method will depend on the database system and tools you are using.

    Verify that the data has been correctly imported into your database and is accessible from your application.

This step is crucial for having a pre-filled database of movies, which will allow you to test and use the application's features that interact with this data.



## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `pages/index.tsx`. The page auto-updates as you edit the file.

[API routes](https://nextjs.org/docs/api-routes/introduction) can be accessed on [http://localhost:3000/api/hello](http://localhost:3000/api/hello). This endpoint can be edited in `pages/api/hello.ts`.

The `pages/api` directory is mapped to `/api/*`. Files in this directory are treated as [API routes](https://nextjs.org/docs/api-routes/introduction) instead of React pages.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
