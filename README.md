# tommyiaq.me
My personal website

✅ Step 1: Choose and Register a Cheap Domain
📝 What You Need to Do
Pick and buy a domain name from a budget-friendly domain registrar. Here are some recommended options for the lowest prices:

Registrar	Typical Cost (per year)	Notes
Namecheap	~$1–$9 (first year)	Offers $0.99 domains for some TLDs
Porkbun	~$1–$3 (first year)	Often has cheap deals, includes WHOIS privacy
Freenom	Free	Offers .tk, .ml, .ga, .cf, .gq TLDs for $0 (but may not be reliable long-term)

🔍 Instructions
Visit Namecheap, Porkbun, or Freenom.

Search for your desired domain name (e.g. hellotommaso.com, mytestsite.ml).

Pick a domain that’s free or under ~$2 for the first year.

Register the domain using a real email and enable free WHOIS privacy if offered (for privacy).

Please go ahead and register your domain now. Once done, let me know the domain name you bought, and I’ll guide you through the next step: setting up a free or very cheap hosting provider and deploying your Hello World site.






Hai detto:
Ok, I bought tommyiaq.me on purkbun. What next?


ChatGPT ha detto:
Perfect! You now own tommyiaq.me—great choice. 🎉

✅ Step 2: Deploy a Simple "Hello World" Website (Free Hosting)
🧠 Goal
We'll now put a basic website online with the message: Hello World, spending nothing on hosting.

We'll use GitHub Pages, which is 100% free, and integrates well with a basic HTML site.

🔧 Instructions: Set Up GitHub Pages
1. Create a GitHub Account (if you don’t have one)
Go to https://github.com/join

Choose a username (can be anything), email, password, etc.

Verify the email once signed up.

2. Create a New Repository
Go to https://github.com/new

Name it: tommyiaq.me (must exactly match your domain to simplify config later)

Make it public

Check ✅ "Add a README file"

Click Create Repository

3. Add Your Hello World Website
In your new repo, click "Add file" → "Create new file"

Name the file: index.html

Paste this simple HTML code:

html
Copia
Modifica
<!DOCTYPE html>
<html>
  <head>
    <title>Hello World</title>
  </head>
  <body>
    <h1>Hello World from tommyiaq.me!</h1>
  </body>
</html>
Scroll down and click Commit new file

4. Enable GitHub Pages
Go to the Settings tab of your repo → Click "Pages" in the left menu

Under "Build and deployment", set:

Source: Deploy from a branch

Branch: main / root directory

Click Save

GitHub will give you a live link like: https://yourusername.github.io/tommyiaq.me/

🟢 Let me know once this is done, and we’ll move to Step 3: Point your domain (tommyiaq.me) to GitHub Pages so the site appears on your custom domain.






Hai detto:
Got it https://github.com/tommyiaq/tommyiaq.me/settings/pages


ChatGPT ha detto:
Awesome — you’ve got your site set up on GitHub Pages. Nice job so far!

✅ Step 3: Connect Your Domain (tommyiaq.me) to GitHub Pages
Now let’s point your custom domain (bought on Porkbun) to your GitHub Pages site. This requires two parts:

🧾 Part A: Configure DNS Records in Porkbun
Log into Porkbun

Go to "Domain Management"

Find tommyiaq.me and click "Details"

Click “DNS Records”

Add these DNS records (delete any existing A, CNAME, or AAAA records that conflict):

➕ A Records (for apex domain: tommyiaq.me)
Type	Host	Value	TTL
A	@	185.199.108.153	Auto
A	@	185.199.109.153	Auto
A	@	185.199.110.153	Auto
A	@	185.199.111.153	Auto

➕ CNAME Record (for subdomain: www.tommyiaq.me)
Type	Host	Value	TTL
CNAME	www	tommyiaq.github.io. (include the dot)	Auto

✅ Note: You can skip the www subdomain if you don’t plan to use it.

🧾 Part B: Add CNAME File in GitHub
Go back to your GitHub repo

Click "Add file" → "Create new file"

Name the file exactly: CNAME (no extension, all caps)

In the content field, write:

tommyiaq.me

🕓 Wait & Test
DNS updates can take up to 5–30 minutes (usually faster).

Visit https://tommyiaq.me in your browser — you should see your Hello World page soon!

Let me know once you've done these steps, or if you want help verifying DNS is correct. After this, I can help you:

Add HTTPS

Deploy updates automatically

Add a custom design

…but let’s finish the DNS part first.






Hai detto:
Looks like it is already working with https


ChatGPT ha detto:
Fantastic — that means you nailed the setup! 🎉

You now have:

✅ A working custom domain (https://tommyiaq.me)
✅ A GitHub Pages–hosted site
✅ HTTPS enabled automatically by GitHub Pages (via Let's Encrypt)
✅ A live “Hello World” HTML page online
✅ All of this at a total cost of only your domain (~$3–$5/year)
