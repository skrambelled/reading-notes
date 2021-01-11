# Next.js II

## Data fetching

Next.js pre-renders every page, rather than relying on clientside javascript to do so, which makes it both faster and also get better SEO results.

Each page gets only the minimal Javascript necesary for that page.

### static generation vs servser-side rendering

*static generation* is pre-rendered at build time, meaning the same page is served over and over

*server-side rendering* is pre-rendered for each request, so we are able to serve dynamic content

Static generation is preferred whenever possible, because it is much faster.

On any given page, you can `export async function getStaticProps()` then Next.js will go fetch those props ahead of time to statically generate the page. Normally, this is ran at build-time, but in dev mode it will be ran for every request.

IF you need to do server-side rendering use `export async function getServerSideProps()` instead.

## Dynamic routes

You can make pages with a name enclosed in square brackets, such as `/pages/posts/[id].js`, and that will allow dynamic routing based on the `id` being passed from the browser's URL.

You can catch all dynamic routes to beyond some endpoint using `/pages/posts/[...id]js` which will match `posts/a` and also `posts/a/b`

You can also `import useRouter from 'next/router'` to gain access to the router directly.

Next.js also supports creating API endpoints: `export default function handler(req, res) { //... }`

## Deployment

Vercel is Next.js deployment platform. You can link up yout guthub account to Vercel.

Using Vercel, you can set up custom domains, environment variables, and HTTPS.

When using Vercel we use a DPS workflow. Develop. Preview. Ship.

You can also deploy to any other provider that supports Node.js.

[<--- Back](../README.md)
