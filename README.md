# NudgeQuest

NudgeQuest is an AI-powered mock job interview platform that helps users prepare for real interviews. Users enter job role details, and the platform curates role-specific questions using the OpenAI API. It features real-time webcam and audio recording, converting responses to text for AI-based analysis and feedback. Built with Next.js, PostgreSQL, and ShadCN, NudgeQuest provides tailored interview practice and actionable insights. Live on Vercel.

[Project PPT & Report](https://drive.google.com/drive/u/0/folders/1-UFM38bdFFD-zzqu34LPo5SoM_2yP4M-)

## Table of Contents

- [About](#about)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [Features](#features)
- [Use Cases](#use-cases)
- [Getting Started](#getting-started)
- [Deployment](#deployment)
- [Contributing](#contributing)
- [License](#license)



## About

NudgeQuest allows users to simulate real interview scenarios and get instant feedback on their performance. The platform leverages machine learning and AI-powered features, such as real-time analysis of recorded answers, to help users improve their responses.

Key features include:
- Customizable interview questions based on the job role
- Real-time webcam and audio recording for responses
- AI-driven feedback and insights on performance
- Dashboard for tracking interview progress and feedback

## Technologies Used

| **Technology**     | **Usage**                                                       |
|--------------------|---------------------------------------------------------------|
| **Frontend**       | Next.js, React.js, Tailwind CSS                                 |
| **Backend**        | Node.js, Express.js, OpenAI API                                |
| **Database**       | PostgreSQL                                                     |
| **UI Framework**   | ShadCN, Tailwind UI                                             |
| **Deployment**     | Vercel                                                         |

---

## Key Functionalities

### For Job Seekers:
- Prepare for interviews with personalized, role-specific questions.
- Record real-time webcam and audio responses.
- Receive AI-based feedback on interview performance.

### For Recruiters/HR Professionals:
- Simulate mock interviews for candidates.
- Analyze responses using AI for a detailed evaluation.
- Provide candidates with actionable feedback for improvement.

---




# NudgeQuest Project Structure

## Folder/File Overview

| Folder/File                               | File Path                                      | Use                                                                 |
|-------------------------------------------|------------------------------------------------|---------------------------------------------------------------------|
| **Authentication**                        | `auth/sign-in/[[...sign-in]]/page.jsx`         | Sign-in page logic                                                 |
|                                           | `auth/sign-up/[[...sign-up]]/page.jsx`         | Sign-up page logic                                                 |
| **Home**                                  | `home/Drawerx.jsx`                             | Drawer component in the homepage                                   |
|                                           | `home/Homeheader.jsx`                          | Header for the home page                                           |
|                                           | `home/TeamSection.jsx`                         | Team section component for the homepage                            |
|                                           | `home/Timeline.jsx`                            | Timeline section for the homepage                                  |
|                                           | `home/down.jsx`                                | Bottom section of the homepage                                     |
|                                           | `home/qa.jsx`                                  | Q&A section for the homepage                                       |
| **Dashboard**                             | `dashboard/_components/AddNewInterview.jsx`     | Component to add a new interview                                   |
|                                           | `dashboard/_components/Header.jsx`             | Header for the dashboard page                                      |
|                                           | `dashboard/_components/InterviewItemCard.jsx`   | Card component for individual interviews                           |
|                                           | `dashboard/_components/InterviewList.jsx`       | List of interviews in the dashboard                                |
|                                           | `dashboard/interview/[interviewId]/`            | Dynamic interview details page                                     |
|                                           | `dashboard/feedback/page.jsx`                  | Feedback page for interviews                                       |
| **Start**                                 | `start/_components/QuestionsSection.jsx`        | Section to show questions in the interview process                 |
|                                           | `start/_components/RecordAnswerSection.jsx`     | Section to record answers during the interview process             |
|                                           | `start/page.jsx`                               | Main page for the start section                                    |
|                                           | `start/layout.jsx`                             | Layout for the start section                                       |
| **UI Components**                         | `components/ui/accordion.jsx`                  | Accordion component for UI                                         |
|                                           | `components/ui/button.jsx`                     | Button component for UI                                            |
|                                           | `components/ui/collapsible.jsx`                | Collapsible component for UI                                       |
|                                           | `components/ui/dialog.jsx`                     | Dialog component for UI                                            |
|                                           | `components/ui/drawer.jsx`                     | Drawer component for UI                                            |
|                                           | `components/ui/input.jsx`                      | Input field component for UI                                       |
|                                           | `components/ui/select.jsx`                     | Select dropdown component for UI                                   |
|                                           | `components/ui/sonner.jsx`                     | Sonner component for UI                                            |
|                                           | `components/ui/textarea.jsx`                   | Textarea component for UI                                          |
| **Utilities (Lib)**                       | `lib/utils.js`                                  | Utility functions for the app                                      |
| **Public Assets**                         | `public/NudgeQues_logo-Photoroom.png`           | Logo image for the platform                                        |
|                                           | `public/dreamjob2.png`                         | Dream job image                                                     |
|                                           | `public/dreamjob4.png`                         | Dream job image                                                     |
|                                           | `public/ex.svg`                                | SVG image for the platform                                         |
|                                           | `public/jobqueue.png`                          | Job queue image                                                     |
|                                           | `public/logo.svg`                              | Logo image in SVG format                                           |
|                                           | `public/lovejob.jpg`                           | Love job image                                                      |
|                                           | `public/lovejob3.jpg`                          | Love job image                                                      |
|                                           | `public/next.svg`                              | Next icon SVG                                                       |
|                                           | `public/vercel.svg`                            | Vercel logo SVG                                                    |
|                                           | `public/walk.png`                              | Walk image                                                          |
|                                           | `public/webcamera.png`                         | Web camera image                                                    |
| **Utilities (Files)**                     | `utils/GeminiAIModal.js`                        | Modal for Gemini AI functionality                                  |
|                                           | `utils/db.js`                                  | Database connection and logic                                     |
|                                           | `utils/schema.js`                              | Database schema definition                                         |
| **Root Files**                            | `.gitignore`                                   | Specifies which files to ignore in version control                 |
|                                           | `README.md`                                    | Project documentation file                                         |
|                                           | `components.json`                               | Configuration file for components                                  |
|                                           | `drizzle.config.js`                             | Drizzle configuration file for database interactions               |
|                                           | `jsconfig.json`                                 | JavaScript configuration file for path aliasing                   |
|                                           | `middleware.js`                                 | Middleware logic for the app                                      |
|                                           | `next.config.mjs`                               | Next.js configuration file                                         |
|                                           | `package-lock.json`                             | Lock file for dependencies                                         |
|                                           | `package.json`                                  | Project dependencies and metadata                                  |
|                                           | `postcss.config.mjs`                            | Configuration file for PostCSS                                     |
|                                           | `tailwind.config.js`                            | Configuration file for Tailwind CSS                                |



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

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.js`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
