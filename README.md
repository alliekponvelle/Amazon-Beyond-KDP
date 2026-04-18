<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Module 33 - Amazon Beyond KDP | The Creator Plug Academy</title>
  <style>
    :root {
      --ink: #24192f;
      --muted: #6f6178;
      --panel: #ffffff;
      --gold: #d9a441;
      --gold-soft: #fff2c9;
      --rose: #f05d8a;
      --teal: #18a6a7;
      --violet: #4d2770;
      --violet-deep: #241332;
      --line: #eadfce;
      --shadow: 0 18px 40px rgba(48, 31, 61, 0.14);
    }
    * { box-sizing: border-box; }
    html { scroll-behavior: smooth; }
    body {
      margin: 0;
      font-family: Arial, Helvetica, sans-serif;
      color: var(--ink);
      background:
        radial-gradient(circle at 14% 8%, rgba(240, 93, 138, 0.15), transparent 28%),
        radial-gradient(circle at 88% 4%, rgba(24, 166, 167, 0.16), transparent 26%),
        linear-gradient(180deg, #fffaf1 0%, #f8f1e7 45%, #f4ebdd 100%);
      line-height: 1.6;
    }
    a { color: #2c6f91; font-weight: 800; }
    .page { width: min(1120px, calc(100% - 32px)); margin: 0 auto; padding: 28px 0 56px; }
    .hero { background: linear-gradient(135deg, rgba(36, 19, 50, 0.96), rgba(77, 39, 112, 0.92)); color: #fff; border-radius: 8px; padding: 34px; box-shadow: var(--shadow); position: relative; overflow: hidden; }
    .hero:after { content: ""; position: absolute; right: -78px; top: -82px; width: 260px; height: 260px; border: 2px solid rgba(217, 164, 65, 0.36); transform: rotate(20deg); }
    .eyebrow { display: inline-flex; background: rgba(217, 164, 65, 0.18); border: 1px solid rgba(217, 164, 65, 0.45); color: #ffe3a0; border-radius: 8px; padding: 7px 11px; font-size: 13px; font-weight: 800; letter-spacing: 0.08em; text-transform: uppercase; }
    h1, h2, h3 { line-height: 1.15; margin: 0; }
    h1 { max-width: 920px; margin-top: 18px; font-size: clamp(34px, 6vw, 70px); }
    .subtitle { max-width: 900px; margin: 18px 0 0; color: #f6e9d6; font-size: 18px; }
    .quick-links { display: flex; flex-wrap: wrap; gap: 10px; margin-top: 24px; position: relative; z-index: 1; }
    .quick-links a, .copy-button { appearance: none; border: 0; border-radius: 8px; background: var(--gold); color: #241332; cursor: pointer; display: inline-flex; align-items: center; justify-content: center; font-family: inherit; font-size: 14px; font-weight: 900; line-height: 1; min-height: 42px; padding: 12px 14px; text-decoration: none; }
    .quick-links a:hover, .copy-button:hover { background: #f1c761; }
    .hero-grid, .three-col { display: grid; grid-template-columns: repeat(3, 1fr); gap: 14px; margin-top: 26px; }
    .hero-card { background: rgba(255, 255, 255, 0.1); border: 1px solid rgba(255, 255, 255, 0.18); border-radius: 8px; padding: 18px; min-height: 126px; }
    .hero-card strong { color: #ffe1a1; display: block; font-size: 15px; text-transform: uppercase; letter-spacing: 0.08em; margin-bottom: 8px; }
    .section { margin-top: 24px; background: rgba(255, 255, 255, 0.88); border: 1px solid var(--line); border-radius: 8px; padding: 28px; box-shadow: 0 10px 24px rgba(48, 31, 61, 0.08); }
    .section h2 { color: var(--violet-deep); font-size: clamp(25px, 3vw, 38px); margin-bottom: 12px; }
    .section-intro { max-width: 900px; color: var(--muted); margin: 0 0 20px; }
    .two-col { display: grid; grid-template-columns: repeat(2, 1fr); gap: 16px; }
    .card { background: var(--panel); border: 1px solid var(--line); border-radius: 8px; padding: 20px; }
    .card h3 { color: var(--violet); font-size: 20px; margin-bottom: 8px; }
    .tag { display: inline-block; border-radius: 8px; padding: 5px 9px; margin-bottom: 12px; background: var(--gold-soft); color: #765210; font-weight: 800; font-size: 12px; text-transform: uppercase; letter-spacing: 0.06em; }
    ul, ol { margin: 10px 0 0 20px; padding: 0; }
    li { margin: 8px 0; }
    .link-grid { display: grid; grid-template-columns: repeat(2, 1fr); gap: 12px; margin-bottom: 24px; }
    .lesson-link { background: #fff; border: 1px solid var(--line); border-radius: 8px; color: var(--violet-deep); display: block; font-weight: 800; padding: 14px; text-decoration: none; }
    .lesson-link:hover { border-color: var(--gold); box-shadow: 0 8px 20px rgba(48, 31, 61, 0.1); transform: translateY(-1px); }
    .lesson { display: grid; grid-template-columns: 84px 1fr; gap: 16px; border-top: 1px solid var(--line); padding: 20px 0; }
    .lesson:first-of-type { border-top: 0; padding-top: 0; }
    .lesson-number { width: 64px; height: 64px; border-radius: 8px; background: linear-gradient(135deg, var(--violet), var(--rose)); color: #fff; display: grid; place-items: center; font-size: 24px; font-weight: 900; box-shadow: 0 12px 22px rgba(77, 39, 112, 0.22); }
    .lesson-number a { color: #fff; display: grid; height: 100%; place-items: center; text-decoration: none; width: 100%; }
    .callout { border-left: 5px solid var(--gold); background: #fff7dc; padding: 16px 18px; border-radius: 8px; margin-top: 16px; }
    .warning { border-left-color: var(--rose); background: #fff0f5; }
    table { width: 100%; border-collapse: collapse; overflow: hidden; border-radius: 8px; background: #fff; border: 1px solid var(--line); margin-top: 14px; }
    th, td { text-align: left; vertical-align: top; border-bottom: 1px solid var(--line); padding: 14px; }
    th { background: var(--violet-deep); color: #fff; font-size: 13px; text-transform: uppercase; letter-spacing: 0.06em; }
    tr:last-child td { border-bottom: 0; }
    .script-box { background: #241332; color: #fdf5e8; border-radius: 8px; padding: 18px; font-family: "Courier New", Courier, monospace; font-size: 14px; line-height: 1.55; white-space: pre-wrap; }
    .copy-row { align-items: center; display: flex; flex-wrap: wrap; gap: 10px; justify-content: space-between; margin-bottom: 10px; }
    .checklist { list-style: none; margin-left: 0; }
    .checklist li { padding-left: 34px; position: relative; }
    .checklist li:before { content: ""; position: absolute; left: 0; top: 5px; width: 19px; height: 19px; border-radius: 5px; border: 2px solid var(--teal); background: #efffff; }
    .footer { margin-top: 24px; text-align: center; color: var(--muted); font-size: 14px; }
    @media (max-width: 820px) {
      .hero { padding: 24px; }
      .hero-grid, .two-col, .three-col, .link-grid { grid-template-columns: 1fr; }
      .lesson { grid-template-columns: 1fr; }
      table, thead, tbody, th, td, tr { display: block; }
      th { display: none; }
    }
  </style>
</head>
<body>
  <main class="page">
    <section class="hero">
      <span class="eyebrow">Module 33</span>
      <h1>Amazon Beyond KDP</h1>
      <p class="subtitle">Build multiple income streams across Amazon's seller ecosystem: FBA, Merch on Demand, Handmade, Associates, Influencer storefronts, Brand Registry, ads, and content-to-commerce systems.</p>
      <nav class="quick-links" aria-label="Quick links">
        <a href="#lessons">Lessons</a>
        <a href="#launch-plan">30-Day Plan</a>
        <a href="#copy-tools">Copy Tools</a>
        <a href="#resources">Resource Links</a>
      </nav>
      <div class="hero-grid">
        <div class="hero-card"><strong>Big Idea</strong>Amazon is not one income stream. It is a marketplace, fulfillment network, ad platform, affiliate engine, and brand-building ecosystem.</div>
        <div class="hero-card"><strong>Best For</strong>Creators, product founders, print-on-demand sellers, handmade makers, affiliates, educators, and ecommerce entrepreneurs.</div>
        <div class="hero-card"><strong>2026 Update</strong>Kindle Vella is retired, so this module treats it as a lesson learned and points serialized fiction creators to KDP plus off-Amazon options.</div>
      </div>
    </section>

    <section class="section" id="overview">
      <h2>Module Overview</h2>
      <p class="section-intro">Most creators stop at KDP. Amazon gives you more lanes: fulfillment, physical products, print-on-demand, handmade goods, affiliate content, influencer storefronts, ads, and brand tools. The goal is to choose the right lane for your budget, skills, and risk tolerance, then stack channels over time.</p>
      <div class="callout warning">Amazon fees, eligibility, and programs change often. Use the official resource links before pricing, sourcing, applying, or launching.</div>
    </section>

    <section class="section" id="lessons">
      <h2>Lessons</h2>
      <div class="link-grid">
        <a class="lesson-link" href="#lesson-1">1. Amazon ecosystem</a>
        <a class="lesson-link" href="#lesson-2">2. FBA deep dive</a>
        <a class="lesson-link" href="#lesson-3">3. Product research and sourcing</a>
        <a class="lesson-link" href="#lesson-4">4. Listing optimization</a>
        <a class="lesson-link" href="#lesson-5">5. Merch on Demand</a>
        <a class="lesson-link" href="#lesson-6">6. Amazon Handmade</a>
        <a class="lesson-link" href="#lesson-7">7. Amazon Associates</a>
        <a class="lesson-link" href="#lesson-8">8. Influencer Program</a>
        <a class="lesson-link" href="#lesson-9">9. Kindle Vella update</a>
        <a class="lesson-link" href="#lesson-10">10. Private label brand</a>
        <a class="lesson-link" href="#lesson-11">11. Amazon advertising</a>
        <a class="lesson-link" href="#lesson-12">12. Passive income stack</a>
        <a class="lesson-link" href="#lesson-13">13. Account health and scaling</a>
        <a class="lesson-link" href="#launch-plan">14. 30-Day Amazon launch plan</a>
      </div>

      <article class="lesson" id="lesson-1">
        <div class="lesson-number"><a href="#lessons">1</a></div>
        <div>
          <h3>Amazon's Full Ecosystem - Beyond the Bookshelf</h3>
          <p>Amazon is a group of business models sitting under one shopping engine. Some are zero-inventory channels. Some require sourcing, operations, and customer support. The smart move is not to chase every program at once; it is to choose the first lane that matches your resources, then stack channels once one is working.</p>
          <table>
            <thead><tr><th>Channel</th><th>What It Is</th><th>Best For</th></tr></thead>
            <tbody>
              <tr><td>KDP</td><td>Self-publish ebooks, paperbacks, hardcovers, journals, planners, and educational books.</td><td>Writers, teachers, niche educators, low-content creators.</td></tr>
              <tr><td>FBA</td><td>Send inventory to Amazon, then Amazon stores, picks, packs, ships, and handles returns/customer service.</td><td>Physical product brands and private-label sellers.</td></tr>
              <tr><td>Merch on Demand</td><td>Upload designs for print-on-demand apparel and accessories with no inventory.</td><td>Designers, meme creators, niche communities, quote brands.</td></tr>
              <tr><td>Amazon Handmade</td><td>Application-based marketplace for authentic handmade, hand-designed, altered, repurposed, or upcycled goods.</td><td>Artists, crafters, makers, small artisan teams.</td></tr>
              <tr><td>Amazon Associates</td><td>Affiliate links that earn commission on qualifying Amazon purchases.</td><td>Bloggers, YouTubers, newsletter writers, reviewers.</td></tr>
              <tr><td>Amazon Influencer</td><td>Creator storefronts, product lists, and shoppable recommendations tied to social presence.</td><td>Social creators with engaged audiences.</td></tr>
              <tr><td>Brand Registry + Ads</td><td>Brand protection, A+ Content, Brand Stores, analytics, Vine, and sponsored ad tools.</td><td>Private-label sellers building real brands.</td></tr>
            </tbody>
          </table>
          <div class="callout">Creator stack idea: KDP + Merch on Demand + Associates can start with low capital. FBA adds the highest physical-product upside once you have product research, cash flow, and operational discipline.</div>
        </div>
      </article>

      <article class="lesson" id="lesson-2">
        <div class="lesson-number"><a href="#lessons">2</a></div>
        <div>
          <h3>Amazon FBA - Fulfillment by Amazon Deep Dive</h3>
          <p>FBA is the major physical product lane. You source or manufacture a product, ship it into Amazon's fulfillment network, and Amazon handles storage, shipping, customer service, and returns. Your job becomes research, margins, inventory, listing quality, reviews, and ads.</p>
          <ol>
            <li>Research a product niche using paid tools, Amazon search, Best Sellers, and customer review gaps.</li>
            <li>Source samples and confirm landed cost, quality, packaging, compliance, and minimum order quantity.</li>
            <li>Create or update a Seller Central account and choose the selling plan that fits your volume.</li>
            <li>Build an optimized listing with title, bullets, images, backend terms, price, and A+ Content if eligible.</li>
            <li>Ship inventory to Amazon and use official calculators before committing to a bulk order.</li>
            <li>Launch with a review strategy, PPC campaign, inventory plan, and weekly profit review.</li>
          </ol>
          <table>
            <thead><tr><th>Model</th><th>How It Works</th><th>Best Fit</th></tr></thead>
            <tbody>
              <tr><td>Private Label</td><td>Source a product, improve it, package it under your own brand.</td><td>Creators who want brand equity and long-term resale value.</td></tr>
              <tr><td>Wholesale</td><td>Buy approved brand-name inventory at wholesale and resell.</td><td>Operators who can manage buy box competition and supplier relationships.</td></tr>
              <tr><td>Retail Arbitrage</td><td>Buy discounted products in stores and resell for profit.</td><td>Low-budget testing, but time-intensive.</td></tr>
              <tr><td>Online Arbitrage</td><td>Source discounted products online and resell on Amazon.</td><td>Sellers using software and repeatable sourcing systems.</td></tr>
              <tr><td>Bundles</td><td>Combine complementary products into a new offer.</td><td>Sellers looking for differentiation without manufacturing from scratch.</td></tr>
            </tbody>
          </table>
          <div class="callout warning">Never source from vibes. Run referral fees, FBA fees, storage, ad spend, returns, shipping, duties, and packaging through Amazon's current fee tools before buying inventory.</div>
        </div>
      </article>

      <article class="lesson" id="lesson-3">
        <div class="lesson-number"><a href="#lessons">3</a></div>
        <div>
          <h3>Product Research Tools and Sourcing</h3>
          <p>Amazon rewards demand and punishes weak math. A product can look exciting and still lose money if the category is too competitive, the product is too heavy, the reviews are impossible to beat, or the ad costs eat the margin.</p>
          <div class="two-col">
            <div class="card">
              <span class="tag">Research Tools</span>
              <ul>
                <li>Helium 10, Jungle Scout, AMZScout, Keepa, Sellerboard, and keyword tools.</li>
                <li>Amazon Best Sellers, Movers & Shakers, reviews, and autocomplete.</li>
                <li>Google Trends, Reddit communities, TikTok search, Pinterest search, and competitor websites.</li>
              </ul>
            </div>
            <div class="card">
              <span class="tag">Sourcing Options</span>
              <ul>
                <li>Alibaba, Global Sources, Made-in-China, DHgate, and sourcing agents.</li>
                <li>US suppliers through ThomasNet, Maker's Row, Faire, and category-specific wholesalers.</li>
                <li>Local manufacturers when speed, quality control, or premium positioning matters more than lowest unit cost.</li>
              </ul>
            </div>
          </div>
          <h4>CLOVER Product Checklist</h4>
          <ul>
            <li><strong>Cost:</strong> Can you source, package, ship, advertise, and still keep margin?</li>
            <li><strong>Lightweight:</strong> Smaller and lighter products usually reduce fulfillment drag.</li>
            <li><strong>Opportunity:</strong> Search demand exists, but the first page is not impossible to beat.</li>
            <li><strong>Value gap:</strong> Competitor reviews reveal fixable complaints.</li>
            <li><strong>Existing sales:</strong> Similar products already sell. Competitors are proof of demand.</li>
            <li><strong>Repeat purchase:</strong> Consumables, accessories, refills, and bundles can compound.</li>
          </ul>
          <div class="callout">Order samples, inspect before bulk shipping, document specifications, get product liability insurance when needed, and understand category compliance before you list.</div>
        </div>
      </article>

      <article class="lesson" id="lesson-4">
        <div class="lesson-number"><a href="#lessons">4</a></div>
        <div>
          <h3>Amazon Listing Optimization - Getting Found and Converting</h3>
          <p>Your listing is the sales page, the search target, and the trust signal. A better product can still lose if the title is vague, the images are weak, the bullets talk features instead of outcomes, or the price does not make sense against competitors.</p>
          <ol>
            <li><strong>Title:</strong> Brand + main keyword + differentiator + size/quantity + use case.</li>
            <li><strong>Bullets:</strong> Lead with benefits and proof. Write for a buyer skimming on mobile.</li>
            <li><strong>Images:</strong> Use a compliant main image, lifestyle shots, infographics, scale references, and packaging shots.</li>
            <li><strong>A+ Content:</strong> Use Brand Registry to add enhanced images, comparison modules, and brand story blocks.</li>
            <li><strong>Backend Search Terms:</strong> Add synonyms, alternate phrases, and relevant misspellings without keyword stuffing.</li>
            <li><strong>Price:</strong> Launch with a margin-aware price, not a panic discount that trains buyers to wait.</li>
            <li><strong>Reviews:</strong> Use compliant tools like Request a Review and Amazon Vine when eligible. Never buy, trade, or incentivize reviews.</li>
          </ol>
          <div class="callout warning">Amazon is strict about review manipulation, IP infringement, and misleading claims. A short-term trick can cost the whole account.</div>
        </div>
      </article>

      <article class="lesson" id="lesson-5">
        <div class="lesson-number"><a href="#lessons">5</a></div>
        <div>
          <h3>Amazon Merch on Demand - Print-on-Demand Apparel</h3>
          <p>Merch on Demand lets you upload artwork, choose products, set prices, and earn royalties when Amazon prints and ships the product. It is one of the cleanest zero-inventory channels for creators, but it requires volume, niche research, and strict copyright hygiene.</p>
          <div class="two-col">
            <div class="card">
              <span class="tag">How It Works</span>
              <ol>
                <li>Apply for a Merch on Demand account.</li>
                <li>Create compliant artwork files and product titles.</li>
                <li>Choose product types and set your price.</li>
                <li>Amazon handles production, shipping, and customer service.</li>
                <li>You earn a royalty based on price minus taxes and Amazon costs.</li>
              </ol>
            </div>
            <div class="card">
              <span class="tag">Niches That Travel</span>
              <ul>
                <li>Occupational humor: nurses, teachers, truckers, barbers.</li>
                <li>Hobbies: fishing, gaming, pickleball, gardening, fitness.</li>
                <li>Identity: dog dad, girl dad, auntie, grandma, college town pride.</li>
                <li>Faith, motivation, birthdays, holidays, and local culture.</li>
              </ul>
            </div>
          </div>
          <div class="callout warning">Before upload, check USPTO for trademarks and avoid copyrighted characters, logos, lyrics, celebrity names, sports team marks, and copied designs. Amazon can reject designs or terminate accounts for violations.</div>
        </div>
      </article>

      <article class="lesson" id="lesson-6">
        <div class="lesson-number"><a href="#lessons">6</a></div>
        <div>
          <h3>Amazon Handmade - The Artisan Marketplace</h3>
          <p>Amazon Handmade is built for makers who create, alter, customize, upcycle, or hand-design physical goods. It is not the lane for mass-produced products pretending to be handmade. The advantage is Amazon's shopper base and Prime-enabled fulfillment options. The challenge is standing out with story, photography, and trust.</p>
          <div class="two-col">
            <div class="card">
              <span class="tag">What Sells</span>
              <ul>
                <li>Jewelry, home decor, kitchen goods, stationery, party supplies, pet accessories, artwork, clothing, and beauty items.</li>
                <li>Personalized products: names, dates, colors, sizes, memorial pieces, wedding gifts, nursery decor.</li>
                <li>Giftable products with strong photos and clear delivery expectations.</li>
              </ul>
            </div>
            <div class="card">
              <span class="tag">Setup Tips</span>
              <ul>
                <li>Apply with a clear artisan profile and photos of your process.</li>
                <li>Write descriptions that explain materials, personalization, care, and production time.</li>
                <li>Batch bestsellers and consider FBA for repeatable SKUs that can ship fast.</li>
              </ul>
            </div>
          </div>
          <div class="callout">Handmade buyers care about the maker. Use your product story as part of the value, not as an afterthought.</div>
        </div>
      </article>

      <article class="lesson" id="lesson-7">
        <div class="lesson-number"><a href="#lessons">7</a></div>
        <div>
          <h3>Amazon Associates - The Affiliate Program</h3>
          <p>Amazon Associates lets you earn commission when people click your links and make qualifying purchases. This is the natural lane for creators who already make content: product roundups, reviews, setup lists, gift guides, tutorials, and "what I use" pages.</p>
          <ol>
            <li>Apply with an active website, app, YouTube channel, or social platform that meets Amazon's requirements.</li>
            <li>Generate affiliate links for products you genuinely recommend.</li>
            <li>Disclose clearly that you may earn from qualifying purchases.</li>
            <li>Place links in content that solves buyer intent: "best," "review," "setup," "comparison," "gift guide," and "tools I use."</li>
            <li>Review Amazon's current commission income statement before forecasting. Rates vary by category and change over time.</li>
          </ol>
          <div class="callout">The affiliate advantage is trust. A small audience that believes your recommendations can outperform a large audience that treats every link like an ad.</div>
        </div>
      </article>

      <article class="lesson" id="lesson-8">
        <div class="lesson-number"><a href="#lessons">8</a></div>
        <div>
          <h3>The Amazon Influencer Program</h3>
          <p>The Influencer Program is an extension of Associates for social creators. It gives you a custom storefront where you can organize recommended products into lists and share a clean Amazon URL with your audience.</p>
          <div class="two-col">
            <div class="card">
              <span class="tag">What You Build</span>
              <ul>
                <li>Storefront collections for your niche: studio setup, beauty shelf, kitchen tools, homeschool kit, creator gear.</li>
                <li>Product recommendation videos and short demos that help shoppers decide.</li>
                <li>Seasonal gift guides and launch lists tied to your content calendar.</li>
              </ul>
            </div>
            <div class="card">
              <span class="tag">Creator Flow</span>
              <ul>
                <li>Use social content to create demand.</li>
                <li>Send viewers to your storefront or product lists.</li>
                <li>Use Amazon videos, product demos, and external content to compound trust.</li>
              </ul>
            </div>
          </div>
          <div class="callout">Your storefront should feel curated, not dumped. Group products by outcome: "Podcast Starter Kit" converts better than "Random Amazon Favorites."</div>
        </div>
      </article>

      <article class="lesson" id="lesson-9">
        <div class="lesson-number"><a href="#lessons">9</a></div>
        <div>
          <h3>Kindle Vella Update - What Changed</h3>
          <p>Kindle Vella used to be Amazon's serialized fiction platform, but Amazon retired it in February 2025. Do not build a new business plan around Vella. Treat it as a case study in platform risk: even Amazon programs can change or close.</p>
          <div class="callout warning">Current path for serialized writers: publish completed arcs through KDP, build reader email lists, experiment with Kindle Unlimited if it fits your strategy, and consider off-Amazon serial platforms or memberships for ongoing episodes.</div>
          <h4>Alternative Paths for Story Creators</h4>
          <ul>
            <li><strong>KDP series:</strong> Turn episodes into short books, novellas, or season collections.</li>
            <li><strong>Reader membership:</strong> Use Patreon, Substack, Ream, or your own community for early chapters.</li>
            <li><strong>Discovery platforms:</strong> Use Wattpad, Royal Road, Radish-style platforms, BookTok, and Bookstagram to build audience.</li>
            <li><strong>Email-first model:</strong> Give away chapter one, nurture readers, then sell bundles, paperbacks, and audiobook editions.</li>
          </ul>
        </div>
      </article>

      <article class="lesson" id="lesson-10">
        <div class="lesson-number"><a href="#lessons">10</a></div>
        <div>
          <h3>Building an Amazon Brand - Private Label Done Right</h3>
          <p>The highest ceiling on Amazon is a real brand, not a random product. A brand has a defined customer, a visual identity, repeatable quality, a product roadmap, and defensible positioning. That is what turns a listing into an asset.</p>
          <ol>
            <li><strong>Validate the niche:</strong> Choose a space with multiple product opportunities, not a one-hit commodity.</li>
            <li><strong>Define the customer:</strong> Know the buyer's use case, budget, frustrations, and emotional reason for buying.</li>
            <li><strong>Develop brand identity:</strong> Name, logo, packaging, voice, images, and promise.</li>
            <li><strong>Protect the brand:</strong> Trademark your name when appropriate and apply for Brand Registry once eligible.</li>
            <li><strong>Build the Amazon Store:</strong> Organize product lines, use lifestyle imagery, and tell the brand story.</li>
            <li><strong>Diversify off Amazon:</strong> Build Shopify, email, social, and creator content because Amazon does not give you full customer ownership.</li>
          </ol>
          <div class="callout">Brand Registry unlocks tools like A+ Content, Amazon Stores, Brand Analytics, Sponsored Brands, and Vine. It is the serious-seller layer of Amazon.</div>
        </div>
      </article>

      <article class="lesson" id="lesson-11">
        <div class="lesson-number"><a href="#lessons">11</a></div>
        <div>
          <h3>Amazon Advertising - Getting Your Products Found</h3>
          <p>Amazon PPC is how new products buy visibility while organic rank develops. Ads are not a substitute for product-market fit, but they are a powerful data engine: you learn which keywords, competitor ASINs, and product angles convert.</p>
          <table>
            <thead><tr><th>Ad Type</th><th>What It Does</th><th>Best For</th></tr></thead>
            <tbody>
              <tr><td>Sponsored Products</td><td>Promotes individual listings in search and product placements.</td><td>Launches, keyword testing, sales velocity.</td></tr>
              <tr><td>Sponsored Brands</td><td>Shows brand creative, logo, headlines, and products.</td><td>Brand-registered sellers building awareness.</td></tr>
              <tr><td>Sponsored Display</td><td>Reaches shoppers on and off Amazon with product and audience targeting.</td><td>Retargeting and competitor-page visibility.</td></tr>
              <tr><td>Sponsored Brands Video</td><td>Video creative in shopping placements.</td><td>Products that need demonstration or visual proof.</td></tr>
            </tbody>
          </table>
          <h4>Beginner Campaign Structure</h4>
          <ol>
            <li>Auto campaign for keyword and ASIN discovery.</li>
            <li>Manual exact campaign for converting search terms.</li>
            <li>Manual phrase campaign for controlled expansion.</li>
            <li>Product targeting campaign for competitor listings.</li>
            <li>Weekly cleanup: pause waste, raise bids on profitable terms, add negatives.</li>
          </ol>
          <div class="callout warning">Watch contribution margin, not vanity sales. If your ACoS looks fine but returns, storage, coupons, and referral fees erase profit, the campaign is not healthy.</div>
        </div>
      </article>

      <article class="lesson" id="lesson-12">
        <div class="lesson-number"><a href="#lessons">12</a></div>
        <div>
          <h3>The Creator's Amazon Passive Income Stack</h3>
          <p>The Creator Plug approach is to build cash-flow layers. Start with the channel that fits your current capital and audience, then connect the channels so each one feeds the next.</p>
          <div class="three-col">
            <div class="card">
              <span class="tag">Tier 1 - Zero Inventory</span>
              <ul>
                <li>KDP books, journals, planners, guides.</li>
                <li>Merch on Demand designs.</li>
                <li>Associates and Influencer storefront content.</li>
              </ul>
            </div>
            <div class="card">
              <span class="tag">Tier 2 - Semi-Passive</span>
              <ul>
                <li>FBA private label with Amazon fulfillment.</li>
                <li>Handmade bestsellers moved into batch production and FBA where possible.</li>
                <li>Brand Registry, A+ Content, Stores, and PPC systems.</li>
              </ul>
            </div>
            <div class="card">
              <span class="tag">Tier 3 - Active Growth</span>
              <ul>
                <li>Retail and online arbitrage.</li>
                <li>Ongoing product demo content.</li>
                <li>Wholesale sourcing, inventory negotiations, and ad optimization.</li>
              </ul>
            </div>
          </div>
          <div class="callout">Example ecosystem: a YouTube gear review earns Associates commission, sends buyers to your Amazon storefront, promotes your KDP guide, and eventually validates an FBA private-label accessory.</div>
        </div>
      </article>

      <article class="lesson" id="lesson-13">
        <div class="lesson-number"><a href="#lessons">13</a></div>
        <div>
          <h3>Amazon Account Health, Policies, and Scaling</h3>
          <p>Your Amazon account is the asset. Protect it like one. Sales are exciting, but one unresolved policy issue, IP complaint, safety claim, or review violation can freeze the whole operation.</p>
          <div class="two-col">
            <div class="card">
              <span class="tag">Protect The Account</span>
              <ul>
                <li>Monitor Account Health and respond to warnings quickly.</li>
                <li>Keep two-factor authentication enabled.</li>
                <li>Respect IP, trademarks, restricted products, and category compliance.</li>
                <li>Do not buy, trade, incentivize, or manipulate reviews.</li>
                <li>Avoid multiple seller accounts unless Amazon approves the exception.</li>
              </ul>
            </div>
            <div class="card">
              <span class="tag">Scale With Systems</span>
              <ul>
                <li>Reinvest profit into inventory, content, creative testing, and compliance.</li>
                <li>Add 1-2 ASINs per quarter only after a proven product has clean data.</li>
                <li>Create SOPs for sourcing, listings, customer messages, ads, and inventory checks.</li>
                <li>Hire VAs or specialists for repeatable admin, PPC, design, and research tasks.</li>
              </ul>
            </div>
          </div>
          <div class="callout warning">Do not scale chaos. If you cannot explain your margins, inventory position, and account risks in one page, slow down and systemize before adding more products.</div>
        </div>
      </article>
    </section>

    <section class="section" id="launch-plan">
      <h2>Your 30-Day Amazon Launch Plan</h2>
      <div class="two-col">
        <div class="card">
          <h3>Week 1 - Choose Your Lane and Research</h3>
          <ul>
            <li>Day 1-2: Choose the first Amazon program based on skills, budget, and risk.</li>
            <li>Day 3-4: Research products, niches, keywords, demand, and competitor gaps.</li>
            <li>Day 5-6: Create the required account or application plan.</li>
            <li>Day 7: Source a sample, create five designs, or outline your first content asset.</li>
          </ul>
        </div>
        <div class="card">
          <h3>Week 2 - Setup and Create</h3>
          <ul>
            <li>Day 8-9: Set up business basics, payment info, tax info, and records.</li>
            <li>Day 10-11: Build the first listing, design, storefront list, or affiliate page.</li>
            <li>Day 12-13: Apply for Brand Registry if you are pursuing private label and eligible.</li>
            <li>Day 14: Submit the first shipment, upload designs, or publish affiliate content.</li>
          </ul>
        </div>
        <div class="card">
          <h3>Week 3 - Launch and Learn</h3>
          <ul>
            <li>Day 15-16: Launch PPC for FBA or promote the new zero-inventory asset.</li>
            <li>Day 17-18: Use compliant review and customer feedback systems.</li>
            <li>Day 19-20: Publish support content: YouTube, blog, email, TikTok, or Pinterest.</li>
            <li>Day 21: Review early data and document what changed.</li>
          </ul>
        </div>
        <div class="card">
          <h3>Week 4 - Optimize and Stack</h3>
          <ul>
            <li>Day 22-24: Refine listings, keywords, images, price, and content CTAs.</li>
            <li>Day 25-26: Add a second asset: another design, product idea, article, video, or bundle.</li>
            <li>Day 27-28: Build the external audience that supports your Amazon channel.</li>
            <li>Day 29-30: Review account health, P&L, and set a 90-day revenue goal.</li>
          </ul>
        </div>
      </div>
      <div class="callout">Amazon creator commitment: Merch sellers publish 30 designs in 30 days. Associates publish four buyer-intent content pieces per month. FBA sellers validate one product deeply before chasing five more.</div>
    </section>

    <section class="section" id="copy-tools">
      <h2>Copy Tools</h2>
      <p class="section-intro">Use these prompts and formulas to move faster without skipping the thinking that protects your margins.</p>
      <div class="card">
        <div class="copy-row">
          <h3>CLOVER Product Research Prompt</h3>
          <button class="copy-button" data-copy="clover">Copy</button>
        </div>
        <div class="script-box" id="clover">Evaluate this Amazon product idea using CLOVER:
Product:
Target customer:
Estimated selling price:
Estimated landed cost:
Main competitors:

C - Cost: Can I keep margin after referral fees, FBA fees, storage, ads, returns, shipping, duties, and packaging?
L - Lightweight: Is it small/light enough to avoid fee drag?
O - Opportunity: Is there demand without impossible competition?
V - Value gap: What review complaints can I improve?
E - Existing sales: Are similar products already selling?
R - Repeat purchase: Can this become repeat orders, bundles, refills, or accessories?</div>
      </div>
      <div class="card">
        <div class="copy-row">
          <h3>Listing Formula</h3>
          <button class="copy-button" data-copy="listing">Copy</button>
        </div>
        <div class="script-box" id="listing">Title: [Brand] + [Main Keyword] + [Differentiator] + [Size/Quantity] + [Use Case]
Bullet 1: Outcome/result the buyer wants
Bullet 2: What makes the product better
Bullet 3: Materials, quality, or compliance proof
Bullet 4: Use cases and who it is for
Bullet 5: Trust, guarantee, care, or bundle detail
Image set: main image, lifestyle, infographic, scale, problem/solution, packaging, comparison</div>
      </div>
      <div class="card">
        <div class="copy-row">
          <h3>Amazon Channel Selector</h3>
          <button class="copy-button" data-copy="selector">Copy</button>
        </div>
        <div class="script-box" id="selector">If I have design skills but low capital: start with Merch on Demand.
If I have writing/teaching skills: start with KDP and Associates.
If I have an audience: start with Associates or Influencer.
If I make physical goods by hand: apply for Amazon Handmade.
If I have $2K-$10K and can handle operations: research FBA private label.
If I want brand equity: combine FBA + Brand Registry + Shopify + email.</div>
      </div>
    </section>

    <section class="section" id="checklist">
      <h2>Quick Reference: Amazon Creator Checklist</h2>
      <div class="two-col">
        <div class="card">
          <h3>Channel Choice</h3>
          <ul class="checklist">
            <li>Primary Amazon channel chosen based on budget and skill.</li>
            <li>Program eligibility and current terms reviewed.</li>
            <li>90-day target set: first sale, first $100, or first $500.</li>
          </ul>
        </div>
        <div class="card">
          <h3>Account Setup</h3>
          <ul class="checklist">
            <li>Seller Central, KDP, Merch, Associates, Influencer, or Handmade account started.</li>
            <li>Business records, payment details, tax information, and 2FA ready.</li>
            <li>Official fee calculators reviewed before pricing.</li>
          </ul>
        </div>
        <div class="card">
          <h3>Product and Listing</h3>
          <ul class="checklist">
            <li>CLOVER research completed.</li>
            <li>Listing title, bullets, images, and keywords drafted.</li>
            <li>Compliance, IP, trademark, safety, and review rules checked.</li>
          </ul>
        </div>
        <div class="card">
          <h3>Launch and Growth</h3>
          <ul class="checklist">
            <li>Traffic plan created: PPC, content, email, social, or storefront.</li>
            <li>Account Health reviewed weekly.</li>
            <li>Second channel planned only after the first channel has clean data.</li>
          </ul>
        </div>
      </div>
    </section>

    <section class="section" id="resources">
      <h2>Official Resource Links</h2>
      <div class="link-grid">
        <a class="lesson-link" href="https://sell.amazon.com/" target="_blank" rel="noreferrer">Sell on Amazon</a>
        <a class="lesson-link" href="https://sell.amazon.com/fulfillment-by-amazon" target="_blank" rel="noreferrer">Fulfillment by Amazon</a>
        <a class="lesson-link" href="https://sellercentral.amazon.com/revcal" target="_blank" rel="noreferrer">Amazon Revenue Calculator</a>
        <a class="lesson-link" href="https://merch.amazon.com/" target="_blank" rel="noreferrer">Merch on Demand</a>
        <a class="lesson-link" href="https://sell.amazon.com/programs/handmade" target="_blank" rel="noreferrer">Amazon Handmade</a>
        <a class="lesson-link" href="https://affiliate-program.amazon.com/" target="_blank" rel="noreferrer">Amazon Associates</a>
        <a class="lesson-link" href="https://affiliate-program.amazon.com/influencers" target="_blank" rel="noreferrer">Amazon Influencer Program</a>
        <a class="lesson-link" href="https://brandservices.amazon.com/" target="_blank" rel="noreferrer">Amazon Brand Registry</a>
        <a class="lesson-link" href="https://advertising.amazon.com/solutions/products/sponsored-products" target="_blank" rel="noreferrer">Sponsored Products</a>
        <a class="lesson-link" href="https://kdp.amazon.com/" target="_blank" rel="noreferrer">Kindle Direct Publishing</a>
        <a class="lesson-link" href="https://kdp.amazon.com/help/topic/G5TFR9WSHB46ZKFN" target="_blank" rel="noreferrer">Kindle Vella Update FAQ</a>
        <a class="lesson-link" href="https://sell.amazon.com/blog/amazon-account-health-rating" target="_blank" rel="noreferrer">Account Health Rating</a>
      </div>
      <div class="callout warning">Final reminder: check official Amazon pages before launch. Fees, eligibility, commission rules, and program names change.</div>
    </section>

    <footer class="footer">
      <p>Module 33 - The Creator Plug Academy</p>
    </footer>
  </main>
  <script>
    document.querySelectorAll(".copy-button").forEach((button) => {
      button.addEventListener("click", async () => {
        const target = document.getElementById(button.dataset.copy);
        if (!target) return;
        await navigator.clipboard.writeText(target.innerText);
        const original = button.innerText;
        button.innerText = "Copied";
        setTimeout(() => { button.innerText = original; }, 1200);
      });
    });
  </script>
</body>
</html>
