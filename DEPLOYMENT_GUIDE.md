# Free Static Hosting & Deployment Guide (GitHub Pages & Cloudflare Pages)

## Folder Structure
```text
data-career-bootcamp/
├── index.html              # Self-contained entry-point web application (Required)
├── research_dataset.json   # Standalone copy of verified job & resource dataset (Optional/Importable)
├── README.md               # Repository overview & architecture documentation
└── DEPLOYMENT_GUIDE.md     # Step-by-step hosting & maintenance instructions
```

## Option 1: GitHub Pages (Recommended — Simplest Setup, $0 Cost)
1. Sign in to [GitHub](https://github.com/) and create a new **Public** repository named `data-career-bootcamp`.
2. Upload `index.html`, `README.md`, `DEPLOYMENT_GUIDE.md`, and `research_dataset.json` to the repository root.
3. Open **Settings** -> **Pages** in your GitHub repository.
4. Under **Build and deployment -> Source**, choose **Deploy from a branch**.
5. Select branch `main` and folder `/ (root)`, then click **Save**.
6. Wait ~60 seconds and open `https://<your-username>.github.io/data-career-bootcamp/`.

## Option 2: Cloudflare Pages (Connected to GitHub)
1. Push your repository to GitHub.
2. Open [Cloudflare Pages](https://developers.cloudflare.com/pages/get-started/) -> **Create application -> Pages -> Connect to Git**.
3. Select your repository, leave **Build command** empty, and set **Build output directory** to `/`.
4. Click **Save and Deploy**. Every future `git push` automatically triggers a new deployment.
