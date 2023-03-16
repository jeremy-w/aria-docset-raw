# aria-docset-raw

This holds the WIP of generating the actual ARIA docset for Dash to eventually submit to https://github.com/Kapeli/Dash-User-Contributions/.

I originally hoped to be able to use Dashing to quickly generate it, but Dashing no longer runs.

## TODO

- Work out how to identify the relevant TOC entries and categorize them
  - This likely means special-casing the handling within Roles and Attributes, and then more general h2 handling for Sections.
  - This work is going on in step 03-inject-toc-anchors.
- Work out sqlite indexing after the entries are in there.
  - This is mostly going to be yanking back out the toc entries we injected and sticking them all in the DB.
  - But will also require indexing the documents themselves and categorizing them appropriately.
  - This work is going on in 04-index-docs.
- At that point, it needs testing locally before getting submitted via my fork of the Dash-User-Contributions repo at https://github.com/jeremy-w/dash-docset-aria.
