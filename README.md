# bytes.net.my

Website for Bytes IT Solution. Plain HTML and CSS, no build step.

## Files

| File | Page |
|---|---|
| `index.html` | Home |
| `about.html` | About us, vision, mission, values, company information |
| `services.html` | The 8 service areas with recent work |
| `projects.html` | Highlights and the full track record (filterable) |
| `credentials.html` | PUKONSA, DBKK licences, Anak Negeri, SST |
| `partners.html` | Dell and the state agencies we serve |
| `contact.html` | Email, phone, address and map |
| `404.html` | Shown when a page is not found |
| `styles.css` | Shared styles for every page |
| `assets/logo.png` | Logo |
| `CNAME` | Tells GitHub Pages to serve the site at bytes.net.my |
| `robots.txt`, `sitemap.xml` | Help Google find every page |

## Publish on GitHub Pages

1. Create a new repository on GitHub, for example `bytes-website`.
2. Upload every file and the `assets` folder to the root of the repository.
3. Go to **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, branch `main`, folder `/ (root)`, and save.
4. After a minute the site is live at `https://<your-username>.github.io/bytes-website/`.

## Point bytes.net.my to GitHub

In the DNS settings for bytes.net.my, add:

| Type | Name | Value |
|---|---|---|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | `<your-username>.github.io` |

Remove any old A or CNAME records for `@` and `www` first. Leave MX records alone so email at info@bytes.net.my keeps working.

Then in **Settings → Pages**, check that the custom domain shows `bytes.net.my`, wait for the DNS check to pass, and tick **Enforce HTTPS**. DNS changes can take up to 24 hours.

## Keep it up to date

- **New project:** add a row to the table in `projects.html`, then update the project count on `index.html`, `about.html`, `projects.html` and `partners.html`, and the bar chart on `index.html`.
- **Licence renewals:** update the validity dates in `credentials.html` and the registration panel on `index.html`. PUKONSA runs to 17/07/2028.
