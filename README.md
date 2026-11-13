# artocons-mail-redirect

Redirects https://mail.artocons.com to Outlook on the web (https://outlook.office.com/mail/).

Microsoft 365 cannot serve a TLS certificate for a custom domain, so `mail.artocons.com`
points here (GitHub Pages issues the certificate) and this page forwards to Outlook.
`404.html` repeats the redirect so old links such as `/owa` also land in Outlook.

If this repository is ever removed, delete the `mail` CNAME record in the artocons.com DNS
at the same time.
