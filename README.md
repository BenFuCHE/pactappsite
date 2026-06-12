# Pact support site

Static launch pages for `pactapp.tech`.

## App Store URLs

- Support URL: `https://pactapp.tech/support`

## Local preview

```sh
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## Recommended deployment

The simplest path is GitHub Pages:

1. Create a GitHub repository for this folder.
2. Push these files to the `main` branch.
3. In GitHub, go to Settings -> Pages.
4. Set Source to "Deploy from a branch".
5. Choose `main` and `/root`.
6. Add the custom domain `pactapp.tech`.
7. In your domain DNS, point `pactapp.tech` to GitHub Pages.

GitHub Pages supports the included `CNAME` file and will serve:

- `https://pactapp.tech/`
- `https://pactapp.tech/support/`

## DNS records for GitHub Pages

For the apex domain, add these A records:

```text
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

For `www`, add a CNAME record:

```text
www -> ben-fu.github.io
```

Replace `ben-fu.github.io` with your actual GitHub Pages hostname if your
GitHub username or organization is different.
