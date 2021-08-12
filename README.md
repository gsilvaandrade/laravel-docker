# Build Dockerfile
docker build -t laravel .

# Run image
docker run -d --name laravel -p 8000:8000 laravel

# Run changing CMD on Dockerfile
docker run -d --name laravel -p 8001:8001 laravel --host=0.0.0.0 --port=8001

# Logs
docker logs laravel -f