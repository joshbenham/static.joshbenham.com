# DEPLOY.md

## Deploy to Cloudflare Pages

This is a static site. Build CSS first, then upload `public/`.

## Local build

```bash
npm install
npm run build
```

That generates:

```text
public/assets/app.css
```

## Direct Upload
1. Log into Cloudflare
2. Go to **Workers & Pages**
3. Create a new **Pages** project
4. Choose **Direct Upload**
5. Upload the contents of the `public/` folder

## Git Deploy
1. Push this project to GitHub
2. In Cloudflare Pages choose **Connect to Git**
3. Build command:

```bash
npm run build
```

4. Output directory:

```text
public
```

## Custom Domain
Add `joshbenham.com` in the project’s **Custom domains** settings.
