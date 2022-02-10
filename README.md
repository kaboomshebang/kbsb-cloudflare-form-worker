# kbsb-cloudflare-form-worker

Process HTML form-data and a hCaptcha token using Cloudflare Workers. 

## Setup wrangler

```bash
# Linux/OSx: install build essentials if not already installed
sudo apt install build-essential

# install Rust
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

# setup wrangler
cargo install wrangler
wrangler login
wrangler generate my-app https://github.com/cloudflare/worker-template

# configure the wrangler.toml
# set values for: name, type, account_id, workers_dev
# https://developers.cloudflare.com/workers/get-started/guide#optional-configure-for-deploying-to-a-registered-domain

# deploy
wrangler dev # to workers.dev
wrangler publish # to Cloudflare global
```

# Resources

https://developers.cloudflare.com/workers/
https://developers.cloudflare.com/workers/examples
https://developers.cloudflare.com/workers/cli-wrangler
