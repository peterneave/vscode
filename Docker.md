# Convert slide deck into HTML

docker run --rm -v .:/home/marp/app/ -e LANG=$LANG marpteam/marp-cli README.md

# Convert slide deck into PDF (using Chromium in Docker)

docker run --rm --init -v .:/home/marp/app/ -e LANG=$LANG marpteam/marp-cli README.md --pdf

# Convert slide deck into PPTX (using Chromium in Docker)

docker run --rm --init -v .:/home/marp/app/ -e LANG=$LANG marpteam/marp-cli README.md --pptx

# Watch mode

docker run --rm --init -v .:/home/marp/app/ -e LANG=$LANG -p 37717:37717 marpteam/marp-cli -w README.md

# Server mode (Serve current directory in http://localhost:8080/)

docker run --rm --init -v .:/home/marp/app -e LANG=$LANG -p 8080:8080 -p 37717:37717 marpteam/marp-cli -s .
