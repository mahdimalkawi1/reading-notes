# Read: Class 41

## React 4:

### Q1. Explain the concept of dynamic routes in Next.js and how they differ from static routes.

**Static Routes:**

- Generated at build time.
- Ideal for unchanging content like blog posts.
- Faster loading as HTML is pre-generated and cached.

**Dynamic Routes:**

- Generated at runtime.
- Suited for content dependent on real-time or changing data.
- File names in square brackets ([]) indicate placeholders.
- Slower loading compared to static routes.


### Q2. Describe the process of deploying a Next.js application. What are the key steps involved, and what are some deployment platforms you can use?

**Deploying a Next.js Application:**

1. **Build**: Create a production build with npm run build or yarn build.

2. **Choose Hosting**: Select a hosting platform for your app.

3. **Environment**: Set required environment variables.

4. **Deploy**: Upload built files to the platform.

5. **Domain & SSL**: Configure custom domain with SSL.

6. **Test**: Verify app functionality after deployment.

**Deployment Platforms:**

- **Vercel**: Next.js optimized, easy and scalable.
- **Netlify**: Continuous deployment, forms, functions.
- **AWS Amplify**: Automatic deployment, scalable hosting.
- **Heroku**: Simple deployment, supports Next.js.
- **GitHub Pages**: Basic static site hosting.
- **DigitalOcean**: Flexible VMs, Kubernetes.
- **Firebase Hosting**: Fast, Google-powered hosting.

### Q3. How does Next.js handle static file serving? Discuss the default folder structure for storing static assets and explain how to reference them in a Next.js application.

**Static File Serving in Next.js:**

Next.js serves static files through the public directory at the root of your app. Anything placed here is accessible directly from your app's root URL.

**Referencing Assets:**

- Images: ```<img src="/logo.png" alt="Logo" />```
- Stylesheets: ```<link rel="stylesheet" href="/styles.css" />```
- Other assets: Reference with / prefix, e.g., /myfont.woff2.



