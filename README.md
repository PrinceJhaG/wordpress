# WordPress Plugin Scaffold

A minimal starting point for the WordPress plugin this repository is intended to contain. The plugin's final name, purpose, supported versions, and functionality are not defined yet.

## Status

This branch adds a plugin entry file and this setup guide. The entry file contains a WordPress plugin header and a direct-access guard; it does not add user-facing functionality.

## File structure

```text
.
├── README.md
└── plugin-name.php
```

Keep the first implementation in the main file while it remains small. Add an `includes/` directory only when a confirmed feature needs a separate class or module.

## Naming placeholders

Before packaging or release, replace the following placeholders consistently:

- Rename `plugin-name.php` to a stable, lowercase plugin slug, for example `your-plugin-slug.php`.
- Set `Plugin Name` to the approved display name.
- Set `Description` to a short description of implemented behavior.
- Set `Author` to the responsible person or organisation.
- Set `Text Domain` to the final plugin slug.

The example values are placeholders, not product or compatibility decisions.

## Local setup

1. Choose the plugin name and slug.
2. Put the renamed main file in a folder whose name matches the slug.
3. Copy that folder into a local WordPress installation's `wp-content/plugins/` directory.
4. Activate it from the WordPress Plugins screen.
5. For a syntax-only check, run `php -l your-plugin-slug.php` with PHP installed.

No WordPress or PHP minimum version has been declared or tested by this scaffold.

## Development

- Keep changes focused on behavior that has been agreed for the plugin.
- Validate, sanitize, and escape data at the appropriate boundaries when a feature handles input or output.
- Add hooks, settings, routes, or integrations only when required by the confirmed feature.
- Record tested WordPress and PHP versions before declaring compatibility.

## First implementation milestone

1. Confirm the plugin's intended user problem and first feature.
2. Approve the display name, slug, author, and supported WordPress/PHP versions.
3. Implement one small end-to-end feature with the relevant access checks and input/output handling.
4. Verify activation and the feature on the declared test environment; record the results here.

## License

No license has been selected for this repository. Add a license only after the repository owner confirms the intended terms.
