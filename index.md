# Privacy Policy — kaitsuke-radar

Last updated: 2026-10-14

kaitsuke-radar is an internal tool of a small vintage clothing shop, used only by the shop owner
(the "operator") to source inventory. It searches public eBay listings through the eBay Browse API and
notifies the operator of new listings that match the operator's own search criteria, so that the
operator can find items to buy on eBay. It does not list, bid on, or buy items automatically.
The tool has no other users, no sign-in, and no public interface.

## Data we collect

From the eBay Browse API (public listing information only):

- Item ID, title, price, current bid and bid count, buying format, auction end time
- Shipping cost to a fixed U.S. postal code, item location (country), item condition, category
- Image URLs
- Seller feedback percentage and feedback score

We do **not** collect, store, or share eBay user IDs (including seller usernames), passwords,
or any other information that identifies an eBay user. We do not use eBay user tokens and do not
access any eBay member's account.

## How we use the data

Only to notify the operator of new listings and to keep those notifications up to date
(price, availability, and auction status). Listings that do not match the operator's buying criteria may be
ranked for a twice-daily digest, using the operator's own purchase records (not eBay data) and the operator's
reactions to earlier notifications. The data is not used to compute statistics about eBay,
eBay categories, or eBay sellers, and it is not used to train machine-learning or AI systems.

## Storage and retention

- Data is stored in a local database on the operator's own computer.
- Listing details (title, price, images, and similar) are stored only for listings that are notified,
  and are deleted as soon as the notification no longer needs them (no later than 24 hours after
  the notification). For other listings, only the item ID and detection time are stored.
- Item IDs and detection times are kept for 3 days to avoid duplicate notifications. For auctions
  that the operator chose to be reminded of, they are kept until the auction ends.
- For finding useful search terms, the tool keeps only daily counts of words that appear in listing
  titles, for up to 30 days; the titles themselves are not stored.
- Candidates for the twice-daily digest are stored as the item ID, a score, and short reasons for the score
  (such as matched keywords and price range) only, for up to 12 hours. Titles, prices, and images are not stored
  for candidates; they are retrieved again from eBay right before the digest is sent.
- To avoid notifying the same item twice when it is relisted under a new item ID, the tool stores a one-way hash
  of the normalized title and price range for 3 days. The titles themselves are not stored.
- When the operator reacts to a notification (thumbs up or down), the tool keeps only the number of reactions per
  keyword and per price range. Only keywords from the operator's own purchase records and buying criteria are
  counted. Item IDs, titles, and other listing details are not stored for this purpose.
- Old data is deleted automatically every time the tool runs.
- If the operator's participation in the eBay Developers Program ends, all eBay data is deleted
  within 10 days.

## Sharing

We do not sell, rent, share, or disclose eBay data to anyone. Notifications are delivered to a
private Discord server that only the operator can access. Every notification shows the time its
listing information was last retrieved. Priority notifications are refreshed at least every 5 hours
and are reduced to a link after 24 hours (or as soon as the item sells or the listing ends). Digest
notifications are retrieved from eBay right before they are sent. Digest and other notifications are not
refreshed and are reduced to a link before they are 6 hours old.

## Cookies and tracking

This tool has no website for users and uses no cookies, analytics, or tracking.

## Your requests

If you are an eBay user and want to ask about or request deletion of information related to you,
please contact us. Because we do not store information that identifies eBay users, there will
usually be nothing to delete, but we will confirm and respond.

## Contact

kusatake0929 [at] gmail.com

## Changes

We will update this page if our practices change. The date at the top shows the latest version.
