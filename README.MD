### Run

```
DO_TOKEN=YOUR_TOKEN
SSH_FINGERPRINT=YOUR_KEY_FINGERPRINT

terraform plan \
-var "do_token=${DO_TOKEN}" \
-var "pub_key=$HOME/.ssh/dokey.pub" \
-var "pvt_key=$HOME/.ssh/dokey" \
-var "ssh_fingerprint=$SSH_FINGERPRINT"

terraform apply \
-var "do_token=${DO_TOKEN}" \
-var "pub_key=$HOME/.ssh/dokey.pub" \
-var "pvt_key=$HOME/.ssh/dokey" \
-var "ssh_fingerprint=$SSH_FINGERPRINT"

```
