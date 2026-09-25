# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.1-alpha] - unreleased

This is an alpha version! The changes listed here are not final.

### Changed
- My Jetpack: Keep focus on pricing tooltip icons when they open, announce their content to screen readers, and show a focus ring after clicking them.

### Fixed
- Connection: Let users without admin access reconnect their own broken account from the connection error notice.
- Let the pointer take over from the arrow keys in the stats chart, instead of flickering between the hovered and selected bars.
- My Jetpack: Fix the layout of the connection screen for right-to-left languages.
- My Jetpack: Open pricing tooltips with the keyboard and dismiss them with Escape.
- My Jetpack: Point users who cannot connect the site at an administrator, instead of an onboarding screen they cannot complete.
- My Jetpack: Report a broken connection on the connection card instead of claiming everything looks good, and show a break only the connection owner can repair as a warning to everyone else.
- My Jetpack: stretch the tab content background to the full height of the page.
- Stop the pricing grid from coming back for up to 5 minutes after choosing Start for free.

## 1.0.0 - 2026-09-23
### Added
- Initial release of Jetpack Stats as a standalone plugin.

[1.0.1-alpha]: https://github.com/Automattic/jetpack-stats-plugin/compare/1.0.0...1.0.1-alpha
