# webring

This is a single-file, static webring coordinator.
It does require javascript in order to function.
Member sites will link back to the list and the script will redirect users to the next or previous page in the ring.

---

When linking to this site, the query portion of the url should contain `q=next`, `q=prev`, or `q=rand` to go to the next, previous, or a random page respectively.
The referring site is checked and used to locate the correct index in the list. If there is no match then the webring landing page will be shown.

---

This webring in particular is available at `goodgirl.club`. New members can request to join via an issue or pull-request on this git repo.
Prior to joining, you will need to have a link to the ring present on the webpage you want to link. Here's some example code for that purpose:

```html
<div>
  <a href="https://goodgirl.club?q=prev">← Previous</a>
  <a href="https://goodgirl.club">GoodGirl.Club Webring</a>
  <a href="https://goodgirl.club?q=rand">Random</a>
  <a href="https://goodgirl.club?q=next">Next →</a>
</div>
```
