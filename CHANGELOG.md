# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.1.0-alpha] - unreleased

This is an alpha version! The changes listed here are not final.

### Added
- Connection: Add a Connected view to the Users page listing users with a linked WordPress.com account.

### Changed
- My Jetpack: Keep focus on pricing tooltip icons when they open, announce their content to screen readers, and show a focus ring after clicking them.
- My Jetpack: Show a Features tab in place of the Products tab.
- My Jetpack: Show product cards flat, without a drop shadow.
- My Jetpack: Show the stats chart tooltip on the dark WordPress design system tooltip surface.
- My Jetpack: Stop asking to connect a WordPress.com account when nothing in use needs one.

### Fixed
- Connection: Fix reconnecting your WordPress.com account so it no longer disconnects other users and clears the broken-connection notice on the first attempt.
- Connection: Let users without admin access reconnect their own broken account from the connection error notice.
- Connection: Stop Site Health from showing spurious connection failures — remove the redundant outbound HTTP/HTTPS checks, and no longer prompt a reconnect when the WordPress.com connection test is inconclusive.
- Connection: Stop users who cannot set up the site connection from becoming the connection owner when the owner's connection is missing.
- Let the pointer take over from the arrow keys in the stats chart, instead of flickering between the hovered and selected bars.
- My Jetpack: Ask for a user connection on the Overview connection card as soon as a plugin that needs one is switched on, without a reload.
- My Jetpack: Fix the layout of the connection screen for right-to-left languages.
- My Jetpack: Open pricing tooltips with the keyboard and dismiss them with Escape.
- My Jetpack: Point users who cannot connect the site at an administrator, instead of an onboarding screen they cannot complete.
- My Jetpack: Report a broken connection on the connection card instead of claiming everything looks good, and show a break only the connection owner can repair as a warning to everyone else.
- My Jetpack: Stop asking for a user connection on the Overview connection card as soon as the plugin that needed one is switched off, without a reload.
- My Jetpack: Stop reporting an error when switching VideoPress off while the Jetpack plugin is inactive.
- My Jetpack: Stop showing an empty account avatar on the Overview connection card on sites without a connection owner when nothing in use needs a user connection.
- My Jetpack: Stop showing an empty account avatar on the Overview connection card when nothing in use needs a user connection.
- My Jetpack: stretch the tab content background to the full height of the page.
- Stats card: Announce the chart correctly to screen readers.
- Stop showing free-plan paywalls in wp-admin on a site whose plan already includes those stats.
- Stop the pricing grid from coming back for up to 5 minutes after choosing Start for free.

## 1.0.0 - 2026-09-23
### Added
- Initial release of Jetpack Stats as a standalone plugin.

[1.1.0-alpha]: https://github.com/Automattic/jetpack-stats-plugin/compare/1.0.0...1.1.0-alpha
