# Ansible Role authentik

install [authentik](https://goauthentik.io/)

## Collection dependencies

The role depends on the

- collection community.docker

## Role Variables

<!-- markdownlint-disable MD033 -->
<!-- markdownlint-disable MD034 -->
| group | variable | default | description |
| --- | --- | --- | --- |
| basic | `authentik_image_tag` | `2022.6.3` | the image tag of authentik |
| basic | `authentik_error_reporting` | `false` | the value for [AUTHENTIK_ERROR_REPORTING__ENABLED](https://goauthentik.io/docs/installation/configuration#authentik_error_reporting) |
| basic | `authentik_base_directory` | `/opt/authentik` | the directory for the docker compose configuration |
| secrets | `authentik_pg_pass` | | the value for [PostgreSQL setting](https://goauthentik.io/docs/installation/configuration#postgresql-settings) AUTHENTIK_POSTGRESQL__PASSWORD |
| secrets | `authentik_secret_key` | | the value for [AUTHENTIK_SECRET_KEY](https://goauthentik.io/docs/installation/configuration#authentik_secret_key) |
| bootstrap | `authentik_bootstrap` | true | if [automated install](https://goauthentik.io/docs/installation/automated-install) should be used |
| bootstrap | `authentik_bootstrap_password` | | the value for [AUTHENTIK_BOOTSTRAP_PASSWORD](https://goauthentik.io/docs/installation/automated-install#authentik_bootstrap_password-or-ak_admin_pass) |
| bootstrap | `authentik_bootstrap_token` | | the value for [AUTHENTIK_BOOTSTRAP_TOKEN](https://goauthentik.io/docs/installation/automated-install#authentik_bootstrap_token-or-ak_admin_token) |
| e-mail | `authentik_smtp_host` | |  the value for [AUTHENTIC_EMAIL](https://goauthentik.io/docs/installation/configuration#authentik_email) AUTHENTIK_EMAIL__HOST |
| e-mail | `authentik_smtp_port` | |  the value for [AUTHENTIC_EMAIL](https://goauthentik.io/docs/installation/configuration#authentik_email) AUTHENTIK_EMAIL__PORT |
| e-mail | `authentik_smtp_username` | |  the value for [AUTHENTIC_EMAIL](https://goauthentik.io/docs/installation/configuration#authentik_email) AUTHENTIK_EMAIL__USERNAME |
| e-mail | `authentik_smtp_password` | |  the value for [AUTHENTIC_EMAIL](https://goauthentik.io/docs/installation/configuration#authentik_email) AUTHENTIK_EMAIL__PASSWORD |
| e-mail | `authentik_smtp_tls` | |  the value for [AUTHENTIC_EMAIL](https://goauthentik.io/docs/installation/configuration#authentik_email) AUTHENTIK_EMAIL__USE_TLS |
| e-mail | `authentik_smtp_ssl` | |  the value for [AUTHENTIC_EMAIL](https://goauthentik.io/docs/installation/configuration#authentik_email) AUTHENTIK_EMAIL__USE_SSL |
| e-mail | `authentik_smtp_from` | |  the value for [AUTHENTIC_EMAIL](https://goauthentik.io/docs/installation/configuration#authentik_email) AUTHENTIK_EMAIL__FROM |
