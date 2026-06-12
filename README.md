# Pact support site

Static launch pages for `pactapp.tech`, deployed from the `pactapp-site`
repository.

## App Store URLs

- Support URL: `https://pactapp.tech/support`

## Local preview

```sh
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## Deployment

This site is hosted with Cloudflare Workers & Pages from GitHub.

After editing locally:

```sh
git status
git add .
git commit -m "Update Pact support site design"
git push
```

Cloudflare will automatically redeploy from the `main` branch.

The live URLs are:

- `https://pactapp.tech/`
- `https://pactapp.tech/support/`
