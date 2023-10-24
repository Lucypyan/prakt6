from ubuntu:latest

run apt-get update && apt-get install -y \
x11-apps \
xauth \
&& rm -rf /var/lib/apt/lists/*

env DISPLAY=:0

CMD ["xeyes"]