# Sol Learning Platform

## Overview

Sol Learning Platform is a K-12 educational web application that provides personalized learning experiences for students. The platform features course management, interactive learning materials, mock tests, progress tracking, and an AI-powered chat assistant named Sol. Built with a modern full-stack architecture, it offers real-time communication capabilities and a responsive design optimized for both desktop and mobile devices.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript for type safety and component-based architecture
- **Routing**: Wouter for lightweight client-side routing
- **State Management**: TanStack React Query for server state management and caching
- **UI Framework**: Shadcn/ui components built on Radix UI primitives with Tailwind CSS for styling
- **Build Tool**: Vite for fast development and optimized production builds
- **Design System**: Custom CSS variables with light/dark mode support and responsive breakpoints

### Backend Architecture
- **Runtime**: Node.js with Express.js framework
- **Language**: TypeScript with ES modules
- **API Design**: RESTful endpoints with WebSocket support for real-time features
- **Real-time Communication**: WebSocket server for live chat functionality
- **Error Handling**: Centralized error middleware with structured error responses
- **Development**: Hot module replacement and live reloading via Vite integration

### Data Storage Solutions
- **Database**: PostgreSQL with Drizzle ORM for type-safe database operations
- **Schema Management**: Drizzle Kit for migrations and schema synchronization
- **Connection**: Neon Database serverless PostgreSQL for cloud hosting
- **Data Validation**: Zod schemas for runtime type checking and validation
- **Session Storage**: PostgreSQL-based session management with connect-pg-simple

### Authentication and Authorization
- **Session Management**: Express sessions with PostgreSQL storage
- **User Context**: User ID-based authorization for API endpoints
- **WebSocket Auth**: User ID validation for real-time connection management
- **Data Access**: User-scoped queries to ensure data isolation

### Core Features Architecture
- **Course Management**: Hierarchical structure with courses, topics, and progress tracking
- **Assessment System**: Mock tests with question banks, scoring, and attempt tracking
- **Progress Tracking**: Individual topic completion and course-wide progress calculation
- **AI Chat Assistant**: OpenAI GPT-4o integration for educational support and quiz generation
- **Real-time Features**: WebSocket-based chat with automatic reconnection

### Design Patterns
- **Component Composition**: Reusable UI components with consistent prop interfaces
- **Custom Hooks**: Abstracted logic for WebSocket connections, mobile detection, and toast notifications
- **Repository Pattern**: Storage interface abstraction for database operations
- **Service Layer**: Separated business logic for AI integration and external services
- **Type Safety**: End-to-end TypeScript with shared schemas between client and server

## External Dependencies

### Database Services
- **Neon Database**: Serverless PostgreSQL hosting with connection pooling
- **Drizzle ORM**: Type-safe database toolkit with automatic migrations

### AI Services
- **OpenAI API**: GPT-4o model for chat responses and quiz generation
- **Environment Configuration**: API key management through environment variables

### UI and Styling
- **Radix UI**: Accessible component primitives for complex UI elements
- **Tailwind CSS**: Utility-first CSS framework with custom design tokens
- **Shadcn/ui**: Pre-built component library with consistent design system
- **Google Fonts**: Inter font family for typography
- **Material Icons**: Icon system for consistent visual elements

### Development Tools
- **Replit Integration**: Development environment optimization with banner and cartographer plugins
- **PostCSS**: CSS processing with Tailwind and Autoprefixer
- **ESBuild**: Fast JavaScript bundling for production builds

### Real-time Communication
- **WebSocket (ws)**: Native WebSocket implementation for real-time chat
- **Automatic Reconnection**: Client-side reconnection logic for connection stability

### Form and Validation
- **React Hook Form**: Form state management with validation
- **Hookform Resolvers**: Integration between React Hook Form and Zod schemas
- **Zod**: Runtime type validation and schema definition

### Utility Libraries
- **Date-fns**: Date manipulation and formatting
- **Clsx & Class Variance Authority**: Conditional CSS class management
- **Nanoid**: Unique ID generation for various entities