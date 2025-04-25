# Streaming App

<div>
  <img src="https://img.shields.io/badge/-TypeScript-black?style=for-the-badge&logoColor=white&logo=typescript&color=3178C6" alt="typescript" />
  <img src="https://img.shields.io/badge/-Next_JS-black?style=for-the-badge&logoColor=white&logo=nextdotjs&color=000000" alt="nextdotjs" />
  <img src="https://img.shields.io/badge/-Tailwind_CSS-black?style=for-the-badge&logoColor=white&logo=tailwindcss&color=06B6D4" alt="tailwindcss" />
</div>

<h3 align="center">A Modern Video Conferencing Platform</h3>

## Overview

SyncStream is a cutting-edge video conferencing solution designed for seamless real-time communication. Built with modern web technologies, it offers an intuitive interface similar to industry-leading platforms while maintaining exceptional performance and security.

The platform features a clean, dark-themed dashboard with quick access to core functionalities including instant meeting creation, joining via link, scheduling, and recording management. The time-centric design emphasizes upcoming meetings and provides clear navigation through the sidebar.

## Technology Stack

- **Frontend Framework**: Next.js 14.1.3
- **Language**: TypeScript
- **Authentication**: Clerk
- **Real-time Communication**: Stream IO Video SDK
- **UI Components**: Radix UI primitives with shadcn/ui
- **Styling**: Tailwind CSS with custom dark theme
- **Date Handling**: date-fns, react-datepicker
- **Unique Identifiers**: UUID

## Key Features

### Streamlined Meeting Experience
- **New Meeting**: Create instant meetings with one click
- **Join Meeting**: Enter meetings via invitation links
- **Schedule Meeting**: Plan future meetings with detailed settings
- **View Recordings**: Access and manage recorded sessions
- **Personal Room**: Dedicated space with persistent link for recurring meetings
![Image](https://github.com/user-attachments/assets/c21149ca-fc4b-435c-8ea8-fa704060ccca)

### Dashboard Interface
- **Time-Aware Layout**: Displays current time and upcoming meetings
- **Intuitive Navigation**: Sidebar access to Home, Upcoming, Previous, and Recordings
- **Card-Based Design**: Visual organization of meeting types and functions
- **Dark Mode**: Optimized for reduced eye strain during long sessions

### Meeting Tools
- HD video and audio streaming
- Screen sharing functionality
- Recording capabilities
- Participant management
- Custom layouts and views
- Emoji reactions and interactive elements

## Installation & Setup

### Prerequisites
- Node.js 18.x or higher
- npm 9.x or higher

### Getting Started

```bash
# Clone the repository
git clone https://github.com/Sandigupta/Streaming_App.git

# Navigate to project directory
cd Streaming_App

# Install dependencies
npm install
```

### Environment Configuration

Create a `.env.local` file in the root directory:

```
# Authentication - Clerk
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_key
CLERK_SECRET_KEY=your_clerk_secret
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up

# Stream IO API
NEXT_PUBLIC_STREAM_API_KEY=your_stream_key
STREAM_SECRET_KEY=your_stream_secret
```

### Development Commands

```bash
# Start development server
npm run dev

# Build for production
npm run build

# Start production server
npm run start

# Run linting
npm run lint
```

## Architecture

SyncStream implements a modern application architecture leveraging Next.js 14's advanced features:

- **App Router**: Utilizing the latest Next.js routing patterns
- **React Server Components**: For optimized server-side rendering
- **Client Components**: For interactive UI elements
- **API Routes**: For secure backend functionality
- **Middleware**: For authentication and request handling

### Component Structure

The application follows a modular component architecture:

```
components/
├── dashboard/          # Dashboard layout components
│   ├── Sidebar.tsx     # Navigation sidebar
│   ├── MeetingCard.tsx # Meeting option cards
│   └── TimeDisplay.tsx # Current date/time display
├── meeting/            # Video conferencing components
│   ├── Controls.tsx    # Meeting control buttons
│   ├── Participants.tsx # Participant management
│   └── Stream.tsx      # Video streaming interface
└── ui/                 # Base UI components (shadcn/ui)
```

## Performance Optimizations

- Server-side rendering for initial page loads
- Optimized asset loading with Next.js Image component
- Component-level code splitting
- Memoization of expensive operations
- Edge function deployments for global performance
- WebRTC optimization for low-latency communication

## Deployment

SyncStream is configured for deployment on Vercel:

```bash
# Deploy to Vercel
vercel

# Production deployment
vercel --prod
```

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add your feature'`)
4. Push to your branch (`git push origin feature/your-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

---

Developed by [Sandigupta](https://github.com/Sandigupta)
