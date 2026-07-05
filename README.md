# Dramameme GitHub Pages Site

This repository hosts the public Dramameme website for TikTok Developer review.

Expected live URLs after GitHub Pages is enabled:

- Web/Desktop URL: `https://charlieevert.github.io/dramameme/`
- Terms of Service URL: `https://charlieevert.github.io/dramameme/terms.html`
- Privacy Policy URL: `https://charlieevert.github.io/dramameme/privacy.html`
- OAuth Redirect URI: `https://charlieevert.github.io/dramameme/oauth-callback.html`

## GitHub Pages settings

1. Go to **Settings → Pages**.
2. Set source to **Deploy from a branch**.
3. Choose branch `main` and folder `/root`.
4. Save and wait for GitHub Pages to publish.

The `.nojekyll` file is included so GitHub Pages serves the static files directly.

## TikTok verification file

When TikTok gives you a URL verification/signature file, upload that exact file to this repo root next to `index.html`.

For example, if TikTok gives you `tiktok-developers-site-verification-abc123.txt`, upload it so it is reachable at:

`https://charlieevert.github.io/dramameme/tiktok-developers-site-verification-abc123.txt`

Then return to TikTok Developer Portal and click verify.

## TikTok app form copy

App description, max 120 characters:

`Dramameme helps creators generate AI meme drama videos and upload approved drafts to TikTok.`

App review explanation:

`Dramameme is a web app that helps creators generate AI-assisted meme drama videos, review the final video and caption, and upload approved content to TikTok. Login Kit lets a creator connect their TikTok account through TikTok OAuth. user.info.basic is used only to confirm the connected account. Content Posting API is used after the creator approves a generated video. Dramameme uses video.upload to upload the approved video to TikTok as a draft so the creator can finish editing and posting in TikTok. Share Kit is used to let a creator share or open approved Dramameme content through TikTok’s sharing flow from the website. Webhooks are used to receive TikTok integration events at Dramameme’s callback endpoint, such as posting/upload status updates when available. Dramameme does not post automatically without creator approval.`

## Important

Do not commit TikTok client secrets, refresh tokens, access tokens, API keys, or user tokens to this repo. This is only the static public website and legal/policy surface.
