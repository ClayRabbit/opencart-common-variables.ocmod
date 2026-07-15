# Common Variables for OpenCart

[Русский](README.ru.md)

Quickly use store contact details, customer information, or even GET request parameters in any storefront `.twig` template — without adding the same changes in every controller.

---

## Features

The modification hooks into `system/engine/loader.php` and enriches the `$data` array before a template is rendered. Works on the **storefront only** (not in admin).

### `_config` — store settings

- `{{ _config.name }}` — store name
- `{{ _config.address }}` — address
- `{{ _config.geocode }}` — geocode
- `{{ _config.email }}` — e-mail
- `{{ _config.telephone }}` — telephone
- `{{ _config.fax }}` — fax
- `{{ _config.open }}` — opening hours
- `{{ _config.url }}` — store URL

### `_customer` — current customer

- `{{ _customer.id }}` — customer ID (0 for guests)
- `{{ _customer.firstname }}` — first name
- `{{ _customer.lastname }}` — last name
- `{{ _customer.email }}` — e-mail
- `{{ _customer.telephone }}` — telephone
- `{{ _customer.newsletter }}` — newsletter subscription
- `{{ _customer.group_id }}` — customer group ID

### `_get` — GET parameters

- `{{ _get.route }}` — current route, etc.

---

## Related modules

For the same variables inside admin-edited HTML content, use the **ShortCodes** module from the author's OpenCart Marketplace profile.

Both modules can be used together or separately.

---

## Installation

1. Upload `.ocmod.zip` via **Extensions → Installer**.
2. Go to **Extensions → Modifications** and click **Refresh**.
3. Clear modification and template cache if needed.

---

## Requirements

- OpenCart 2.3 or 3.x

---

## Support

Provided as-is. Paid support and custom work: https://t.me/clayrabbit

---

## License

Free software under the [GNU GPL v3](https://www.gnu.org/licenses/gpl-3.0.html) or later. You may use, modify, and redistribute it under the same license.

---

## Tags

common variables, twig, template variables, store info, customer data, developer tools