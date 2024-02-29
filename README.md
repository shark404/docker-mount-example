
A simple example showing a caching issue with Orbstack on Mac.

```bash
docker compose build test
echo 'Test' > ./data/test.txt && ls -la ./data/test.txt && docker compose run --rm test bash -c 'ls -la /app/data/test.txt'
```