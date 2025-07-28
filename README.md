# AI Resume Analyzer

A modern, full-stack web application for analyzing resumes using AI, providing ATS (Applicant Tracking System) feedback and improvement tips. Built with React, React Router, TypeScript, Zustand, and TailwindCSS.

---

## Features

- **Resume Upload & Analysis:** Upload your resume (PDF), get AI-powered feedback and ATS scoring.
- **Job Context:** Input job title and description for tailored analysis.
- **Visual Feedback:** See scores and improvement tips across ATS, tone, content, structure, and skills.
- **History:** Track and review past resume submissions.
- **Authentication:** Secure login/logout flow.
- **Modern UI:** Responsive, accessible, and styled with TailwindCSS.

---

## Project Structure

```
app/
  components/    # Reusable UI components (ResumeCard, Details, ATS, FileUploader, etc.)
  lib/           # Utility logic (PDF to image, state management, helpers)
  routes/        # Route components (home, upload, resume, auth, wipe)
  root.tsx       # App root
  routes.ts      # Route definitions
constants/       # AI prompt templates and response formats
public/          # Static assets (images, icons)
```

---

## Getting Started

### 1. Install dependencies

```bash
npm install
```

### 2. Start the development server

```bash
npm run dev
```

Visit [http://localhost:5173](http://localhost:5173) in your browser.

---

## Building for Production

```bash
npm run build
```

---

## Deployment

### Docker

```bash
docker build -t ai-resume-analyzer .
docker run -p 3000:3000 ai-resume-analyzer
```

### Manual

Deploy the contents of the `build/` directory using any Node.js hosting or cloud provider.

---

## Key Technologies

- **React** & **React Router** (SPA, routing)
- **TypeScript** (type safety)
- **Zustand** (state management)
- **TailwindCSS** (styling)
- **pdfjs-dist** (PDF parsing)
- **Vite** (build tool)

---

## Customization

- **AI Feedback Logic:** See `constants/index.ts` for prompt templates and feedback format.
- **Routes:** Defined in `app/routes.ts`.
- **Components:** Located in `app/components/`.

---

## License

MIT
