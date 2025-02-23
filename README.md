# Next.js 15 Client-Side Navigation Error with next/link

This repository demonstrates a common error encountered in Next.js 15 applications when using `next/link` for client-side navigation.  The error occurs when an invalid route is specified in the `href` prop, causing unexpected behavior or errors. The solution shows how to handle invalid routes gracefully. 

## Bug Description
When navigating to a non-existent route using `next/link`, Next.js might not handle this gracefully, possibly resulting in a 404 error or unexpected behavior. This issue becomes crucial when using dynamic routes or routes that might change based on user actions.

## Bug Solution
The solution demonstrates using an error boundary component (`ErrorBoundary`) which catches the error and shows a fallback UI for invalid routes.  Also, ensuring the routes within `next/link` are valid before rendering the component prevent the errors.