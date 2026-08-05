# wsb-pulse-live

Static snapshot of the [wsb-pulse](https://github.com/aasenevan-dot/evanaasen-obsidian-vault) dashboard — r/wallstreetbets ticker mention velocity + sentiment, scraped from old.reddit via Lightpanda.

Regenerate + publish:

    cd ~/wsb-pulse
    .venv/bin/python scrape_lightpanda.py --threads 8
    .venv/bin/python export_static.py --out <this-repo>/index.html
    git commit -am "snapshot" && git push

Not investment advice. Sentiment is VADER + a WSB slang lexicon.
