# BlueBox

A web application designed to support the Training Records requirements of the SPL glider pilot training program. 

## Tech Stack

- **Frontend**: Next.js 14
- **Backend**: Prisma ORM with Neon.tech database
- **Authentication**: NextAuth with email/password
- **Styling**: Tailwind CSS with dark/light mode support

## Getting Started

1. Clone the repository
2. Install dependencies:

```bash
npm install
```

3. Set up your environment variables:

```bash
# Copy the example environment file and update with your values
cp .env.example .env
```

The `.env.example` file contains all the necessary environment variables with placeholder values. Edit the `.env` file with your actual configuration:

- `NEXT_PUBLIC_APP_NAME`: Your application name
- `NEXTAUTH_URL`: The base URL of your application (default: "http://localhost:3000")
- `NEXTAUTH_SECRET`: A secret key for NextAuth.js (at least 32 characters)
- `DATABASE_URL`: Your database connection string

Never commit your actual `.env` file to version control.

4. Run database migrations:

```bash
npx prisma migrate dev
```

5. Start the development server:

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to view the application.


## License

MIT License - see LICENSE file for details
