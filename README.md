# AFTR

A nightlife discovery and booking app that makes going out effortless. Discover clubs and events, explore venues, reserve tables, and secure entry tickets, all in one place. Find your next night out, book your spot, and enjoy the experience without the hassle.

Three kinds of users: **customers** going out, **venues** (owners and managers), and **promoters** — "PR" in Italian nightlife, people who bring guests in and manage lists. Requirements below are split into **functional** (what it does), **non-functional** (how it behaves: speed, security, reliability), and **domain** (nightlife and Italian-regulatory rules the software has to follow).

---

## Functional requirements

### Account & roles
- **Sign-up and login** email/phone or social sign-up, with separate account types for customer, venue, and promoter, so everyone gets the tools built for their role right away.
- **Role selection** venue and promoter accounts go through a short approval step before going live, so the platform knows who it's dealing with before handing out booking or list tools.
- **Profile editing** customers manage prefs and payment methods; venues manage business details, photos, and licenses; promoters manage agency and affiliated venues.
- **Password recovery** reset by email or SMS, with two-factor login required for venue and promoter accounts, since those are tied to payouts and guest lists.

### Discovering venues & events
- **Event feed with filters** browse events by date, genre, price, minimum age, and entry type (list or map view), so customers find a night out fast and venues get discovered by people actively looking.
- **Venue page** photos, address, hours, capacity, dress code, and services, so customers know what to expect and venues field fewer repeat questions.
- **Event page with line-up** DJs, times, prices, and rules on one page with a booking button, turning a browse into a booking.
- **Favorites and notifications** follow venues, DJs, and promoters and get alerted to new events and last spots, without either side paying for social ads every time.

### Table booking
- **Interactive floor plan** see which tables are free, where they are, and what they cost, so venues sell the best spots without endless chats and calls.
- **Booking with deposit** hold a table with a deposit or card on file, deducted from the minimum spend — fewer no-shows for the venue, a guaranteed table for the customer.
- **Split payment between friends** the organizer creates the table and shares a link; the table confirms once everyone's paid their share.
- **Self-service changes and cancellations** change time, party size, or cancel from the app, with automatic refunds where the policy allows.

### Tickets & entry
- **Digital ticket with QR code** buy in advance (early/standard/last-minute pricing) and get a QR ticket in the app wallet — no queue, and venues know numbers ahead of time.
- **Guest list entry** sign up to a venue's or promoter's list and get a confirmed arrival window, replacing lists kept on WhatsApp and paper.
- **Ticket transfer to a friend** send a ticket to a friend under their own name if plans change, instead of risking a shady resale.
- **Staff check-in app** QR scanning, name search, age checks, and a live headcount for faster, more controlled entry.

### Venue area
- **Event creation and recurring templates** set up an event (or a weekly template) once — line-up, prices, capacity, tables — and publish it everywhere.
- **Real-time dashboard** tickets sold, tables booked, entries vs. capacity, and revenue by channel, all without counting by hand.
- **Staff roles and permissions** separate accounts for owner, manager, cashier, door, and promoters, so everyone sees only what they need.
- **Automatic payouts and reports** per-event revenue summaries, itemized fees, and an export ready for the accountant.
- **Regular customers and campaigns** spot returning customers and lapsed ones, and message only the people who opted in.
- **Promoted listings** pay to boost an event in the feed and search for a set window, with view/click stats — more visibility without looking like spam.

### Promoter area
- **Personal link and QR code** every sign-up or sale through a promoter's link is attributed to them automatically, no arguments about who brought whom.
- **Guest lists with quotas** the venue sets a name quota and closing time; the promoter manages it all from the app.
- **Automatic commissions** calculated on actual entries or sales, with a running statement — no end-of-month disputes.
- **Stats and goals** link visits, sign-ups, attendance, and conversion in one dashboard, with bonuses at set thresholds.

### Trust, safety & messaging
- **Verified venue badge** venues submit VAT and license info for a check before getting a verified badge, so customers can tell real listings from copycats.
- **Verified promoter badge** a promoter gets verified once a venue confirms the relationship from its own dashboard.
- **Direct messages and contact requests** customers can message a venue or promoter about a booking; venues/promoters can send a gated invite (e.g. VIP) that needs accepting before a chat opens — no cold messages either way.
- **Block and report** anyone can block or report a conversation, with reports going to a moderation queue.
- **Verified reviews** only customers with a confirmed check-in can review an event, keeping out fake or rival reviews.

---

## User stories
One story per functional feature above, in backlog-ready format.

### Account & roles
- **US-01** As a new user, I want to sign up with email, phone, or social login, so that I can start using AFTR under the right role right away.
- **US-02** As a venue or a promoter, I want my account to go through a short approval step, so that customers know they're dealing with a vetted business or promoter.
- **US-03** As a user, I want to keep my profile information up to date, so that the people I book with or work with always see accurate details.
- **US-04** As a user, I want to reset my password by email or SMS, so that I can get back into my account without contacting support.

### Discovering venues & events
- **US-05** As a customer, I want to filter events by date, genre, price, age limit, and entry type, so that I can find a night out that fits what I'm looking for in seconds.
- **US-06** As a customer, I want to see a venue's photos, hours, capacity, dress code, and services, so that I know what to expect before I go.
- **US-07** As a customer, I want to see an event's line-up, times, prices, and rules on one page, so that I can decide and book without hunting for information.
- **US-08** As a customer, I want to follow venues, DJs, and promoters, so that I hear about new events without having to search for them.

### Table booking
- **US-09** As a customer, I want to see which tables are free and what they cost on a floor plan, so that I can pick the spot I want before booking.
- **US-10** As a customer, I want to hold a table with a deposit, so that it's guaranteed to be mine when I arrive.
- **US-11** As a customer, I want to split a table's cost with my friends through a shared link, so that no one has to front the whole amount.
- **US-12** As a customer, I want to change or cancel my booking from the app, so that I don't have to call the venue for routine changes.

### Tickets & entry
- **US-13** As a customer, I want to buy my entry ticket in advance with a QR code, so that I can skip the queue at the door.
- **US-14** As a customer, I want to sign up for a venue's or promoter's guest list, so that I can get in under my own name without buying a ticket.
- **US-15** As a customer, I want to transfer my ticket to a friend, so that I don't lose my money if I can't make it.
- **US-16** As a door staff member, I want to scan QR codes and search names against the guest list, so that I can let people in quickly and know how many are inside.

### Venue area
- **US-17** As a venue, I want to create an event or reuse a weekly template, so that I don't have to re-enter the same details every week.
- **US-18** As a venue, I want a real-time dashboard of tickets, tables, entries, and revenue, so that I know how the night is going without counting by hand.
- **US-19** As a venue, I want to give my staff different levels of access, so that each person only sees what their role needs.
- **US-20** As a venue, I want an automatic, itemized payout report after each event, so that I don't have to reconcile the books by hand.
- **US-21** As a venue, I want to message only the customers who opted in, so that I can bring back regulars without spamming everyone.
- **US-22** As a venue, I want to pay to boost an event's visibility for a set period, so that I can get more bookings during a slow week or a new launch.

### Promoter area
- **US-23** As a promoter, I want a personal link and QR code, so that every customer I bring in is automatically attributed to me.
- **US-24** As a promoter, I want to manage my own quota of guest-list names and closing time, so that I don't have to work from chats and spreadsheets.
- **US-25** As a promoter, I want my commissions calculated automatically from actual entries or sales, so that I don't have to argue about numbers at the end of the month.
- **US-26** As a promoter, I want a dashboard of my link visits, sign-ups, and conversion rate, so that I can see what's working and chase my bonus thresholds.

### Trust, safety & messaging
- **US-27** As a venue, I want to submit my VAT number and license for a check, so that I get a verified badge that sets me apart from copycat listings.
- **US-28** As a promoter, I want a venue to confirm my relationship with them, so that I get a verified badge customers can trust.
- **US-29** As a customer, I want to message a venue or promoter about my booking, so that I can get quick answers without leaving the app.
- **US-30** As a user, I want to block or report another user, so that I can stop unwanted contact.
- **US-31** As a customer, I want to leave a review only after a confirmed check-in, so that my feedback counts as genuine and reviews stay trustworthy.

---

## Non-functional requirements
- **Handling traffic peaks** 95% of requests under 2 seconds even when many people book at once; a waiting queue instead of errors beyond capacity.
- **Availability and recovery** 99.9% uptime, updates scheduled outside weekend nights, backups restorable within an hour.
- **Offline check-in** the staff app pre-downloads lists and tickets, works without signal, and syncs (flagging duplicates) once it's back.
- **Secure payments and anti-fraud** card data never touches our servers, 3-D Secure on payments, and a signed single-use QR that can't be screenshotted and reused.
- **Privacy and GDPR** marketing consent kept separate from service consent, minimal data collection, account deletion on request, lists visible only to those entitled to see them.
- **Mobile usability** one-handed use, dark theme, booking in under a minute, WCAG 2.1 AA accessible.
- **Multi-venue and scalability** one platform, many venues and cities, each venue's data kept separate, growth handled without slowdown.
- **No double bookings** a table or ticket is held during payment and recorded once, even on a retry — no overbooking to untangle mid-shift.

---

## Domain requirements
Italy-specific; product guidelines, not legal advice.

- **Minimum age per event** shown before purchase, checked at the door — selling or serving alcohol to under-18s is illegal.
- **Maximum capacity** sales capped at the venue's authorized capacity, with a live headcount for staff.
- **Fiscally compliant ticketing** tickets issued through a system that can generate the SIAE fiscal seal where required (to confirm per event with SIAE or an accountant).
- **No resale above face value** tickets can only be transferred at the price paid, no open resale market — Italian law bars reselling show tickets outside the official issuing system.
- **Admission conditions** dress code, entry rules, and cut-off times shown and accepted before payment, so fewer arguments at the door.
- **Table rules** minimum spend, max party size, and a hold time, after which an unclaimed table goes back on sale.
- **Promoter list rules** name quotas, a closing time, and commissions earned only on confirmed check-ins.
- **Alcohol and hours** no alcohol sold or served 3–6 am by law (except New Year's and Ferragosto nights), plus whatever local ordinances a given city adds.
- **Refunds for fixed-date events** Italian consumer law excludes the usual distance-sale withdrawal right for a specific night out; if the venue cancels, refunds go out automatically.

The ticketing and resale rows are the most delicate confirm them with SIAE or an accountant before selling real tickets.

---

## Sources
Checked online in September 2026. Not legal advice.

- Ban on selling/serving alcohol to under-18s: [Dequo](https://www.dequo.it/articoli/vendere-alcolici-a-minori)
- No alcohol sales 3–6 am, clubs included: [Studio Cataldi](https://www.studiocataldi.it/articoli/36199-vendita-e-somministrazione-di-alcool.asp)
- Municipal ordinances vary by city: [Lentepubblica](https://lentepubblica.it/cittadini-e-imprese/divieto-alcol-ai-minori-stretta-dei-sindaci-ordinanze-in-tutta-italia/)
- Fiscal seal / SIAE smart card in ticketing systems: [CNR test plan](https://openportal.isti.cnr.it/data/2007/160865/2007_160865.pdf), [example tender spec](https://lnx.marcheteatro.it/wp-content/uploads/2020/09/informatizzazione-biglietteria_Allegato1.pdf)
- Secondary ticketing (Law 232/2016, art. 1, par. 545): [Il Sole 24 Ore](https://en.ilsole24ore.com/channel/soleonline5/type/articolo/uuid/AEooe7hB), [Corriere Comunicazioni](https://www.corrierecomunicazioni.it/?p=226632)
- No withdrawal right for fixed-date leisure services (Consumer Code, art. 59): [ECC-Net Italia](https://ecc-netitalia.it/wp-content/uploads/Newsletter_interattive_pdf/2014/18_Newsletter_ECC_Net_Italia_ottobre2014.pdf), [Brocardi](https://brocardi.it/codice-del-consumo/parte-iii/titolo-iii/capo-i/sezione-ii/art59.html)
