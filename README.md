# DiscAtlas website prototype

An interactive, single page concept based on the [DiscAtlas users, user stories, and use case scenarios](https://docs.google.com/document/d/1252b8yEUJAdJCLTg5IX1H1eXZWr8KbsK0kSmY-W7lhE/edit). Open `index.html` in a browser or serve the folder with `python3 -m http.server 8000` and visit `http://localhost:8000`.

The eight molds and three brands are **illustrative**, not verified product records. User data is stored in browser `localStorage`. Sign in is a named demo session and **does not provide secure authentication**. The role selector illustrates separate workflows and **does not enforce permissions**. This prototype is for product review, not deployment with real users.

## Story coverage

| Stories | Working prototype flow |
| --- | --- |
| US-01–08 | Search, brand pages, detailed filters, mold profiles, comparison, similar molds, community reviews, new arrivals |
| US-09–19 | Demo account, player profile, bag, collection, want to try, favorites, write reviews, submit flight and trait data, recommendations, directional alternatives |
| US-20–22 | Plain language flight guidance, beginner filter, guided Disc Finder with explained matches |
| US-23–26 | Numeric and physical filters, profile based community segments, official vs community flight display, plastic information |
| US-27–29 | Use votes, edit and remove own reviews, report content |
| US-30–31 | Brand suggestion form and clearly labeled official vs community information |
| US-32–36 | Reference data editor, plastic associations, moderation queue, role assignment screen, separate data presentation |

### Interactions to try

1. Explore **Discover**, filter by speed and stability, open a mold, and compare it with another.
2. Use **Disc Finder**, create a demo profile, save discs to **My Bag**, and visit **For You**.
3. Submit a review and community flight rating. Filter community ratings by throw distance.
4. Report a review, then use the footer **Team workspace** link and the Moderator view to resolve it.
5. In the Brand view, submit a correction. In Content admin, review it and edit a mold or attach plastics.

## Implementation boundary

The screens and browser interactions cover all 36 stories as a design prototype. Production fulfillment of US-09, US-30, US-32, US-34, and US-35 requires an authenticated backend, verified manufacturer identities, server side authorization, persistent database, and a real moderation audit trail. The current recommendation and community aggregate methods operate on the small sample catalog and local submissions.
