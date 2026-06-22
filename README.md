# Briefly landing page

The brief form sends each submission to your inbox using
[Web3Forms](https://web3forms.com), a simple form-to-email service. No backend,
no server, no deploy configuration needed.

## How the form works
- The form posts to `https://api.web3forms.com/submit` with your **public access
  key** (already wired into `index.html`).
- Web3Forms emails the brief to the address registered to that key.
- Your real email address is **not** in the page, only the public access key is,
  which is safe to expose.
- A hidden honeypot field (`company`) silently drops spam bots.

## To change where briefs are delivered
Update the email on your Web3Forms account, or generate a new access key at
https://web3forms.com and replace `WEB3FORMS_KEY` near the bottom of
`index.html`.

## Notes
- The form works from any hosted URL **and** from localhost, you can test it
  right away.
- If submissions stop arriving, check your spam folder and confirm the access
  key is still active on web3forms.com.
