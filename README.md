# Owen Global Multibiz Services

Public website for **Owen Global Multibiz Services**, a business name registered with the Corporate Affairs Commission (CAC) of Nigeria.

Live site: [https://owenglobal.store](https://owenglobal.store)

The site describes the company’s trade in wholesale, retail, supermarket operations, general goods supply, and agriculture. It includes the contact details and legal pages payment partners such as Paystack typically expect when reviewing a merchant for international payments.

## Pages

- Home
- About
- Services and product categories
- Contact (email and enquiry form)
- Privacy Policy
- Terms of Service
- Refund and Return Policy

## Connect owenglobal.store (Namecheap + GitHub Pages)

After this code is on the `main` branch, do both of the following. GitHub Pages hosting is free. Do not buy SSL or hosting from Namecheap.

### 1. GitHub — attach the domain

1. Open the repository **Settings → Pages**.
2. Under **Build and deployment**, set source to **GitHub Actions**.
3. Under **Custom domain**, enter `owenglobal.store` and save.
4. Wait until DNS check succeeds, then tick **Enforce HTTPS**. This can take from a few minutes up to 24 hours.

### 2. Namecheap — DNS records

1. Sign in to [Namecheap](https://www.namecheap.com/).
2. Go to **Domain List → Manage** next to `owenglobal.store`.
3. Open the **Advanced DNS** tab.
4. Delete any existing **A**, **CNAME**, or **URL Redirect** records for `@` or `www` (parking or Namecheap default pages will block the site).
5. Add these records and save:

| Type | Host | Value | TTL |
| --- | --- | --- | --- |
| A Record | `@` | `185.199.108.153` | Automatic |
| A Record | `@` | `185.199.109.153` | Automatic |
| A Record | `@` | `185.199.110.153` | Automatic |
| A Record | `@` | `185.199.111.153` | Automatic |
| CNAME Record | `www` | `ojoakiliwo.github.io.` | Automatic |

Use `ojoakiliwo.github.io.` for the www CNAME (your GitHub username, not the repository name). Include the trailing dot if Namecheap shows it.

When HTTPS is on, give Paystack this URL:

`https://owenglobal.store`

The first time someone uses the contact form, Formsubmit will email `owenglobalmultibiz@gmail.com`. Open that message and confirm so enquiries can arrive.

## Details to add when you have them

Edit `contact.html` to include:

- CAC registration / business-name number
- Registered office address (Paystack usually wants this on the site)
- Business telephone number
- Social media links, if any

## Local preview

Open `index.html` in a browser, or from this folder run:

```bash
python3 -m http.server 8080
```

Then visit `http://localhost:8080`.
