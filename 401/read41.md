# Dynamic Routs
Next.js allows you to statically generate pages with paths that depend on external data.

**steps**

1. Implement getStaticPaths
2. Implement getStaticProps
3. Render Markdown: To render markdown content, we’ll use the remark library `npm install remark remark-html`
4. Polishing the Post Page
5. Formatting the Date: To format the date, we’ll use the date-fns library `npm install date-fns`
6. Adding CSS
7. Polishing the Index Page
8. Fetch External API or Query Database
9. Development v.s. Production:
  - In development (npm run dev), getStaticPaths runs on every request.
  - In production, getStaticPaths runs at build time.


------------------


# Next.js Deploying

**steps**

1. Push to GitHub
2. Deploy to Vercel by:
  - Create a Vercel Account
  - Import your nextjs-blog repository

## Next.js and Vercel
Vercel is made by the creators of Next.js and has first-class support for Next.js.
Vercel is a serverless platform for static and hybrid applications built to integrate with your headless content, commerce, or database.

### Develop, Preview, Ship
- Develop: We’ve written code in Next.js and used the Next.js development server running to take advantage of its hot reloading feature.
- Preview: We’ve pushed changes to a branch on GitHub, and Vercel created a preview deployment that’s available via a URL. We can share this preview URL with others for feedback.
- Ship: We’ve merged the pull request to main to ship to production.


<p style='color:#000B49'>resources</p>
<a href='https://canvas.instructure.com/courses/3671304/assignments/25742387/submissions/30664666'> read link </a>

1. <a href='https://nextjs.org/learn/basics/dynamic-routes'>next.js dynamic-routes</a>
2. <a href='https://nextjs.org/learn/basics/deploying-nextjs-app'>next.js deployment</a>
