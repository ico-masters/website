# TLDR Website

## Ruby version
- 2.5.1

## System dependencies
- Bundler

## How to install
```
$> bundle
```

## How to run in development mode
For local development I use the test-repo backend, which uses an in-memory object that is cleared with each refresh.

Make sure that *admin/config.yml* has this setup
```
backend:
  name: test-repo
```

then run on the console
```
$> jekyll server
```

and go to: http://127.0.0.1:4000

## How to deploy for staging
Make sure you revert *admin/config.yml* to:
```
backend:
  name: git-gateway
```

Open a PR with your changes, netlify.com will generate a test environment for QA to use.

and go to: https://tldrcapital.netlify.com

## Responsive images
- https://www.netlify.com/blog/2015/08/20/simple-responsive-images-with-jekyll/

Be sure to use: https://github.com/niveus/jekyll-srcset and not the https://github.com/netlify/jekyll-srcset one, because of this open issue: https://github.com/netlify/jekyll-srcset/issues/3

## Handy docs

- https://www.netlify.com/docs/
- https://www.netlify.com/blog/2017/08/17/a-complete-cms-with-no-server-and-18-lines-of-code/
- https://jekyllrb.com/docs/liquid/
- https://shopify.github.io/liquid/basics/introduction/

- https://www.youtube.com/watch?v=R4rLx6wTqMw

## Notes

The **netlify-cms** folder in this project, came from https://github.com/ico-masters/netlify-cms
