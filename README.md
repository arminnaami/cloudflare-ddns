# cloudflare-ddns
This Dockerfile will keep your Docker containers public IP address up to date with a CloudFlare DNS A record (Dynamic DNS).
(Based on the work of Marcus Hughes <hello@msh100.uk to better fit UNRAID)

Usage

To use, run the Docker container with your CloudFlare API credentials found on your CloudFlare account page

docker run -e 'CF_EMAIL=your@cloudflare_email.com' \
           -e 'CF_HOST=sub.domain.com' \
           -e 'CF_API=a1b2c3d4e5' \
            mace/cloudflare-ddns
To run in the background, add the -d switch to docker run.
