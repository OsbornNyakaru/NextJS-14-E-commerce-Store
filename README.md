This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

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

# Educational Platform - Cognita
Welcome to the Educational Platform project! This README will guide you through the setup, configuration, and usage of the platform. This project aims to provide a comprehensive educational platform similar to edX, offering courses, certifications, and interactive learning experiences.

![thumbnail](https://github.com/OsbornNyakaru/PLP-Project-Cognita/assets/110415101/b1ee7e6e-4ee2-4413-a94c-370e99f858cd)

## Table of Contents

1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Technologies Used](#technologies-used)
4. [Installation](#installation)
5. [Configuration](#configuration)
6. [Usage](#usage)
7. [Project Structure](#project-structure)
8. [Contributing](#contributing)
9. [License](#license)

## Project Overview

The E-Commerce Platform is designed to deliver high-quality online shopping through a user-friendly and scalable web application.

## Features

- **User Authentication**: Secure user registration and login.
- **Sales Management**: Enables tracking the number of sales, orders and products available for sale.
- **Payment System**: Stripe payment system to allow simplified, fast and secure payment.

## Technologies Used

### Frontend

- **Typescript**: Markup language for structuring the web content.
- **TailwindCSS**: Stylesheet language for designing the web pages.

### Backend

- **Node.js**: JavaScript runtime environment for server-side scripting.
- **Prisma**: Web framework for Node.js to build RESTful APIs.
- **Railway**: Web framework for Node.js to build RESTful APIs.

### Database

- **MySQL on Railway**: Relational database management system for storing sales and orders.

### Payment Integration

- **Stripe**: Payment processing platform for handling course payments.

### Authentication

- **Clerk**: Authentication service for managing user sign-ups, logins, and sessions.

## Installation

1. **Clone the repository:**

    ```sh
    git clone https://github.com/OsbornNyakaru/PLP-Project-Cognita.git
    cd PLP-Project-Cognita
     ```

2. **Install backend dependencies:**

    ```sh
    npm init -y
    npm install stripe express.js nodemon dotenv
    ```

3. **Configure the environment variables:**

    Create a `.env` file in the root directory and add the following:

    ```plaintext
    PORT=3000
    NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
    CLERK_SECRET_KEY=
    NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
    NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
    NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
    NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/
    ```

4. **Initialize the database:**

    Ensure MySQL is running and create a database for the project. Then run the SQL scripts provided in the `database` folder to set up the necessary tables.

5. **Run the server:**

    ```sh
    npm start
    ```

    The server will start on `http://localhost:3000`.

## Usage

1. **Access the platform:**

    Open your web browser and navigate to `http://localhost:3000`.

2. **Sign up and log in:**

    Use Clerk's authentication system to sign up and log in to the platform.

3. **Browse and try out the ecommerce admin store:**

    Browse available courses, add them to your cart, and proceed to checkout using Stripe for payments.

## Contributing

Contributions are welcome! Please submit a pull request or open an issue for any changes or improvements.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.



Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel 

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
