# Prometheus Collector - Quick Collect

This is just a little docker-compose to make it easy to take prometheus metrics endpoint output and send it to Honeycomb.

# Process

1. Scrape a prometheus endpoint output and replace what's in metrics/index.html
2. export your HONEYCOMB_API_KEY into your environment variables
3. run `docker compose up`
