## Tech Stack

| Name                                                                    | Purpose        | Description                    |
| ----------------------------------------------------------------------- | -------------- | ------------------------------ |
| [next.js](https://nextjs.org/)                                          | Framework      | React framework for production |
| [next-Auth](https://next-auth.js.org/)                                  | Authentication | Authentication for Next.js     |
| [jsonwebtoken](https://www.npmjs.com/package/jsonwebtoken)              | JWT            | JWT for authentication         |
| [firebase](https://firebase.google.com/)                                | Database       | Database for images            |
| [prisma](https://www.prisma.io/)                                        | ORM            | ORM for database               |
| [MySQL](https://www.mysql.com/)                                         | Database       | Database for users             |
| [Tailwind CSS](https://tailwindcss.com/)                                | Styling        | CSS framework for styling      |
| [react-toastify](https://fkhadra.github.io/react-toastify/introduction) | Toasts         | Toasts for notifications       |
| [react-icons](https://react-icons.github.io/react-icons/)               | Icons          | Icons for UI                   |
| [@emailjs/browser](https://www.emailjs.com/)                            | Email          | Email service                  |

## Models

## Installation

### Dependencies

```bash
npm install
# or
yarn install
# or
pnpm install
```

### MySQL

- first ensure that the mysql80 service is running
- then enter your password in the mysql command line client
- then connect to the server in the mysql shell using `\connect root@localhost`
- now in sql mode to create the database run `create database <database_name>;`
- now to use the database run `use <database_name>;`
- the url for the database is `mysql://root:<password>@localhost:3306/<database_name>`

### Prisma

To see the CLI documentation [click here](https://www.prisma.io/docs/concepts/components/prisma-cli/commands#prisma-migrate-dev)

In the `/src` directory, run the following commands:

```bash
npx prisma init

# after defining the schema.prisma file, run the following command:

npx prisma migrate dev --name init

# To view the database in the prisma studio, run the following command:
npx prisma studio

# to generate the prisma client, after installing @prisma/client, run the following command:
npx prisma generate
```

## Start the development server

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.
