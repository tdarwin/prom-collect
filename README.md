# Prometheus Collector - Quick Collect

This is just a little docker-compose to make it easy to take prometheus metrics endpoint output and send it to Honeycomb.

## Process

1. Scrape a prometheus endpoint output and replace what's in metrics/index.html
2. export your HONEYCOMB_API_KEY into your environment variables

    ```text
    you can also use a .env file to store that environment variable. Docker Compose will pick that up.
    ```

3. run `docker compose up`
4. once you see your metrics in Honeycomb, you can run `docker compose down` (or `ctrl -c` if you didn't background your docker compose process)
