# Paste-to-HTML Email Converter Service

Use this to paste plain text and instantly generate polished HTML email with CTA button.

## File

- Open [email-converter-service.html](email-converter-service.html) in your browser.

## How It Works

1. Paste your plain text email in the big input box.
2. Keep first line as `Subject: ...` to auto-extract subject.
3. Set brand details, color, logo URL, website, and CTA button URL.
4. Click `Generate HTML`.
5. Copy the generated HTML and paste into your email sender.

## Input Format Example

```text
Subject: Quick thought for your brand

Hi Name,

I loved what you are building and had one quick idea.

We help brands improve conversion with better web funnels.

https://example.com/prototype

Would you be open to a short chat next week?

Best,
Ahsan Malik
```

## Notes

- URLs inside paragraphs are auto-converted to links.
- Greeting lines like `Hi Name,` are styled as a greeting.
- Subject is separated so you can paste it directly into your mail subject field.
- This is local and static. No server or API required.

## Optional Next Upgrade

If you want, I can add a true API service next:

- Endpoint `/render-email`
- Accepts plain text + brand settings JSON
- Returns `{ subject, html }`
- Ready to plug into CRM or automation tools

## GitHub Pages Deployment

This is ready for GitHub Pages, but it still needs a Git repository and a remote GitHub repo to publish.

Fastest path:

1. Create or choose a GitHub repo.
2. Put this file as `index.html` in the repo root or in `/docs`.
3. Push the branch to GitHub.
4. In GitHub repo settings, enable Pages from the branch root or `/docs` folder.

If you want me to do the actual deployment from here, I need the GitHub repo owner/name or the repo URL.
