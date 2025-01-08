# Effector Course Starter Project

This repository serves as the starter template for learning and demonstrating **Effector** in a **Next.js** project. It is designed to help students and developers quickly set up a Next.js application and dive into using Effector to manage state efficiently.

## Table of Contents

- [About Effector](#about-effector)
- [Features](#features)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Running the Project](#running-the-project)
- [Folder Structure](#folder-structure)
- [Effector in Action](#effector-in-action)
- [Contributing](#contributing)
- [License](#license)

## About Effector

[Effector](https://effector.dev/) is a powerful and fast state manager that allows you to build predictable and flexible state logic in JavaScript applications. Effector promotes clean architecture and is perfect for managing complex state scenarios, including:

- Reactive data flows
- Derived state
- Scoped state management
- Dependency management

## Features

- **Next.js Framework**: Full support for SSR (Server-Side Rendering) and static generation.
- **Effector Integration**: Pre-configured Effector setup for managing state across the application.
- **TypeScript Ready**: Built with TypeScript for type safety and better developer experience.
- **Prettier & ESLint**: Enforced code style and quality.

## Getting Started

### Prerequisites

Ensure you have the following tools installed:

- [Node.js](https://nodejs.org/) (version 18 or later)
- [npm](https://www.npmjs.com/) or [yarn](https://yarnpkg.com/)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/effector-course-starter.git
   ```

2. Navigate to the project folder:
   ```bash
   cd effector-course-starter
   ```

3. Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   ```

### Running the Project

1. Start the development server:
   ```bash
   npm run dev
   # or
   yarn dev
   ```

2. Open [http://localhost:3000](http://localhost:3000) in your browser to see the app in action.

## Effector in Action

The repository includes examples to help you learn Effector:

- **Basic Store**: Setting up a simple Effector store.
- **Reactive Updates**: Reactively updating components based on store changes.
- **Server-Side State**: Integrating Effector with Next.js SSR and static generation.

### Example Store

```typescript
import { createStore, createEvent } from 'effector';

export const increment = createEvent();
export const decrement = createEvent();

export const counter = createStore(0)
  .on(increment, (state) => state + 1)
  .on(decrement, (state) => state - 1);
```

## Contributing

We welcome contributions! To contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -m 'Add your feature'`).
4. Push the branch (`git push origin feature/your-feature`).
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Happy coding and enjoy learning Effector with Next.js!
