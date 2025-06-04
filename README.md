# Coturn Docker Deployment

This project provides a simple way to run a [Coturn](https://github.com/coturn/coturn) TURN server using Docker and `docker-compose`. Coturn is an open-source TURN/STUN server that helps with NAT traversal for WebRTC and other real-time communication applications.

## Features

- **Easy deployment**: Start a TURN server with a single command using Docker Compose.
- **Custom configuration**: Coturn is configured via the provided `turnserver.conf` file.
- **Authentication**: Example credentials are set for demonstration and testing.
- **TLS Support**: Ready to use with your own certificates.
- **Port forwarding**: All necessary TURN/STUN ports are exposed and mapped.

## Quick Start

1. **Configure certificates**

   Place your TLS certificate (`cert.pem`) and private key (`key.pem`) in the `certs/` folder. Make sure to update the paths in `turnserver.conf` if needed.

2. **Start the server**

   ```bash
   docker-compose up -d
   ```
