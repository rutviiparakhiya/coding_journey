NEXT JS (Full stack framework)   
Next.js is a React-based full-stack framework for building modern web applications.     

it is a framework built on top of React.js that enables developers to build server-side rendered and statically generated web applications. It provides features like automatic code splitting, optimized performance, and easy routing.   

◯ Diffrence between library and framework :-   
| library | framework |
| :---: | :---: |
| it provides specific functionality that we can use when needed. | provides a complete structure for building an application. |
| The developer controls the application flow. | The framework controls the overall application flow. |
| We choose when and where to use it. | We follow its rules and conventions. |
| Example: React | Example: Next.js |

◯ Why we use next js?   
Next.js is a React-based framework used to build fast, SEO-friendly, and full-stack web applications.    
it provides built in features such as file based routing, multiple rendering strategies, server side capabilites, data fetching, image optimization, and TypeScript support and These features reduce the need to configure everything manually and make application development easier and more efficient.   

◯ Diffrence between app router and page router :-
| app router | page router |
| :----------: | :-----------: |
|            |             |

◯ File-based-routing :- The application's routing system is automatically determined by the structure of your files and folders.   

□ Type of file base routing :-
1. static routes - they are pages with fixed URLs, such as /about, /contact, and /pricing.   
2. nested routes - they are created by putting folders inside other folders to create subpages, such as /dashboard/settings.    
3. dynamic routes - they are used when a part of the URL changes, using square brackets like [id], such as /products/1 or /products/25.   

□ Method of getting values from url :-
1. route parameters - they take values from dynamic URL segments, such as id = "25" in /products/25, to identify which resource the page &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; displays.    
2. search parameters - the values written after ? in a URL, used for searching, filtering, sorting, or pagination, such as /products? &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; search=phone.    

◯ Diffrence between route parametere and search parametere :-    
| route parametere                 | search parametere                   |
| :--------------------------------: | :-----------------------------------: |
| Gets the value from the URL path | Gets the value after ? in the URL.  |
| To identify a specific resource. | Search, filter, sorting, pagination |
| e.g. - /products/25              | e.g. - /products?search=phone       |

◯ Diffrence between Catch-All Routes [...slug] and Optional Catch-All Routes [[...slug]] :-  
| Catch-All Routes [...slug]                          | Optional Catch-All Routes [[...slug]]                               |
| :---------------------------------------------------: | :-------------------------------------------------------------------: |
| Matches one or more URL segments                    | Matches zero or more URL segments.                                  |
| we should use When at least one segment is required | we should use When the base route and nested routes are both needed |
| /docs is not matched                                | /docs is matched                                                    |

◯ navigation with link :- In Next.js, Link is used to navigate from one page to another without fully reloading the page.    

◯ Layout :- It provides shared UI for multiple pages, such as a Navbar and Footer.    

layout concepts and benifits :   
1. root layout - it wraps all pages and contains the required html and body tags.  
2. Shared UI with a Layout - A layout allows multiple pages to use the same UI, such as a Navbar and Footer, without repeating the code.  
3. nested layout - it allows a route segment to have its own layout inside the root layout, sharing UI such as a sidebar across its subpages.  
4. Layout Persistence - it means the layout remains mounted while navigating between routes that share the same layout, and only the page &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; content changes.  
5. layout Hierarchy - it is the order in which multiple nested layouts wrap a page, from the root layout to the innermost layout.
6. Different Layouts for Different Sections - Different sections of an application can use different layouts, and route groups ( ) help organize them without changing the URL.  

◯ Server Components :- That run on the server by default in Next.js App Router and are mainly used for fetching data and accessing server-side resources.  

◯ Client Components :- They are components that use "use client" to enable interactivity, React hooks, event handlers, and browser APIs in Next.js.  
"use clinet" - It is a directive used at the top of a file to create a Client Component boundary when client-side features are required.  

◯ "use server" - It is a directive used to define Server Functions that perform server-side operations, such as database updates and server-side validation.  

◯ Data Fetching - Data fetching means retrieving data from sources like APIs, databases, or files to display it in a page or component.  
there are 2 methods of data fetching :  
1. Sequential Fetching - Fetching data one request at a time, waiting for each request to finish before starting the next.  
2. Parallel Fetching - Fetching multiple independent requests at the same time to save time.  

◯ Server side & clinet side data fetching :-   
| serever side data fetching                        | clinet side data fetching                        |
| :-------------------------------------------------: | :------------------------------------------------: |
| it runs on server                                 | it runs on browser                               |
| best for initial page data                        | best for interactive data                        |
| it Can access databases and server-only resources | it Uses browser-accessible resources             |
| we Can keep secret keys on the server             | we Cannot safely store server secrets            |
| Usually Server Components                         | Usually Client Components                        |
| e.g. - Fetching products when a page loads        | e.g. - Fetching search results when a user types |

◯ UI Loading State :- A loading state shows a message or UI while data is being fetched or page content is being prepared.
there are 2 types of creating ui states :
1. loading.tsx: Displays loading UI for a route segment and its child routes.
2. Suspense: Displays fallback UI while a specific component or section is waiting for data.

◯ Error Handling :- Error handling means displaying a useful error message when something goes wrong, such as an API failure or network error.

◯ Why error.tsx Is a Client Component :- 
error.tsx must use "use client" because it uses client-side features such as the reset() function and interactive buttons.
reset() Function - The reset() function attempts to render the route again after an error.

◯ Error Boundary :- An Error Boundary catches rendering errors and displays fallback UI instead of the broken part of the application.

◯ Error Flow :- fetch() → Error thrown → Error Boundary → error.tsx → Error UI

◯ Rendering :- Rendering is the process of generating the UI that the browser displays.

◯ CSR(Client-Side Rendering) :-   
CSR means fetching data and rendering or updating the UI in the browser after JavaScript loads.   
□ How it works : Browser → Load JavaScript → React Runs → Fetch API → Update UI   
□ When to Use : Interactive dashboards, Chat applications, Client-side search and filtering, Real-time updates, Complex forms and drag-and-drop interfaces.    
□ advantages : Provides interactive user experiences, Works well for browser-dependent interactions, Updates UI without reloading the entire page.    
□ disadvabtages : Search engine indexing can be less straight forward for content rendered only in the browser, Can increase  initial loading time if substantial JavaScript is required, Some content may appear only after JavaScript runs and data loads.  

◯ Static Rendering :- Static Rendering means generating a page before the user requests it and reusing the generated result for multiple users.   
□ how it works : Build / Static Generation → Generate HTML → Store / Cache Result → User Request → Serve Existing Result   
□ advantages : Fast responses, Good scalability, Good SEO, Less server work for each request     
□ disadvantages : Content may become outdated if it is not regenerated, Not suitable for highly personalized content that changes for each user : Content updates may require rebuilding or revalidating the page.    

◯ Dynamic Rendering :- Dynamic Rendering means generating a page on the server at request time using request-specific information or data.   
□ How it works : User Request → Next.js Server → Fetch / Calculate Data → Generate Response → Browser    
□ advantages : Handles request-specific information, Works with cookies and authentication, Supports personalized content for each user, Displays up-to-date data.   
□ disadvantages : Can increase server costs under heavy traffic, Requires more server processing for each request, May have slower response times than static rendering.   

◯ Diffrence between dynamic routing and static routing :-
| static rendering                        | dynamic rendering                              |
| :---------------------------------------: | :----------------------------------------------: |
| Result can be reused for multiple users | Result depends on request-specific information |
| Best for shared public content          | Best for personalized content                  |
| Generate ahead of the request           | Generate for the request                       |
| Includes SSG and ISR                    | Closely related to SSR                         |

◯ SSR — Server-Side Rendering :- SSR means generating HTML on the server for a user's request.
How it works : User Request → Next.js Server → Fetch Request-Specific Data → Generate HTML → Browser → Hydration
When to Use SSR / Dynamic Rendering : Data that must be fetched at request time, Personalized feeds, Order details, Authenticated dashboards, User profiles
advantages : Can display request-specific and up-to-date data, Supports personalized content, Can display request-specific and up-to-date data.
disadvantages : May be slower than serving a cached static page, Requires more server resources under heavy traffic, Can increase response time because the server performs work for each request.

◯ SSG — Static Site Generation :- SSG means generating pages ahead of time, usually during the build, so the generated result can be reused for multiple requests.
How it works : Build → Fetch Data → Generate Page → Store / Cache Result → Serve to Users
When to Use SSG : Product pages with known IDs, Blogs, Documentation, About and pricing pages
Advantages : Good scalability, Less work for the server on each request, Good SEO, Fast page delivery
Disadvantages : Not ideal for content that must change for every user's request, Rebuilding many pages can take time, Content can become outdated until regenerated.

◯ ISR — Incremental Static Regeneration(Static Rendering + Revalidation) :- ISR means updating statically generated pages after a specified time or when revalidation is triggered, without rebuilding the entire application.
How it works : Generate Static Page → Serve Cached Page → Revalidate → Regenerate Page → Serve Updated Version
When to Use ISR : Travel listings, Real-estate listings, Blog listings, News websites, Product catalogs
Advantages: Fast responses from cached pages, Content can be refreshed without rebuilding the entire application, Reduces repeated server work. 
Disadvantages: Content may remain outdated until revalidation occurs, Regeneration can add server work, Revalidation timing and cache behavior require careful configuration.

