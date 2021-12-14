# Nuxt build bug

1. Clone this repo
2. run `npm i`
3. run `npx nuxt build` (or `npm run build`)
    - expected: Nuxt builds a server application with client side rendering
    - actual: Nuxt generates a static site with client side rendering

Notes:
- this is a default project created with `npx create-nuxt-app` and nothing else added
- in my actual project I also have a serverMiddleware API (which is the reason I need `target: "server"`) but since the reproduction works without it I didn't include it here
