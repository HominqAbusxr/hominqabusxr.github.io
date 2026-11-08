# Tom Carter · Portfolio

A buildless portfolio and printable CV. The public pages use HTML, CSS, local SVG artwork and a small print-button script. The site works from a GitHub Pages project subdirectory as well as the root of `tomgc.com`.

## Preview and edit

Run `python3 -m http.server 8080` in the checkout and open `http://localhost:8080`. Edit `index.html` for the portfolio, `cv.html` for the CV and `assets/site.css` for layout and print styles. Use **Print / save PDF** on the CV to make a PDF with the browser's print dialog.

## Content to add next

- Lead with an e4education case study if you have a public site, archived URL or approved screenshot. Explain the original brief, the parts of the frontend you owned and one constraint that shaped the implementation.
- Add an approved screenshot or a short recording of the actual webOS fork, especially remote focus moving between categories, channels and the programme guide. A repo link already gives visitors the source.
- Add one real device capture of Tom’s Trains showing a departure and a tracked service. A short caption can explain why the board sorts by arrival time.
- Expand NucleusOne into a full case study with an approved screenshot from each product area. Explain how the two-developer team divided the work, which decisions you owned, and what a customer can now do in one place. Add a verified outcome if you can share one.

## Design directions

- **Current design** uses an editorial layout, an orange interface illustration and a dark project index. The CV keeps the same typography with a separate print layout.
- **Case study first** would lead with one approved screenshot and give the project its own page about the problem, implementation and outcome.
- **CV first** would put the career timeline directly after the introduction for visitors who primarily want to assess experience.

## GitHub Pages

1. Push this repository to GitHub. In **Settings → Pages**, choose **Deploy from a branch**, then `main` and `/ (root)`.
2. Verify `tomgc.com` in your GitHub account's Pages settings using the TXT record GitHub provides.
3. Set `tomgc.com` as the repository's custom domain. GitHub writes a `CNAME` file when Pages publishes from a branch. Pull that commit before editing the branch locally.
4. Point the domain's web records at GitHub Pages using the [official custom domain instructions](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site). Leave mail and mail-verification records in place. Use DNS-only records in Cloudflare for the Pages hostname.
5. Enable **Enforce HTTPS** once GitHub has provisioned the certificate.
