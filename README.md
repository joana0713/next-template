## 🚧 Project Status

This template is currently under development.

There is a known build issue related to configuration setup.
The project structure is completed, and the issue will be resolved in the next update.

## ⚠️ Known Issues

- Build error during `npm run build`
- Possible cause: Next.js app directory configuration

## ⚠️ Reason
- There was no page.tsx file.
- error in import part
- src/app/... so in all import part, have to consider...

## 👌 Fix
- Create page.tsx in src/app folder.
- In next.config.ts, input the following codes.

    import path from "path";
    sassOptions: {
        includePaths: [path.join(__dirname, "src/styles")],
    },

## 🛠 Tech Stack

- Next.js
- TypeScript
- Tailwind CSS

## 📦 Installation

```bash
npm install
npm run dev