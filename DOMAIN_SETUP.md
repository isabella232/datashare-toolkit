[Back to Datashare](./README.md)

# Overview
Datashare requires two domains, one for the UI, and one for the API layer. We recommend configuring as such:
- https://datashare.your-domain.com/
- https://api.datashare.your-domain.com/

# Pre-requisites
You must have access to administer DNS for the domains that you will use.

# Verifying your domain using the gcloud CLI
Create a DOMAIN environment variable based off the custom subdomain:

```
export DOMAIN=datashare.your-domain.com
```

Verify domain ownership the first time you use that domain in the Google Cloud project:

```
gcloud domains list-user-verified
```

If your ownership of the domain needs to be verified, open the Webmaster Central verification page:

```
gcloud domains verify $DOMAIN
```

# Next
[Setup OAuth credential](./CREDENTIAL_SETUP.md)
