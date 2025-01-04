# **SaaS Code Editor - CodeCraft**

This project features the creation of **CodeCraft**, an advanced online IDE inspired by **VS Code**. It allows users to write, execute, and share code snippets across multiple programming languages with secure payment integration.

---

## **Features**

- **Multi-Language Support**:
  - Supports **10 programming languages**.
  - Free plan users can execute JavaScript code.
  - Paid plan unlocks Python, Java, Go, C++, and more.

- **Secure Payments**:
  - Lifetime access through **Lemon Squeezy** integration.

- **Snippet Sharing**:
  - Users can share, star, and comment on code snippets.
  - Snippets can be filtered, searched, and viewed in grid or list formats.

- **Real-Time Updates**:
  - Built with **Convex** for a seamless, real-time experience.

- **Interactive Profile Dashboard**:
  - Tracks code executions, favorite snippets, and usage statistics.

---

## **Tech Stack**

- **Frontend**: Next.js (v15) with TailwindCSS
- **Backend**: Convex for real-time database and serverless functions
- **Authentication**: Clerk for user management and secure authentication
- **Payments**: Lemon Squeezy for encrypted payment processing
- **Editor**: Monaco Editor for a VS Code-like experience

---

## **Directory Structure**

```bash
├── app
│   ├── components
│   ├── pages
│   ├── services
│   ├── styles
│   └── utils
├── convex
│   ├── schema
│   └── http
├── constants
├── types
├── public
│   └── assets
├── prisma
│   └── schema.prisma
├── README.md
└── package.json
```

---

## **Setup and Installation**

### **Prerequisites**

1. **Node.js**: Version 16 or above.
2. **Convex Account**: Sign up at [Convex](https://convex.dev).
3. **Clerk API Key**: Obtain from [Clerk](https://clerk.dev).
4. **Lemon Squeezy API Key**: Set up payments via [Lemon Squeezy](https://www.lemonsqueezy.com).

### **Steps**

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/codecraft.git
   cd codecraft
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Set up environment variables:
   - Create a `.env.local` file in the root directory and include:

     ```env
     NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_next_public_clerk
     CLERK_SECRET_KEY=your_clerk_secret_key
     CONVEX_DEPLOYMENT=your_convex_deployment_key
     NEXT_PUBLIC_CONVEX_URL=your_public_convex_url
     ```

4. Initialize Convex:

   ```bash
   npx convex dev
   ```

5. Run the application:

   ```bash
   npm run dev
   ```

6. Access the app at `http://localhost:3000`.

---

## **How It Works**

### **Core Workflow**

1. **User Authentication**:
   - Secure login and sign-up via Clerk.
   - Supports Google and GitHub authentication.

2. **Real-Time Updates**:
   - Convex database ensures real-time sharing and updates of code snippets.

3. **Code Execution**:
   - Runs user-written code with error messages or success outputs.

4. **Snippet Sharing**:
   - Allows creating, sharing, and starring snippets within a community.

5. **Payment Integration**:
   - Lemon Squeezy manages secure payments for upgrading to the Pro plan.

---

## **Deployment**

1. **Build for Production**:

   ```bash
   npm run build
   ```

2. **Deploy**:
   - Host the app on Vercel or AWS.
   - Configure `.env` for the production environment.

---

## **Future Enhancements**

- Add advanced editor features such as code linting.
- Support team collaboration for shared projects.
- Include AI-powered code suggestions.

---

## **Contributing**

Contributions are welcome! Please fork the repository, create a feature branch, and submit a pull request.

---

## **License**

This project is licensed under the MIT License. See the `LICENSE` file for more details.

---
