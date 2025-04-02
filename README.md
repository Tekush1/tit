
**Directory and File Descriptions:**

*   `.bolt/`: Contains Bolt-related configuration files, if the project uses Bolt.
*   `node_modules/`: Stores the Node.js dependencies installed by npm.
*   `public/`: Contains static assets such as images, fonts, and other files that don't require processing.
*   `src/`: The main source code directory for the React application.
    *   `audio/`: Contains audio files and the `gameAudio.ts` module for managing audio playback.
    *   `components/`: Houses reusable React components.
        *   `forms/`: Contains form components like `BecomeMentorForm.tsx`, `BookSessionForm.tsx`, and `RegisterForm.tsx`.
        *   `sections/`: Contains reusable sections for different pages, such as `HeroSection.tsx`, `ImpactSection.tsx`, etc.
        *   `shared/`: Contains shared components like `ErrorBoundary.tsx`, `Image.tsx`, and `Modal.tsx`.
        *   Other components: `About.tsx`, `ArrivalAnimation.tsx`, `CountUp.tsx`, `Dashboard.tsx`, `DynamicText.tsx`, `Events.tsx`, `FloatingCube.tsx`, `Footer.tsx`, `Gallery.tsx`, `HallOfFame.tsx`, `Home.tsx`, `Join.tsx`, `Mentors.tsx`, `Navigation.tsx`, `ParticleBackground.tsx`, `Profile.tsx`.
    *   `pages/`: Contains React components that represent different pages of the website.
        *   `AboutPage.tsx`, `DashboardPage.tsx`, `EventsPage.tsx`, `GalleryPage.tsx`, `HallOfFamePage.tsx`, `HomePage.tsx`, `JoinPage.tsx`, `MentorsPage.tsx`, `ProfilePage.tsx`, `TryPreparationPage.tsx`.
    *   `App.tsx`: The main application component that sets up routing and layout.
    *   `index.css`: Global CSS styles for the application.
    *   `main.tsx`: The entry point for the React application.
    *   `vite-env.d.ts`: TypeScript environment declarations for Vite.
*   `.eslintrc.cjs`: Configuration file for ESLint, a JavaScript and TypeScript linter.
*   `index.html`: The main HTML file that serves as the entry point for the website.
*   `package.json`: Contains project metadata, dependencies, and scripts for building and running the application.
*   `postcss.config.js`: Configuration file for PostCSS, a tool for transforming CSS with plugins.
*   `tailwind.config.js`: Configuration file for Tailwind CSS, a utility-first CSS framework.
*   `tsconfig.app.json`: TypeScript configuration file for the application.
*   `tsconfig.json`: Main TypeScript configuration file that references other configurations.
*   `tsconfig.node.json`: TypeScript configuration file for Node.js-related code.
*   `vite.config.ts`: Configuration file for Vite, a fast build tool and development server.
*   `README.md`: The project documentation file (this file).

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
