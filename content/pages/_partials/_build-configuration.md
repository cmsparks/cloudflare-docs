---
_build:
  publishResources: false
  render: never
  list: never

buildConfigs:
  create-react-app:
    displayName: Create React App
    buildCommand: npm run build
    buildOutputDirectory: build
  gatsby:
    displayName: Gatsby
    buildCommand: gatsby build
    buildOutputDirectory: public
  keywork:
    displayName: Keywork
    buildCommand: yarn build
    buildOutputDirectory: dist
  next-js:
    displayName: Next.js
    buildCommand: npx @cloudflare/next-on-pages@1
    buildOutputDirectory: .vercel/output/static
  next-js-static:
    displayName: Next.js (Static HTML Export)
    buildCommand: next build && next export
    buildOutputDirectory: out
  nuxt-js:
    displayName: Nuxt.js
    buildCommand: npm run build
    buildOutputDirectory: dist
  qwik:
    displayName: Qwik
    buildCommand: npm run build
    buildOutputDirectory: dist
  remix:
    displayName: Remix
    buildCommand: npm run build
    buildOutputDirectory: public
  svelte:
    displayName: Svelte
    buildCommand: npm run build
    buildOutputDirectory: public
  sveltekit:
    displayName: SvelteKit
    buildCommand: npm run build
    buildOutputDirectory: .svelte-kit/cloudflare
  vue:
    displayName: Vue
    buildCommand: npm run build
    buildOutputDirectory: dist
  astro:
    displayName: Astro
    buildCommand: npm run build
    buildOutputDirectory: dist
  angular-cli:
    displayName: Angular (Angular CLI)
    buildCommand: ng build --prod
    buildOutputDirectory: dist
  brunch:
    displayName: Brunch
    buildCommand: brunch build --production
    buildOutputDirectory: public
  docusaurus:
    displayName: Docusaurus
    buildCommand: npm run build
    buildOutputDirectory: build
  eleventy:
    displayName: Eleventy
    buildCommand: eleventy
    buildOutputDirectory: _site
  ember-js:
    displayName: Ember.js
    buildCommand: ember build
    buildOutputDirectory: dist
  gitbook:
    displayName: GitBook
    buildCommand: gitbook build
    buildOutputDirectory: _book
  gridsome:
    displayName: Gridsome
    buildCommand: gridsome build
    buildOutputDirectory: dist
  hugo:
    displayName: Hugo
    buildCommand: hugo
    buildOutputDirectory: public
  jekyll:
    displayName: Jekyll
    buildCommand: jekyll build
    buildOutputDirectory: _site
  mkdocs:
    displayName: Mkdocs
    buildCommand: mkdocs build
    buildOutputDirectory: site
  pelican:
    displayName: Pelican
    buildCommand: pelican content
    buildOutputDirectory: output
  react-static:
    displayName: React Static
    buildCommand: react-static build
    buildOutputDirectory: dist
  slate:
    displayName: Slate
    buildCommand: ./deploy.sh
    buildOutputDirectory: build
  umi:
    displayName: Umi
    buildCommand: umi build
    buildOutputDirectory: dist
  vuepress:
    displayName: VuePress
    buildCommand: vuepress build
    buildOutputDirectory: .vuepress/dist
  zola:
    displayName: Zola
    buildCommand: zola build
    buildOutputDirectory: public
---