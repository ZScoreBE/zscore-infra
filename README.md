# Z-Score infrastructure

This repository has examples on how to set up Z-Score

Z-Score has 2 main parts, the **API** and a front-end called the **console**.
The **api** needs a relational database and an SMTP connection

## Z-Score API environment variables

| Variable Name                               | Description                                                                 | Default | Required |
|---------------------------------------------|-----------------------------------------------------------------------------|---------|----------|
| DATASOURCE_URL                              | Datasource URL. Example: jdbc:mysql://db:3306/z-score                       |         | x        |
| DATASOURCE_USERNAME                         | Datasource username                                                         |         | x        |
| DATASOURCE_PASSWORD                         | Datasource password                                                         |         | x        |
|                                             |                                                                             |         |          |
| SMTP_HOST                                   | SMTP Host                                                                   |         | x        |
| SMTP_PORT                                   | SMTP Port                                                                   |         | x        |
| SMTP_USERNAME                               | SMTP username                                                               |         | x        |
| SMTP_PASSWORD                               | SMTP password                                                               |         | x        |
| SMTP_AUTH_ENABLED                           | is SMTP Auth enabled                                                        |         | x        |
| SMTP_STARTTLS_ENABLED                       | is SMTP start tls enabled                                                   |         | x        |
|                                             |                                                                             |         |          |
| ZSCORE_CORS_ALLOWED_ORIGINS                 | Comma seperated list of allowed CORS origins                                |         | x        |
|                                             |                                                                             |         |          |
| ZSCORE_TOKEN_SECRET                         | JWT Token secret                                                            |         | x        |
| ZSCORE_TOKEN_EXPIRY_DURATION                | JWT token expiry duration in hours                                          |         | x        |
| ZSCORE_REFRESH_TOKEN_EXPIRY_DURATION        | JWT Refresh token expiry duration in hours                                  |         | x        |
| ZSCORE_PLAYER_TOKEN_EXPIRY_DURATION         | JWT Player token expiry duration in hours                                   |         | x        |
| ZSCORE_PLAYER_REFRESH_TOKEN_EXPIRY_DURATION | JWT Player refresh token expiry duration in hours                           |         | x        |
|                                             |                                                                             |         |          |
| ZSCORE_EMAIL_OVERRIDE_TEMPLATES             | Do you want to override the email templates                                 | false   |          |
| ZSCORE_EMAIL_TEMPLATES_PATH                 | Email template path (Required when ZSCORE_EMAIL_OVERRIDE_TEMPLATES is true) | ''      |          |
|                                             |                                                                             |         |          |
| ZSCORE_EMAIL_NO_REPLY                       | No reply email                                                              |         | x        |
| ZSCORE_EMAIL_NO_REPLY_NAME                  | No reply name                                                               |         | x        |
| ZSCORE_EMAIL_ACTIVATION_URL                 | Activation url on the Front-End                                             |         | x        |
| ZSCORE_EMAIL_RESET_PASSWORD_URL             | Reset password url on the Front-End                                         |         | x        |
| ZSCORE_EMAIL_REGISTER_URL                   | Register url on the Front-End                                               |         | x        |


## Z-Score console environment variables

| Variable Name | Description                                                                | Default | Required |
|---------------|----------------------------------------------------------------------------|---------|----------|
| BASE_API_URL  | The api url                                                                |         | x        |
| TERMS_URL     | The link that needs to be shown when clicking the terms and agreement link |         | x        |