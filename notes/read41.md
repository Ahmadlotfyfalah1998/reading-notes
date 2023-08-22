[githup](https://ahmadlotfyfalah1998.github.io/reading-notes/)<BR>
## Q1.Explain the concept of dynamic routes in Next.js and how they differ from static routes.
Dynamic routes in Next.js allow you to create pages with URLs that have parameters, making it possible to handle variable data.<BR>
These parameters are indicated using brackets in the page file name (e.g., [id].js).<BR>
When a user accesses a dynamic route, Next.js generates the page on the server or at build time, depending on the scenario.<BR>
This enables the creation of personalized pages based on the dynamic content. In contrast, <BR>
static routes are pre-rendered during build time and do not involve parameterized URLs. They're suitable for pages with content that doesn't change frequently.<BR>

## Q2.Describe the process of deploying a Next.js application. What are the key steps involved, and what are some deployment platforms you can use?
Deploying a Next.js application involves several key steps. First, you build the application using the next build command.<BR>
Then, you can use various deployment platforms like Vercel, Netlify, or platforms like AWS, Heroku, and more. For Vercel and Netlify,<BR>
you typically connect your repository, configure build settings, and deploy directly from there. For other platforms,<BR>
you might set up a server to host the built files. The deployment process includes configuring environment variables, specifying build commands, <BR>
and handling routing (if needed). The deployment platform then takes care of deploying your application to the web.<BR>

## Q3.How does Next.js handle static file serving? Discuss the default folder structure for storing static assets and explain how to reference them in a Next.js application.
Next.js serves static files, like images or stylesheets, through its /public folder. This folder contains assets that remain unchanged during runtime.<BR>
For example, an image named my-image.jpg in the /public folder can be accessed at the URL /my-image.jpg.<BR>
This feature is efficient and doesn't involve any special routing. When referencing these static assets in your Next.js application,<BR>
you can use relative paths based on the root of the /public folder (e.g., /my-image.jpg).<BR>
These assets are served directly by the web server and don't go through the Next.js rendering process,<BR>
making them suitable for elements that don't require dynamic behavior.<BR>


## Things I want to know more about
NATLIFAY DEPLOYMENT 
