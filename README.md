# Highlightext

**Highlight what matters. Faster.**

Highlightext brings relevant words and phrases into focus so you can spot important
information while reading, researching, and analyzing. A familiar idea—a
highlighter—reimagined for digital work.

## Explore the project

- [Visual website](index.html): an animated, responsive introduction with an interactive keyword-highlighting demo.
- [Suggest a word](add-word.html): prepare an email request for a word, phrase, handle, or matching rule. Also request a custom keyword list for insurance, campaign management, legal, financial, or other specialized needs, with requirements and existing keywords. Requests go to hi@highlightext.com for review.
- [HTML for AI agents](agents.html): a plain semantic HTML summary with no JavaScript, CSS, images, or external dependencies.
- [Highlighter repository](https://github.com/highlightext-Org/highlighter): the core project’s home.

These links open source files in GitHub’s repository viewer. Download the HTML
files to open them in a browser, or serve them locally using the instructions below.

## What it is for

Make the language relevant to your task easier to notice:

| Work | Example reading focus |
| --- | --- |
| Research and financial analysis | Revenue, disclosures, growth, risk factors |
| Contracts and compliance | Clauses, exclusions, renewal dates, requirements |
| Marketing and communications | Brand names, competitor mentions, campaign approvals |
| Recruiting and project operations | Role requirements, deliverables, dependencies, deadlines |
| Academic research | Technical terms, citations, relevant findings |

These are proposed use cases. Highlights help direct attention; interpreting the
surrounding text and evaluating the evidence remains part of the reader’s work.

## Try the demo

Open `index.html` directly in a browser. No installation or build step is needed.

1. Choose **Research**, **Contracts**, or **Campaigns** to load an illustrative passage.
2. Enter your own comma-separated words or phrases.
3. Select **Apply highlights** to find literal, case-insensitive matches.
4. Use **Hide highlights** to compare the passage with and without highlighting.

The demo runs locally in the page. It makes no network requests, uses no analytics,
and does not upload your terms or load the project’s profile, wallet, or contact datasets.

To preview over HTTP, run this command from the directory containing this README:

```sh
python3 -m http.server 8765
```

Then visit [the visual page](http://localhost:8765/index.html) or
[the agent page](http://localhost:8765/agents.html).

## Design and accessibility

The visual page follows the supplied black-and-electric-yellow brand artwork.
Images, styles, and scripts are embedded in one standalone HTML file. It includes:

- Responsive layouts for small and large screens.
- Highlight animations and reduced-motion preferences.
- Semantic sections, keyboard controls, visible focus indicators, and a skip link.
- Live announcements of the match count.
- Print styles and readable project information when JavaScript is disabled.

The separate agent page exposes the project summary directly in HTML source,
without requiring script execution or visual interpretation.

## Project status

This repository presents the brand concept and a working keyword demonstration.
A released browser extension, installation package, and AI highlighting service
are not included here. The artwork’s local-processing and optional AI-assistance
messaging describes the product direction; the demo implements local keyword matching.

## Files and publishing

| File | Purpose |
| --- | --- |
| `index.html` | Standalone visual website and interactive demo |
| `add-word.html` | Word suggestion form that prepares an email draft for review |
| `payment-complete.html` | Static return page after Coinbase checkout; does not verify payment or activate access |
| `agents.html` | Script-free, style-free project summary for agents and readers |
| `README.md` | Project introduction and local preview instructions |

Serve the directory containing both HTML files as a static website. Keep them
beside each other so the links between versions work. No framework, package
manager, external font, or build pipeline is required.

GitHub Pages requires a separately configured deployment; committing HTML files
alone does not publish a website. No deployment is configured by these files.

## Source material and verification

The content draws on the project descriptions, supplied brand artwork (read
visually and with OCR), and target-market research. Use cases are presented
without treating occupational counts as customer adoption or addressable-market claims.

JavaScript syntax, demo interactions, local links, fragment targets, unique IDs,
and local HTTP responses were checked. The plain HTML page was checked for the
absence of scripts, styles, and images. Visual browser and device-size verification
remains outstanding because a browser was unavailable during authoring.

## Search and sharing

The production domain is `https://highlightext.com` (configured in `CNAME`).
All three public HTML pages have unique titles and descriptions, canonical URLs,
Open Graph and Twitter card metadata, and favicon links. The homepage includes
Organization, WebSite, and WebPage JSON-LD; the request page includes WebPage
JSON-LD. The agent page remains script-free.

`robots.txt` permits crawling and points to `sitemap.xml`, which lists canonical
public pages. When adding or removing pages, update the sitemap and page metadata.
Social preview and icon assets live in `assets/`; `favicon.ico` is at the site root.
Do not add fake ratings, unsupported product claims, or verification tokens.

After deployment, verify the domain in Google Search Console and Bing Webmaster
Tools using the account owner's verification method, then submit
`https://highlightext.com/sitemap.xml`. Check indexing reports and validate the
homepage with Google's Rich Results Test. These account actions are separate
from the repository changes. Keep HTTPS enforced in GitHub Pages settings.

## Subscription plans

For Coinbase checkout, set the post-payment redirect URL to
`https://highlightext.com/payment-complete.html` after deploying this page.
The return page is excluded from search indexing and intentionally omitted from
the sitemap. It is a static acknowledgement; transactions must be verified
separately before access is arranged.

The static homepage lists Advanced ($9 USD/month), Pro ($19 USD/month), and
Publisher (enquiry only). Advanced and Pro link directly to hosted Stripe
subscription checkout. Advanced and Pro also offer crypto payment through hosted Coinbase
payment links alongside Stripe. Transactions are verified and access arranged after payment;
this page does not automatically provision access. Publisher enquiries go to
hi@highlightext.com. No Stripe API credentials are included in the website.

## One-time targeted social handle research

The homepage includes a keyword and project-brief form for targeted social handle
research. It prepares an email draft for manual review; the visitor must send it.
Scope, one-time price, and delivery are agreed before payment. The Stripe product
is configured separately in `billing/stripe-research-product.json` in the parent
workspace. A price and hosted checkout link remain pending the owner's price.

## Legal pages

`terms.html` and `privacy.html` describe website use, subscriptions, custom work,
public-profile research, and data handling. They are linked from the homepage,
pricing section, request page, and sitemap. Update these notices before changing
data practices or commercial terms. Checkout or a written order must expressly
incorporate the Terms; a footer link alone is not a record of customer consent.

The notices use the Highlightext brand and existing support email. Confirm the
operating legal entity, business address, jurisdiction, actual provider/retention
practices, and applicable privacy obligations with counsel. In particular, selling
public-profile research can trigger privacy, opt-out, and data-broker obligations;
public availability alone does not remove those obligations. Configure hosted
checkout disclosures and affirmative agreement to match these pages.

## Community tier — free open-source tools

The Community tier is **free ($0)**: use the open-source tools without a
subscription or purchase. Company-owned software and associated technical
documentation are available under the [MIT License](LICENSE), including its
**AS IS / no-warranty / no-liability** provisions. Community support is best
effort; maintenance and updates are not guaranteed.

Read [license scope and software disclaimer](DISCLAIMER.md) before use. The
software license does not grant rights in branding, third-party material,
personal information, or generated datasets. Test suitability, verify results,
and keep backups. Liability exclusions apply only to the extent permitted by law.
Paid plans and custom services are separate from Community software rights.

## Research publications

The homepage links to [the research index](research/index.html), which links to
[HT-RP-001: What matters most to Burbank residents?](research/burbank-resident-priorities.html).
The article is an exploratory brief with sources, methods, corrections, and visible
questions and answers. It does not claim external peer review or representative sampling.

Agent discovery: [the .skills agent page](agents.html#research), [llms.txt](llms.txt),
and [the publication catalog](research/catalog.json). All article content is
server-readable static HTML; JavaScript is not needed to retrieve answers.
Read [research maintenance guidance](research/README.md) before adding papers.
