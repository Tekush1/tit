# TIT Developer Community Website

## Overview

This website serves as the online presence for the TIT (Technocrats Institute of Technology) Developer Community. It aims to provide information about the community, its activities, members, and resources. The site is built using modern web development technologies to ensure a responsive, engaging, and performant user experience.

## Technologies Used

*   **Frontend:**
    *   **React:** A JavaScript library for building user interfaces.
    *   **TypeScript:** A superset of JavaScript that adds static typing.
    *   **Tailwind CSS:** A utility-first CSS framework for rapid UI development.
    *   **Lucide React:** A library of beautiful, consistent icons.
    *   **Framer Motion:** A motion library for React to create animations and transitions.
    *   **GSAP (GreenSock Animation Platform):** A JavaScript library for creating high-performance animations.
    *   **React Router DOM:** For navigation and routing within the application.
    *   **React Intersection Observer:** To detect when an element enters or leaves the viewport.
    *   **React Lazy Load Image Component:** For lazy loading images to improve performance.
    *   **@headlessui/react:** For accessible and unstyled UI components.
    *   **Howler:** For audio playback.
    *   **Three.js:** A JavaScript 3D library.
    *   **@react-three/fiber:** A React renderer for Three.js.
    *   **@react-three/drei:** Useful helpers for react-three-fiber.
    *   **Swiper:** For creating carousels and sliders.
*   **Build Tool:**
    *   **Vite:** A fast build tool and development server.
    *   **vite-plugin-image-optimizer:** For optimizing images during the build process.
*   **Other:**
    *   **ESLint:** For linting JavaScript and TypeScript code.
    *   **PostCSS:** For transforming CSS with plugins.

## Project Structure

The project structure is organized as follows:

vite-react-typescript-starter/
├── .bolt/                     # Bolt-related configuration (if applicable)
├── node_modules/              # Node.js dependencies (not typically in README)
├── public/                    # Static assets (images, fonts, etc.)
│   ├── vite.svg               # Vite logo
│   └── ...
├── src/                       # Source code directory
│   ├── audio/                 # Audio files and logic
│   │   └── gameAudio.ts       # Manages game audio
│   ├── components/            # React components
│   │   ├── forms/             # Form components
│   │   │   ├── BecomeMentorForm.tsx
│   │   │   ├── BookSessionForm.tsx
│   │   │   └── RegisterForm.tsx
│   │   ├── sections/          # Reusable sections for pages
│   │   │   ├── CallToActionSection.tsx
│   │   │   ├── FeaturesSection.tsx
│   │   │   ├── HeroSection.tsx
│   │   │   ├── ImpactSection.tsx
│   │   │   └── TimelineSection.tsx
│   │   ├── shared/            # Shared components
│   │   │   ├── ErrorBoundary.tsx
│   │   │   ├── Image.tsx
│   │   │   └── Modal.tsx
│   │   ├── About.tsx            # About section component
│   │   ├── ArrivalAnimation.tsx # Initial animation component
│   │   ├── CountUp.tsx          # Count-up animation component
│   │   ├── Dashboard.tsx        # Dashboard component
│   │   ├── DynamicText.tsx      # Dynamic text component
│   │   ├── Events.tsx           # Events section component
│   │   ├── FloatingCube.tsx     # 3D cube component
│   │   ├── Footer.tsx           # Footer component
│   │   ├── Gallery.tsx          # Gallery component
│   │   ├── HallOfFame.tsx       # Hall of Fame component
│   │   ├── Home.tsx             # Home section component
│   │   ├── Join.tsx             # Join section component
│   │   ├── Mentors.tsx          # Mentors section component
│   │   ├── Navigation.tsx       # Navigation component
│   │   ├── ParticleBackground.tsx # Particle background component
│   │   ├── Profile.tsx          # Profile component
│   ├── pages/                 # React pages
│   │   ├── AboutPage.tsx
│   │   ├── DashboardPage.tsx
│   │   ├── EventsPage.tsx
│   │   ├── GalleryPage.tsx
│   │   ├── HallOfFamePage.tsx
│   │   ├── HomePage.tsx
│   │   ├── JoinPage.tsx
│   │   ├── MentorsPage.tsx
│   │   ├── ProfilePage.tsx
│   │   └── TryPreparationPage.tsx
│   ├── App.tsx                # Main application component
│   ├── index.css              # Global CSS styles
│   ├── main.tsx               # Entry point for React
│   ├── vite-env.d.ts          # TypeScript environment declarations
├── .eslintrc.cjs            # ESLint configuration
├── index.html               # Main HTML file
├── package.json             # Project dependencies and scripts
├── postcss.config.js        # PostCSS configuration
├── tailwind.config.js       # Tailwind CSS configuration
├── tsconfig.app.json        # TypeScript application configuration
├── tsconfig.json            # Main TypeScript configuration
├── tsconfig.node.json       # TypeScript Node.js configuration
├── vite.config.ts           # Vite configuration
└── README.md                # Project documentation (this file)



## Setup Instructions

Follow these steps to set up the website locally:

1.  **Install Node.js:** Make sure you have Node.js installed on your system. You can download it from [https://nodejs.org/](https://nodejs.org/).
2.  **Clone the Repository:** Clone the project repository to your local machine.
    ```bash
    git clone [repository URL]
    cd [project directory]
    ```
3.  **Install Dependencies:** Install the required Node.js packages using npm.
    ```bash
    npm install
    ```
4.  **Run the Development Server:** Start the Vite development server.
    ```bash
    npm run dev
    ```
    This will start the development server and open the website in your browser (usually at `http://localhost:5173/`).

## Building for Production

To build the website for production, follow these steps:

1.  **Build the Project:** Run the Vite build command.
    ```bash
    npm run build
    ```
    This will create an optimized build of the website in the `dist` directory.
2.  **Deploy the `dist` Directory:** Deploy the contents of the `dist` directory to your web server or hosting provider.

## Key Components and Features

*   **Arrival Animation:** The `ArrivalAnimation` component provides an engaging initial loading experience with animated messages and a cinematic opening.
*   **Dynamic Text:** The `DynamicText` component animates a sequence of words, creating a dynamic and eye-catching effect.
*   **Floating Cube:** The `FloatingCube` component uses Three.js to render an interactive 3D cube.
*   **Impact Section:** The `ImpactSection` component showcases key statistics and achievements of the community using animated count-up numbers.
*   **Mentors Section:** The `Mentors` component displays a list of mentors with their expertise and allows users to book sessions.
*   **Gallery:** The `Gallery` component displays photos from community events.
*   **Modals:** Reusable modal components are used for forms and other interactive elements.
*   **Forms:** The project includes several form components for user registration, mentor applications, and session booking.
*   **Lazy Loading:** Images are lazy-loaded using the `react-lazy-load-image-component` to improve performance.
*   **Responsive Design:** The website is designed to be responsive and work well on different screen sizes.

## Configuration

*   **Tailwind CSS:** The Tailwind CSS configuration is located in `tailwind.config.js`. You can customize the theme, colors, fonts, and other settings in this file.
*   **Vite:** The Vite configuration is located in `vite.config.ts`. You can customize the build process, plugins, and server settings in this file.
*   **ESLint:** The ESLint configuration is located in `eslint.config.js`. You can customize the linting rules in this file.

## Contributing

Contributions to the website are welcome! To contribute, follow these steps:

1.  Fork the repository.
2.  Create a new branch for your feature or bug fix.
3.  Make your changes and commit them with descriptive commit messages.
4.  Push your changes to your fork.
5.  Submit a pull request.

## License

This project is licensed under the [License Name] License.



