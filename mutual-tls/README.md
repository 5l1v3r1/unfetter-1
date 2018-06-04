## WARNING!
The certificates generated by these scripts should *NOT* be viewed as secure, they are for testing purposes only!

The following files contain passwords uses in the certificates: `grep -ln password ./*`

If you *insist* on using these scripts, replace those passwords with something more secure before generating the certificates.

---

## Instructions

### Create server certificates, client certificate authority, and testclient certificates

- `./init.sh`
- Start/restart stack
- `./test_taxii.sh`
    - Prettified: `./test_taxii.sh | python -m json.tool`

### Create additional certifications for distribution

- `./new_client.sh {name}`

---

This folder was taken from the following open source project: [https-demo](https://github.com/mmendelson222/https-demo)

The scripts have been modified.