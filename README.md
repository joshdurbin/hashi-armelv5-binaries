# hashi-armelv5-binaries

Compile instructions

## consul-template

- Clone consul-template: `git clone git@github.com:hashicorp/consul-template.git`
- Checkout `v0.25.1`: `git checkout v0.25.1`
- Compile for PI Zero ARM: `env GOOS=linux GOARCH=arm GOARM=5 go build`
- Compress (w/ zip) the output: `zip consul-template-v0.25.1-armelv5.zip consul-template`
- Checkout this repo: `git clone git@github.com:joshdurbin/hashi-armelv5-binaries.git`
- Add file: `git add consul-template-v0.25.1-armelv5.zip`
- Commit: `git commit -m 'adding consul-template for pi zero'`
