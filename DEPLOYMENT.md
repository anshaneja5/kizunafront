# Frontend Deployment Guide

## Vercel Deployment Configuration

### Build Settings:
- **Framework Preset:** Vite
- **Build Command:** `npm run build`
- **Output Directory:** `dist`
- **Install Command:** `npm install`

### Environment Variables Required:
```
VITE_BACKEND_URL=https://your-backend-url.onrender.com
```

### Deployment Steps:

1. **Connect to Vercel:**
   - Go to https://vercel.com
   - Connect your GitHub repository
   - Select the `kizunafront` directory

2. **Set Environment Variables:**
   - In Vercel dashboard, go to Project Settings > Environment Variables
   - Add: `VITE_BACKEND_URL` = `https://your-backend-url.onrender.com`

3. **Deploy:**
   - Vercel will automatically deploy on every push to main branch

### Custom Domain (Optional):
- Add custom domain in Vercel dashboard
- Configure DNS settings as instructed

## Local Development Setup

1. Create `.env.local` file:
```
VITE_BACKEND_URL=http://localhost:5000
```

2. Install dependencies:
```bash
npm install
```

3. Run development server:
```bash
npm run dev
``` 