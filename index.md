# Privacy Policy — kaitsuke-radar

Last updated: 2026-10-13

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
(price, availability, and auction status). The data is not used to compute statistics about eBay,
eBay categories, or eBay sellers, and it is not used to train machine-learning or AI systems.

## Storage and retention

- Data is stored in a local database on a computer or private server controlled by the operator.
- Listing details (title, price, images, and similar) are stored only for listings that are notified,
  and are deleted as soon as the notification no longer needs them (no later than 24 hours after
  the notification). For other listings, only the item ID and detection time are stored.
- Item IDs and detection times are kept for 3 days to avoid duplicate notifications. For auctions,
  they are kept until the auction ends.
- For finding useful search terms, the tool keeps only daily counts of words that appear in listing
  titles, for up to 30 days; the titles themselves are not stored.
- Old data is deleted automatically every time the tool runs.
- If the operator's participation in the eBay Developers Program ends, all eBay data is deleted
  within 10 days.

## Sharing

We do not sell, rent, share, or disclose eBay data to anyone. Notifications are delivered to a
private Discord server that only the operator can access. Every notification shows the time its
listing information was last retrieved. Priority notifications are refreshed at least every 5 hours
and are reduced to a link after 24 hours (or as soon as the item sells or the listing ends). Other
notifications are not refreshed and are reduced to a link before they are 6 hours old.

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
