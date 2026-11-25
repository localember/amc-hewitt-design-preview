# AMC Hewitt location site: Design preview, not live

Ticket AMC-2026-11-25-hewitt-site-build. Rebuilt the existing homepage-only preview
(localember/amc-hewitt-design-preview) to the full Copperas Cove site standard, including the
Nov 25 review changes: button hover, menu matching the Hewitt live menu minus Home, scroll-away
header (the header is not fixed) plus sticky bottom CTA on pages with hero buttons, and Short Answer
stock images on service and condition pages.

Full Hewitt location site on the AMC main design (Local Ember Alpine, AMC palette). Every URL on
the live hewitt.anthonychiro.com site (page sitemap, post sitemap, and the FAQ in the menu) is kept
at the same slug, except /ai-generated-content-disclaimer/, removed the same way as the Copperas Cove
preview. /science-glp-1-weight-loss/ on the live site redirects to the medical weight loss program;
both addresses exist here with that program's content.

Facts are this office's: 518 North Hewitt Drive, Hewitt, TX 76643, (254) 235-0793, Monday to
Thursday 8:30am to 6:00pm, Friday through Sunday closed. Specials are the three offers on the live
specials page. Team bios and the four Google reviews are carried word for word. There is no
/insurance/ page on the live site, so it is not in the menu.

- noindex,nofollow on every page and robots.txt Disallow: /
- Forms off: disabled inputs and buttons, no form actions, no tracking or third-party scripts
- Service and condition pages use the Local Ember catalog (tools/bd-generator/catalog). Kinesio
  taping has no catalog file; the page uses the design draft from the Georgetown preview with
  Hewitt's office facts. Medical weight loss does not use services/weight-loss.json, because that
  file describes a non-medical program with no medications. The Hewitt program is medical, and
  visits are at the Waco clinic. Botox has no catalog file; the page uses the homepage's own line
  and does not repeat the old article.
- Blog: 2 posts rewritten (car-accident-tips-chiropractor, sciatic-leg-pain); the other 39 are
  placeholders at their exact live URLs
- Legal pages are the Local Ember standards, at the live site's slugs. SMS terms are the program
  terms published on the Hewitt site, including the STOP number (254) 330-3410.
- Review layer: assets/review-comments.js. It is not part of the site design and must not ship live.
- Not the live site. Not sent to the client.
