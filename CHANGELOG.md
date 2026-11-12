# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.1.0-alpha] - unreleased

This is an alpha version! The changes listed here are not final.

### Added
- Add Stats v2 and its WooCommerce section, off until the site opts in, as the Jetpack plugin does.
- Connection: Add a Connected view to the Users page listing users with a linked WordPress.com account.
- Connection: Note that moving a Jetpack plan is an additional step when transferring connection ownership, and link to the support doc on transferring a plan.
- Connection: Show connection errors on the Connectors card, and keep showing the connection owner when their account connection breaks.
- Connection: Transfer connection ownership to another administrator without leaving your site.
- Connection: Transfer connection ownership to another connected administrator from the Connectors page.
- My Jetpack: Add an Available filter to the Features list.
- My Jetpack: Add catalog-controlled Pro offers and preserve existing plan management.
- My Jetpack: Recognize Jetpack Pro subscriptions and licenses.
- Premium Analytics: Add a Last 3 years period to the date menu, charted by years, so traffic can be compared year by year without picking a custom range.
- Premium Analytics: Add an Arrange tabs option to the Stats v2 page options menu, to reorder the tabs and choose the one that opens first.
- Premium Analytics: Add previous and next arrows beside the date range picker that step the range by its own length, as classic Stats does.
- Premium Analytics: Offer a quarterly interval in the Traffic summary and the WooCommerce tab on ranges of a year or longer.
- Premium Analytics: Offer a yearly chart interval on any date range that covers three calendar years.
- Site Health: Add Jetpack connection details to the Info tab and the copied site info report.

### Changed
- Connection: Ask for confirmation before disconnecting your user account, and offer to transfer ownership first when you own the connection.
- Connection: Link the connection owner's name on the Connectors card to their profile, and update the card without reloading the page when a non-owner disconnects their account.
- Connection: Show a clear message when connecting the site to WordPress.com from the Connectors card fails, instead of WordPress.com's raw error text.
- Connection: Use one wording across My Jetpack and the Connectors screen for the consent notice shown before connecting, for Offline Mode, and for the ownership lock.
- Connection: When disconnecting the site from the Connectors card, list the plugins that will stop working and link to help.
- Explain in the Visitor consent settings that views may drop once Stats follows visitor consent.
- Leave a bar chart column empty when its value is zero, instead of drawing a thin bar that looks like a small count.
- Mark the keyboard-selected bar in the My Jetpack stats chart with a focus ring that shows on any bar color.
- My Jetpack: Connect a WordPress.com account from feature cards that need one. Show feature states through switches or buttons instead of redundant Active or Inactive badges, and show host restrictions below descriptions. Leave features out of Available when their only action is an install you cannot make.
- My Jetpack: Highlight expiring and expired plans in the account panel under your avatar, list them first with a renew link, and show other plans as active until their renewal date.
- My Jetpack: Keep focus on pricing tooltip icons when they open, announce their content to screen readers, and show a focus ring after clicking them.
- My Jetpack: Leave the recommendation to install or activate plugins included in a bundle plan out of the Jetpack menu notification badge.
- My Jetpack: Line up notices with the cards below them, and drop the grey background behind the Features grid and list buttons.
- My Jetpack: On the Features tab, keep a plugin's switch busy until its card is up to date after a failed change, or after any change on sites that also run Jetpack.
- My Jetpack: Open supported Modules links in Features when Jetpack is active.
- My Jetpack: Open the Jetpack Connection details on the Connectors screen from the header's Manage connection link.
- My Jetpack: Refresh Pro availability while preserving existing offers.
- My Jetpack: Return to the license screen after you connect your account from "Activate a license", and show the WordPress.com connection screen made for your site's plugins.
- My Jetpack: Return to the page you were on after you connect your account or restore the connection from the header, and show the WordPress.com connection screen made for your site's plugins.
- My Jetpack: Show a Features tab in place of the Products tab.
- My Jetpack: Show product cards flat, without a drop shadow.
- My Jetpack: Show the avatar and connection status control in the header by default, with access to connection and plan details.
- My Jetpack: Show the Features page on sites in Offline Mode, without connecting to WordPress.com.
- My Jetpack: Show the stats chart tooltip on the dark WordPress design system tooltip surface.
- My Jetpack: Stop asking to connect a WordPress.com account when nothing in use needs one.
- My Jetpack: Turn a module on once Install Jetpack or Activate Jetpack on its card finishes setup.
- Premium Analytics: Load Stats v2 sooner when it is opened from the admin menu.
- Premium Analytics: Load the All-time stats and Most popular day widgets faster by skipping the share counts they never show.
- Premium Analytics: Move the Stats v2 settings from a dashboard tab to their own page, reached from the page options menu.
- Premium Analytics: Name the post detail traffic tab and the highlights and views cards for the content type, such as Product traffic.
- Premium Analytics: Open post and video reports on the date range of the page that linked to them.
- Premium Analytics: open the Top posts and the other Traffic lists tall enough to show ten entries by default.
- Premium Analytics: Remove the feedback banner and menu option from the new Stats once classic Stats is retired.
- Premium Analytics: Serve the author page from /report/author/<id>; the old /author/<id> address redirects.
- Premium Analytics: Show exact figures in single-figure widgets, shortening them only where they would be clipped.
- Premium Analytics: Show the first Stats v2 widgets sooner.
- Premium Analytics: Show the selected section tab in the design system colors instead of the admin theme color.
- Premium Analytics: Show the Top locations views as one-click toggles instead of a dropdown.
- Stats: Mark the jetpack-stats/update-settings ability as destructive, since it overwrites the saved Stats settings.
- Stats v2: Let the number of dashboard columns follow the width of the page, up to six.
- Stats widget: show a skeleton of the widget while it loads, in place of the spinner.
- Stop counting visitors who have not allowed statistics cookies on sites that run the WP Consent API.
- Update package dependencies.
- Update TOS links

### Fixed
- Charts: Wait for a chart's size before drawing it, so charts and their legends no longer jump into place as a page loads.
- Connection: Explain why connecting the site failed instead of showing a raw or generic error.
- Connection: Fix reconnecting your WordPress.com account so it no longer disconnects other users and clears the broken-connection notice on the first attempt.
- Connection: Fix the Safe Mode window in My Jetpack opening empty, with no choices.
- Connection: Keep the progress indicator on screen after clicking Restore Connection until the redirect to WordPress.com.
- Connection: Let users without admin access reconnect their own broken account from the connection error notice.
- Connection: Show connection owner names containing characters like & correctly.
- Connection: Stop Site Health from showing spurious connection failures — remove the redundant outbound HTTP/HTTPS checks, and no longer prompt a reconnect when the WordPress.com connection test is inconclusive.
- Connection: Stop users who cannot set up the site connection from becoming the connection owner when the owner's connection is missing.
- Connection: Translate the Connectors card's text on sites that don't use English.
- Count visitors who allowed statistics when a performance plugin delays the WP Consent API script.
- Count visitors who have not made a consent choice on opt-out sites when a performance plugin delays the WP Consent API script.
- Declare support for the WP Consent API, so its Site Health check no longer lists Jetpack Stats as not conforming.
- Footer: Show the Features link to administrators only.
- Let the pointer take over from the arrow keys in the stats chart, instead of flickering between the hovered and selected bars.
- My Jetpack: Ask for a user connection on the Overview connection card as soon as a plugin that needs one is switched on, without a reload.
- My Jetpack: Bring the first Features results into view after changing the filter or search while scrolled down.
- My Jetpack: Fill checked checkboxes in the Features list with the selected filter's color, show their focus ring only for keyboard focus, and show one focus ring per control instead of two.
- My Jetpack: Fix a fatal error when activating Jetpack Stats beside an older Jetpack plugin.
- My Jetpack: Fix the layout of the connection screen for right-to-left languages.
- My Jetpack: Fix the Overview showing a product's old status after a feature is switched on or off on the Features tab.
- My Jetpack: Fix the Security and Growth filters on the Features tab showing no features.
- My Jetpack: Hide other plugins' notices while the setup screen is open, and stop the full-screen layout breaking when another plugin adds an admin body class first.
- My Jetpack: Keep the Help tab's cards inside their column on narrow screens.
- My Jetpack: Make the connection screen's Connect button and footer links reachable on shorter screens.
- My Jetpack: Open pricing tooltips with the keyboard and dismiss them with Escape.
- My Jetpack: Point users who cannot connect the site at an administrator, instead of an onboarding screen they cannot complete.
- My Jetpack: Report a broken connection on the connection card instead of claiming everything looks good, and show a break only the connection owner can repair as a warning to everyone else.
- My Jetpack: Return to the tab you came from with the back link on product upgrade screens.
- My Jetpack: Show the correct product status and use the active plugin copy when turning products on or off with both stable and Beta or development copies installed.
- My Jetpack: Show the highest-priority notice first when several are set at once.
- My Jetpack: Show what went wrong and let users retry when the onboarding connection to WordPress.com fails.
- My Jetpack: Stop asking for a user connection on the Overview connection card as soon as the plugin that needed one is switched off, without a reload.
- My Jetpack: Stop offering retired Security and Growth plans while preserving existing subscriptions.
- My Jetpack: Stop reporting an error when switching VideoPress off while the Jetpack plugin is inactive.
- My Jetpack: Stop showing $0.00 for paid plans on recommendation cards when prices cannot be loaded.
- My Jetpack: Stop showing an empty account avatar on the Overview connection card on sites without a connection owner when nothing in use needs a user connection.
- My Jetpack: Stop showing an empty account avatar on the Overview connection card when nothing in use needs a user connection.
- My Jetpack: stretch the tab content background to the full height of the page.
- Name each pie chart segment, so a screen reader reads the breakdown instead of an empty chart.
- On sites running the WP Consent API, count AMP views only after the visitor allows statistics in an AMP consent banner. AMP pages without one, AMP pages not rendered by the AMP plugin, and Web Stories are no longer counted there.
- Premium Analytics: Fix Jetpack icon alignment and spacing in page headers.
- Premium Analytics: Improve page transitions between reports and detail views.
- Premium Analytics: Keep Stats under My Home in the admin menu on WordPress.com, where it had dropped below Hosting and Upgrades.
- Premium Analytics: Keep the month in month labels for Japanese, Chinese and Korean sites, which showed a day marker instead (2021年1日 rather than 2021年1月).
- Premium Analytics: Keep Year in review and Subscriber highlights in columns after switching dashboard tabs.
- Premium Analytics: Move an old Year to date or All time link to today's window when its saved interval no longer fits, so the address bar matches the charts.
- Premium Analytics: Move a preset's dates to the new day when a page is left open past midnight, so the numbers and the date controls include today.
- Premium Analytics: Open the dashboard for old Stats links on WordPress 7.2 instead of a page-not-found error.
- Premium Analytics: Read a preset as the window it names today in the date controls, the interval menu and the comparison, as the widgets do, so a bookmark with older dates no longer names last week in the date tooltip and the calendar, or compares this week against the wrong one.
- Premium Analytics: Stop long row names in cards such as Top UTM from running under the views count on hover.
- Premium Analytics: Stop screen readers from announcing widget content as dimmed outside edit mode.
- Premium Analytics: Use the locale's default date format when the site's Date Format setting lacks a day, month or year, so chart labels and the date selector stay unambiguous.
- Show view counts in the Pages list, and any list with more than 100 posts, instead of leaving them blank.
- Stats: Open Stats v2 from old Stats links and stop offering to switch back to classic Stats once the classic Stats page is retired.
- Stats card: Announce the chart correctly to screen readers.
- Stats v2: Leave the plan usage card out of the Settings tab when the plan has no view limit, instead of saying usage isn't available.
- Stop showing free-plan paywalls in wp-admin on a site whose plan already includes those stats.
- Stop store money charts repeating y-axis labels, such as $1, $1, $2, when the store shows fewer decimals than its amounts carry.
- Stop the pricing grid from coming back for up to 5 minutes after choosing Start for free.
- WooCommerce: Keep report widgets loading while a new store's analytics data is prepared, instead of showing an error.

## 1.0.0 - 2026-09-23
### Added
- Initial release of Jetpack Stats as a standalone plugin.

[1.1.0-alpha]: https://github.com/Automattic/jetpack-stats-plugin/compare/1.0.0...1.1.0-alpha
