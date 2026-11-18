# Plumbing Emergency Playbook

Static directory site (Python + Markdown), same generator pattern as shred-directory and directory-site. Planned URL: https://plumbing.christiejustice.com (GitHub Pages; NOT deployed yet).

    python3 build.py            # build into dist/ (drafts excluded)
    python3 serve.py            # preview at http://127.0.0.1:8000

Add a page: content/pages/<slug>.md with front matter title, slug, description, last_updated, optional draft/listings. Only sourced facts; no invented businesses, phones, prices, reviews.
Deploy (when approved): create GitHub repo, push to main; .github/workflows/pages.yml publishes; static/CNAME holds the domain; DNS CNAME needed.
data/ and tools/ are gitignored (private earnings/outreach notes).
