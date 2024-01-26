# Pipelines

CI/CD pipelines.

## Hugo

+ `.cf-pages-deploy-ci.yml`: Build Hugo site using `hugo/.hugo-build-ci.yml` and deploy it to Cloudflare Pages via Wrangler direct upload.
+ `.gl-pages-deploy-ci.yml`: DEPRECIATED, switch from `hugo/.gl-pages-deploy-ci.yml` to `hugo/.hugo-build-ci.yml` for continued functionality. This pipeline will run as an alias for `hugo/.hugo-build-ci.yml` until removed.
+ `.hugo-build-ci.yml`: Build hugo site to the `public` dir, `public` will be exported as an artifact.

## NPM

+ `.npmjs-publish-ci.yml`: Publish NPM package, on tag creation, to the NPM registry.
