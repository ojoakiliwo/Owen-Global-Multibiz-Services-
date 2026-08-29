# Owen Global Multibiz Services

Public website for **Owen Global Multibiz Services**, a business name registered with the Corporate Affairs Commission (CAC) of Nigeria.

The site describes the company’s trade in wholesale, retail, supermarket operations, general goods supply, and agriculture. It includes the contact details and legal pages payment partners such as Paystack typically expect when reviewing a merchant for international payments.

## Pages

- Home
- About
- Services and product categories
- Contact (email and enquiry form)
- Privacy Policy
- Terms of Service
- Refund and Return Policy

## Publish the site (required for Paystack)

Paystack needs a **live public URL**, not only these files in GitHub.

### Option 1 — GitHub Pages (free)

1. Merge this project to the `main` branch.
2. In the GitHub repository open **Settings → Pages**.
3. Under **Build and deployment**, choose **GitHub Actions** (the workflow in `.github/workflows/pages.yml` publishes the site).
4. After the workflow succeeds, the site is available at:

   `https://ojoakiliwo.github.io/Owen-Global-Multibiz-Services-/`

5. Paste that URL into the Website field on your Paystack compliance / international payments request.

The first time someone uses the contact form, Formsubmit will send a confirmation email to `owenglobalmultibiz@gmail.com`. Open that email and confirm so messages can be delivered.

### Option 2 — Custom domain (recommended later)

A domain such as `owenglobalmultibiz.com` looks more like a trading business than a `github.io` address. After you buy a domain, point it at GitHub Pages and add a `CNAME` file in this repository.

## Details to add when you have them

Edit `contact.html` (and the same lines on other pages if needed) to include:

- CAC registration / business-name number
- Registered office address (Paystack usually wants this on the site)
- Business telephone number
- Social media links, if any

The enquiry form currently emails **owenglobalmultibiz@gmail.com**.

## Local preview

Open `index.html` in a browser, or from this folder run:

```bash
python3 -m http.server 8080
```

Then visit `http://localhost:8080`.
