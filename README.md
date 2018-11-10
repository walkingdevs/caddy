## Usage

    cat > $PWD/caddyfile << EOF
    some caddy config...
    EOF    

    docker run --restart always -d \
               --name caddy \
               -v $PWD/caddy:/caddy \
               -p 80:80 \
               -p 443:443 \
               walkingdevs/caddy