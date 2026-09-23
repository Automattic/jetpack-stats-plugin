# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## 0.1.0-alpha - unreleased

This is an alpha version! The changes listed here are not final.

### Added
- Add a Settings tab to the Stats dashboard, to choose who can view Stats, which views are counted, and whether the admin bar shows a traffic chart.
- Add the views chart and Stats link to the admin bar, a Stats column to the Posts and Pages lists, and the Stats widget to the WordPress dashboard.
- Connection: Surface SSL certificate verification failures reported by WordPress.com as a connection error notice.
- Initial scaffold for the standalone Jetpack Stats plugin.
- My Jetpack: Allow the Automattic for Agencies banner to be dismissed.

### Changed
- Boost: Wait up to four minutes for slow speed tests in My Jetpack instead of timing out after two.
- Charts: follow the WordPress admin color scheme for chart series colors.
- Charts: update chart grid, axis and label colors immediately when the theme changes.
- Connection: Show every connection error in one notice, each with the account it affects, and link to Site Health when a firewall is blocking WordPress.com.
- Document the WordPress.com connection, Sync and daily site report in the readme.
- Document the WordPress.com Tracks service and link to the plugin source code in the readme.
- General: Update minimum WordPress version to 7.0.
- Hide WordPress admin notices on the Stats dashboard, and let hosts show or hide the Stats sidebar entry.
- Link the Stats packages and the Odyssey Stats dashboard source in the readme.
- My Jetpack: answer module switch clicks immediately, and explain what happened when a change fails.
- My Jetpack: Restyle dashboard notices to match the WordPress design system.
- My Jetpack: Show the dashboard in the new rounded admin page frame.
- My Jetpack: Show the Jetpack menu notification badge when a connection error is detected.
- My Jetpack: Show what Paid Stats actually adds — UTM tracking, device stats, and region & city locations — instead of commercial use.
- Show the Stats dashboard on a site with no connection instead of redirecting to My Jetpack.
- Sidebar: sort Jetpack menu items alphabetically, pinning My Jetpack to the top and external links and Settings to the bottom.
- Stop bundling the Blaze package, which nothing in the plugin starts.
- Tested up to WordPress 7.1.
- Update package dependencies.

### Removed
- Updated PHP version requirements to PHP 7.4 or newer.

### Fixed
- Charts: draw labels at the design system's font weight and size.
- Connection: Fix a stale connection error notice that could persist on healthy sites.
- Connection: Hide connection error notices from users who cannot fix the connection.
- Fix access for users whose allowed role is not their first assigned role.
- JITM: Fix missing messages and a console error on sites without the Jetpack plugin active.
- Keep admin icons colored after the @wordpress/icons 16 update, which draws them as strokes.
- Keep excluding a visitor IP address from tracking when it is written in another form.
- My Jetpack: Fix the dashboard failing to load on WordPress.com-hosted sites.
- My Jetpack: Keep keyboard focus on the first or last data point when an arrow key reaches the end of the stats chart, return focus to the chart when Escape closes a tooltip, stop a focused chart from swallowing keys it does not use such as Page Down, and close the tooltip when the series it describes is hidden.
- My Jetpack: Keep the Automattic for Agencies banner hidden after dismissing it and switching tabs.
- My Jetpack: keep the stats chart tooltip under sticky and fixed page elements.
- My Jetpack: Show each notice once instead of twice.
- My Jetpack: Show Stats as active when the Jetpack Stats plugin runs without the Jetpack plugin.
- My Jetpack: Show the right product status as soon as fresher plan data is available, instead of reusing an earlier lookup.
- My Jetpack: Stop repeating the partner lookup request on every page load.
- My Jetpack: Stop the Stats dashboard from asking which plan you want again after Start for Free was already chosen.
- Report the same visitor address the rest of Jetpack resolves on sites with a trusted IP header configured.
- Return focus to bar charts after pressing Escape, and select the bar under the pointer for tooltips and pointer callbacks.
- Status: Detect a site served on any 127.0.0.0/8 loopback address, or on 0.0.0.0, as a local site.
- Stop recording a malformed visitor IP address.
