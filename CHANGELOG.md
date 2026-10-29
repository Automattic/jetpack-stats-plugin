# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.1.0-alpha] - unreleased

This is an alpha version! The changes listed here are not final.

### Added
- Connection: Add a Connected view to the Users page listing users with a linked WordPress.com account.
- Connection: Show connection errors on the Connectors card, and keep showing the connection owner when their account connection breaks.
- Connection: Transfer connection ownership to another administrator without leaving your site.
- Connection: Transfer connection ownership to another connected administrator from the Connectors page.
- My Jetpack: Add an Available filter to the Features list.
- My Jetpack: Add catalog-controlled Pro offers and preserve existing plan management.
- My Jetpack: Recognize Jetpack Pro subscriptions and licenses.

### Changed
- Connection: Ask for confirmation before disconnecting your user account, and offer to transfer ownership first when you own the connection.
- Connection: Link the connection owner's name on the Connectors card to their profile, and update the card without reloading the page when a non-owner disconnects their account.
- Connection: Show a clear message when connecting the site to WordPress.com from the Connectors card fails, instead of WordPress.com's raw error text.
- Connection: Use one wording across My Jetpack and the Connectors screen for the consent notice shown before connecting, for Offline Mode, and for the ownership lock.
- Connection: When disconnecting the site from the Connectors card, list the plugins that will stop working and link to help.
- Mark the keyboard-selected bar in the My Jetpack stats chart with a focus ring that shows on any bar color.
- My Jetpack: Connect a WordPress.com account from feature cards that need one. Show feature states through switches or buttons instead of redundant Active or Inactive badges, and show host restrictions below descriptions. Leave features out of Available when their only action is an install you cannot make.
- My Jetpack: Keep focus on pricing tooltip icons when they open, announce their content to screen readers, and show a focus ring after clicking them.
- My Jetpack: Line up notices with the cards below them, and drop the grey background behind the Features grid and list buttons.
- My Jetpack: On the Features tab, keep a plugin's switch busy until its card is up to date after a failed change, or after any change on sites that also run Jetpack.
- My Jetpack: Open supported Modules links in Features when Jetpack is active.
- My Jetpack: Refresh Pro availability while preserving existing offers.
- My Jetpack: Show a Features tab in place of the Products tab.
- My Jetpack: Show product cards flat, without a drop shadow.
- My Jetpack: Show the avatar and connection status control in the header by default, with access to connection and plan details.
- My Jetpack: Show the stats chart tooltip on the dark WordPress design system tooltip surface.
- My Jetpack: Stop asking to connect a WordPress.com account when nothing in use needs one.
- Stop counting visitors who have not allowed statistics cookies on sites that run the WP Consent API.
- Update package dependencies.

### Fixed
- Connection: Explain why connecting the site failed instead of showing a raw or generic error.
- Connection: Fix reconnecting your WordPress.com account so it no longer disconnects other users and clears the broken-connection notice on the first attempt.
- Connection: Fix the Safe Mode window in My Jetpack opening empty, with no choices.
- Connection: Let users without admin access reconnect their own broken account from the connection error notice.
- Connection: Show connection owner names containing characters like & correctly.
- Connection: Stop Site Health from showing spurious connection failures — remove the redundant outbound HTTP/HTTPS checks, and no longer prompt a reconnect when the WordPress.com connection test is inconclusive.
- Connection: Stop users who cannot set up the site connection from becoming the connection owner when the owner's connection is missing.
- Connection: Translate the Connectors card's text on sites that don't use English.
- Let the pointer take over from the arrow keys in the stats chart, instead of flickering between the hovered and selected bars.
- My Jetpack: Ask for a user connection on the Overview connection card as soon as a plugin that needs one is switched on, without a reload.
- My Jetpack: Bring the first Features results into view after changing the filter or search while scrolled down.
- My Jetpack: Fix a fatal error when activating Jetpack Stats beside an older Jetpack plugin.
- My Jetpack: Fix the layout of the connection screen for right-to-left languages.
- My Jetpack: Hide other plugins' notices while the setup screen is open, and stop the full-screen layout breaking when another plugin adds an admin body class first.
- My Jetpack: Keep the Help tab's cards inside their column on narrow screens.
- My Jetpack: Make the connection screen's Connect button and footer links reachable on shorter screens.
- My Jetpack: Open pricing tooltips with the keyboard and dismiss them with Escape.
- My Jetpack: Point users who cannot connect the site at an administrator, instead of an onboarding screen they cannot complete.
- My Jetpack: Report a broken connection on the connection card instead of claiming everything looks good, and show a break only the connection owner can repair as a warning to everyone else.
- My Jetpack: Return to the tab you came from with the back link on product upgrade screens.
- My Jetpack: Show the correct product status and use the active plugin copy when turning products on or off with both stable and Beta or development copies installed.
- My Jetpack: Show the highest-priority notice first when several are set at once.
- My Jetpack: Stop asking for a user connection on the Overview connection card as soon as the plugin that needed one is switched off, without a reload.
- My Jetpack: Stop offering retired Security and Growth plans while preserving existing subscriptions.
- My Jetpack: Stop reporting an error when switching VideoPress off while the Jetpack plugin is inactive.
- My Jetpack: Stop showing an empty account avatar on the Overview connection card on sites without a connection owner when nothing in use needs a user connection.
- My Jetpack: Stop showing an empty account avatar on the Overview connection card when nothing in use needs a user connection.
- My Jetpack: stretch the tab content background to the full height of the page.
- Show view counts in the Pages list, and any list with more than 100 posts, instead of leaving them blank.
- Stats card: Announce the chart correctly to screen readers.
- Stop showing free-plan paywalls in wp-admin on a site whose plan already includes those stats.
- Stop the pricing grid from coming back for up to 5 minutes after choosing Start for free.

## 1.0.0 - 2026-09-23
### Added
- Initial release of Jetpack Stats as a standalone plugin.

[1.1.0-alpha]: https://github.com/Automattic/jetpack-stats-plugin/compare/1.0.0...1.1.0-alpha
