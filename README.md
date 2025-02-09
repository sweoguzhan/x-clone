# X (Twitter) Clone

A modern Twitter clone built with Next.js 14, featuring real-time notifications, infinite scroll, and a clean UI design. This project demonstrates the implementation of key social media features using cutting-edge web technologies.

![Project Preview](project-preview.png)

## ✨ Features

### Core Features
- 🔒 **Authentication** - Secure user authentication with Clerk
- 📝 **Posts** - Create, like, repost and comment on posts
- 👥 **Social** - Follow/unfollow users
- 🔔 **Real-time Notifications** - Instant notifications for likes, comments, reposts and follows
- ♾️ **Infinite Scroll** - Dynamic content loading with infinite scroll

### Additional Features
- 🖼️ **Media Handling** - Upload and edit images with different aspect ratios
- 📱 **Responsive Design** - Fully responsive UI that works on all devices
- 🎨 **Modern UI** - Clean and modern interface similar to Twitter
- 💾 **Data Persistence** - Reliable data storage with PostgreSQL
- 🔍 **Server Actions** - Utilizes Next.js 14 server actions for better performance

## 🛠️ Tech Stack

### Frontend
- **Next.js 14** - React framework with App Router
- **Tailwind CSS** - Utility-first CSS framework
- **React Query** - Server state management
- **Socket.IO Client** - Real-time client communications

### Backend
- **Next.js API Routes** - Backend API endpoints
- **Prisma** - Type-safe database ORM
- **PostgreSQL** - SQL database
- **Socket.IO** - Real-time server communications

### Services
- **Clerk** - Authentication and user management
- **ImageKit** - Image storage and transformation
- **Vercel** - Deployment and hosting

## 🚀 Getting Started

### Prerequisites

- Node.js 18+ 
- PostgreSQL database
- Clerk account
- ImageKit account

### Installation Steps

1. Clone the repository:
```bash
git clone https://github.com/yourusername/twitter-clone.git
cd twitter-clone
```

2. Install dependencies:
```bash
npm install
# or
yarn install
```

3. Set up environment variables:

Create a `.env` file in the root directory with the following variables:
```env
# Database
DATABASE_URL="your-postgresql-url"

# Clerk Auth
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

# ImageKit
NEXT_PUBLIC_URL_ENDPOINT=
```

4. Run database migrations:
```bash
npx prisma migrate dev
```

5. Start the development server:
```bash
npm run dev
# or
yarn dev
```

6. Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## 📝 Project Structure

```
├── src/
│   ├── app/             # Next.js app router pages
│   ├── components/      # React components
│   ├── actions/         # Server actions
│   ├── prisma/         # Database schema and client
│   └── utils/          # Utility functions
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Next.js Documentation](https://nextjs.org/docs)
- [Clerk Documentation](https://clerk.dev/docs)
- [Prisma Documentation](https://www.prisma.io/docs)
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)