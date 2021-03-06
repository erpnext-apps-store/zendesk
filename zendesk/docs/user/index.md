## Zendesk

#### Installation

This application requires [Frappe](https://github.com/frappe/frappe) and [ERPNext](https://github.com/frappe/erpnext) v11.0.0 or higher.

1. `bench get-app zendesk https://github.com/DOKOS-IO/zendesk/`
2. `bench install-app zendesk`
3. `bench restart && bench migrate`

In Zendesk, enable Token Access and create a new API token in "Channels > API"
<img class="screenshot" alt="Zendesk API" src="{{docs_base_url}}/assets/zendesk_api.png">

In ERPNext, add your email address (the admin email address in Zendesk), the API credentials, and your subdomain in Zendesk Settings.
Example: if you domain is `dokos.zendesk.com`, your subdomain is `dokos`.

Verify that your scheduler is enabled (`bench enable-scheduler`) if you want to sync zendesk and erpnext every three-four minutes.

#### Features

{index}
