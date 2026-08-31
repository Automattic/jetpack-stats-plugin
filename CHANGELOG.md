# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## 0.1.0-alpha - unreleased

This is an alpha version! The changes listed here are not final.

### Added
- Initial scaffold for the standalone Jetpack Stats plugin.
- My Jetpack: Allow the Automattic for Agencies banner to be dismissed.

### Changed
- Boost: Wait up to four minutes for slow speed tests in My Jetpack instead of timing out after two.
- Charts: follow the WordPress admin color scheme for chart series colors.
- Document the WordPress.com connection, Sync and daily site report in the readme.
- Document the WordPress.com Tracks service and link to the plugin source code in the readme.
- General: Update minimum WordPress version to 7.0.
- Link the Stats packages and the Odyssey Stats dashboard source in the readme.
- My Jetpack: Show what Paid Stats actually adds — UTM tracking, device stats, and region & city locations — instead of commercial use.
- Show the Stats dashboard on a site with no connection instead of redirecting to My Jetpack.
- Stop bundling the Blaze package, which nothing in the plugin starts.
- Tested up to WordPress 7.1.

### Removed
- Updated PHP version requirements to PHP 7.4 or newer.

### Fixed
- Charts: draw labels at the design system's font weight and size.
- Fix access for users whose allowed role is not their first assigned role.
- JITM: Fix missing messages and a console error on sites without the Jetpack plugin active.
- Keep excluding a visitor IP address from tracking when it is written in another form.
- My Jetpack: Keep the Automattic for Agencies banner hidden after dismissing it and switching tabs.
- My Jetpack: Stop repeating the partner lookup request on every page load.
- My Jetpack: Stop the Stats dashboard from asking which plan you want again after Start for Free was already chosen.
- Report the same visitor address the rest of Jetpack resolves on sites with a trusted IP header configured.
- Stop recording a malformed visitor IP address.
