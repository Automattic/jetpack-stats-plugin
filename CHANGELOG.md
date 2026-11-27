# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.1.0-alpha] - unreleased

This is an alpha version! The changes listed here are not final.

### Security
- Stats: Limit subscriber data to subscriber counts, so users who can view Stats cannot read the subscriber list.

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
- Premium Analytics: Add an Items sold widget to the WooCommerce analytics dashboard.
- Premium Analytics: Add a time-since-send control to the opens and clicks charts on the post page's email tabs: the first 24 hours by the hour, the first week or 30 days by the day, or all time by the month.
- Premium Analytics: Add a zoom-out button beside the date arrows that returns to the period a chart was zoomed in from.
- Premium Analytics: Add Download CSV to the Devices and Top platforms cards.
- Premium Analytics: Add Download CSV to the post, video and email detail cards.
- Premium Analytics: Add Download CSV to the Traffic summary card.
- Premium Analytics: Add Download CSV to the Views over years, Monthly posting activity and Subscriber summary cards.
- Premium Analytics: Add Items sold to the Store performance metrics.
- Premium Analytics: Add previous and next arrows beside the date range picker that step the range by its own length, as classic Stats does.
- Premium Analytics: Let a click on a point or bar in the WooCommerce tab charts set the dashboard to that period, and open the previous period for a click on a previous-period point or bar in any chart.
- Premium Analytics: Let the Top tags & categories widget show only tags or only categories.
- Premium Analytics: Offer a quarterly interval in the Traffic summary and the WooCommerce tab on ranges of a year or longer.
- Premium Analytics: Offer a yearly chart interval on any date range that covers three calendar years.
- Premium Analytics: Open the WooCommerce tab on a disconnected store set to report from its own data.
- Premium Analytics: Reload the analytics dashboard once when part of it fails to load after an update, instead of showing an error. WordPress.com sites only.
- Site Health: Add Jetpack connection details to the Info tab and the copied site info report.

### Changed
- Abilities: Make the Stats abilities available to AI agents by default. Return false from the jetpack_wp_abilities_enabled filter in an mu-plugin to turn them off.
- Connection: Ask for confirmation before disconnecting your user account, and offer to transfer ownership first when you own the connection.
- Connection: Link the connection owner's name on the Connectors card to their profile, and update the card without reloading the page when a non-owner disconnects their account.
- Connection: Show a clear message when connecting the site to WordPress.com from the Connectors card fails, instead of WordPress.com's raw error text.
- Connection: Use one wording across My Jetpack and the Connectors screen for the consent notice shown before connecting, for Offline Mode, and for the ownership lock.
- Connection: When disconnecting the site from the Connectors card, list the plugins that will stop working and link to help.
- Explain in the Visitor consent settings that views may drop once Stats follows visitor consent.
- Leave a bar chart column empty when its value is zero, instead of drawing a thin bar that looks like a small count.
- Load the Stats page faster.
- Make view counts easier to compare across the heatmaps, so quiet periods can be told apart instead of sharing one pale shade, and mark months the data does not yet fill.
- Mark the keyboard-selected bar in the My Jetpack stats chart with a focus ring that shows on any bar color.
- My Jetpack: Call the header's connection panel and its button "Jetpack Connection", without repeating it in the button's name during a connection error.
- My Jetpack: Connect a WordPress.com account from feature cards that need one. Show feature states through switches or buttons instead of redundant Active or Inactive badges, and show host restrictions below descriptions. Leave features out of Available when their only action is an install you cannot make.
- My Jetpack: Highlight expiring and expired plans in the account panel under your avatar, list them first with a renew link, and show other plans as active until their renewal date.
- My Jetpack: Keep focus on pricing tooltip icons when they open, announce their content to screen readers, and show a focus ring after clicking them.
- My Jetpack: Leave the recommendation to install or activate plugins included in a bundle plan out of the Jetpack menu notification badge.
- My Jetpack: Line up notices with the cards below them, and drop the grey background behind the Features grid and list buttons.
- My Jetpack: On sites with Jetpack Pro, replace "Purchase a plan" with "Upgrade to Complete", which goes straight to checkout.
- My Jetpack: On the Features tab, keep a plugin's switch busy until its card is up to date after a failed change, or after any change on sites that also run Jetpack.
- My Jetpack: Open supported Modules links in Features when Jetpack is active.
- My Jetpack: Open the Jetpack Connection details on the Connectors screen from the header's Manage connection link.
- My Jetpack: Refresh Pro availability while preserving existing offers.
- My Jetpack: Remember whether you last picked the grid or the list layout on the Features tab, and open the tab in that layout next time.
- My Jetpack: Remove the Features link from the footer, since the header already links to it.
- My Jetpack: Return to the license screen after you connect your account from "Activate a license", and show the WordPress.com connection screen made for your site's plugins.
- My Jetpack: Return to the page you were on after you connect your account or restore the connection from the header, and show the WordPress.com connection screen made for your site's plugins.
- My Jetpack: Show a Features tab in place of the Products tab.
- My Jetpack: Show product cards flat, without a drop shadow.
- My Jetpack: Show the avatar and connection status control in the header by default, with access to connection and plan details.
- My Jetpack: Show the Features page on sites in Offline Mode, without connecting to WordPress.com.
- My Jetpack: Show the stats chart tooltip on the dark WordPress design system tooltip surface.
- My Jetpack: Show the WordPress.com connection screen made for your site's plugins when you connect your account from the Features tab.
- My Jetpack: Stop asking to connect a WordPress.com account when nothing in use needs one.
- My Jetpack: Turn a module on once Install Jetpack or Activate Jetpack on its card finishes setup.
- Premium Analytics: Draw the text inside dashboard widgets at 14px, as classic Stats did, with headline figures in bold, so lists and figures are easier to read.
- Premium Analytics: Drop the "N more" count below the Latest subscribers list.
- Premium Analytics: Hide the Subscribers tab in Stats v2, since its Newsletter feature needs the Jetpack plugin.
- Premium Analytics: Load Stats v2 sooner when it is opened from the admin menu.
- Premium Analytics: Load the All-time stats and Most popular day widgets faster by skipping the share counts they never show.
- Premium Analytics: Move the Stats v2 settings from a dashboard tab to their own page, reached from the page options menu.
- Premium Analytics: Name the post detail traffic tab and the highlights and views cards for the content type, such as Product traffic.
- Premium Analytics: Open a page's own report, /report/page/<id>, from the Top posts & pages card and the Posts & pages report.
- Premium Analytics: Open post and video reports on the date range of the page that linked to them.
- Premium Analytics: open the Top posts and the other Traffic lists tall enough to show ten entries by default.
- Premium Analytics: Remove the feedback banner and menu option from the new Stats once classic Stats is retired.
- Premium Analytics: Rename the Stats v2 page options menu to Stats options, and show it on the report, connect and upgrade pages so Settings can be reached from every page.
- Premium Analytics: Serve the author page from /report/author/<id>; the old /author/<id> address redirects.
- Premium Analytics: Show exact figures in single-figure widgets, shortening them only where they would be clipped.
- Premium Analytics: Show the first Stats v2 widgets sooner.
- Premium Analytics: Show the selected section tab in the design system colors instead of the admin theme color.
- Premium Analytics: Show the Stats v2 dashboard widgets sooner.
- Premium Analytics: Show the Top locations views as one-click toggles instead of a dropdown.
- Premium Analytics: Show the view options of Top pages, Top platforms, Latest emails sent, All-time traffic and Views over years as one-click toggles instead of a dropdown.
- Premium Analytics: Use the Stats script for WooCommerce store tracking on sites not hosted on WordPress.com, so a pageview no longer adds an uncached request to the site.
- Replace the classic Stats page with the new Stats. The Stats menu and old Stats links now open the new Stats.
- Safe Mode: Show the Jetpack Safe Mode admin bar item while the choice is still pending, style it on the front end of the site too, and have it open My Jetpack from Jetpack pages that can't show the Safe Mode screen.
- Stats: Mark the jetpack-stats/update-settings ability as destructive, since it overwrites the saved Stats settings.
- Stats v2: Let the number of dashboard columns follow the width of the page, up to six.
- Stats widget: show a skeleton of the widget while it loads, in place of the spinner.
- Stop counting visitors who have not allowed statistics cookies on sites that run the WP Consent API.
- Update package dependencies.
- Update TOS links

### Removed
- Settings: Remove the WordPress.com Reader "Show post views for this site" setting, which no longer has any effect.

### Fixed
- Charts: Name a month the date range cuts by its days in the Post views, Video and Author performance tooltips.
- Charts: Name a whole month by its month and year in tooltips, not by its first day.
- Charts: Wait for a chart's size before drawing it, so charts and their legends no longer jump into place as a page loads.
- Connection: Explain why connecting the site failed instead of showing a raw or generic error.
- Connection: Fix reconnecting your WordPress.com account so it no longer disconnects other users and clears the broken-connection notice on the first attempt.
- Connection: Fix the Safe Mode window in My Jetpack opening empty, with no choices.
- Connection: Keep a Safe Mode screen left open, for example in another tab, from disconnecting a site that is no longer in Safe Mode.
- Connection: Keep the progress indicator on screen after clicking Restore Connection until the redirect to WordPress.com.
- Connection: Let a second administrator fix a broken connection owner by connecting their own account, which makes them the new owner.
- Connection: Let users without admin access reconnect their own broken account from the connection error notice.
- Connection: Show clearer messages when the connect request to your site fails, for example because its REST API is disabled or a PHP error broke the response.
- Connection: Show connection owner names containing characters like & correctly.
- Connection: Stop showing a connection error notice for a request signature mismatch, which reconnecting rarely fixes.
- Connection: Stop Site Health from showing spurious connection failures — remove the redundant outbound HTTP/HTTPS checks, and no longer prompt a reconnect when the WordPress.com connection test is inconclusive.
- Connection: Stop users who cannot set up the site connection from becoming the connection owner when the owner's connection is missing.
- Connection: Translate the Connectors card's text on sites that don't use English.
- Count visitors who allowed statistics when a performance plugin delays the WP Consent API script.
- Count visitors who have not made a consent choice on opt-out sites when a performance plugin delays the WP Consent API script.
- Declare support for the WP Consent API, so its Site Health check no longer lists Jetpack Stats as not conforming.
- Fix the Stats dashboard failing to load on WordPress 7.2.
- Footer: Show the Features link to administrators only.
- Format numbers in the site's full locale, so Traditional Chinese sites read 萬 instead of 万.
- Let the pointer take over from the arrow keys in the stats chart, instead of flickering between the hovered and selected bars.
- My Jetpack: Announce the same connection status on the header's account button as in its panel, and read that status first when the panel opens from the keyboard.
- My Jetpack: Ask for a user connection on the Overview connection card as soon as a plugin that needs one is switched on, without a reload.
- My Jetpack: Bring the first Features results into view after changing the filter or search while scrolled down.
- My Jetpack: Don't install a product's plugin when plugin installs are turned off or the user can't install plugins.
- My Jetpack: Explain why a Jetpack Pro license can't be activated on a site.
- My Jetpack: Fill checked checkboxes in the Features list with the selected filter's color, show their focus ring only for keyboard focus, and show one focus ring per control instead of two.
- My Jetpack: Fix a fatal error when activating Jetpack Stats beside an older Jetpack plugin.
- My Jetpack: Fix the layout of the connection screen for right-to-left languages.
- My Jetpack: Fix the Learn more, Manage and Connect buttons on recommendation cards, which did nothing.
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
- My Jetpack: Show the manual-install notice and disable the install buttons on product pricing pages when the site cannot install plugins.
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
- Premium Analytics: Draw the legend labels and values in breakdown charts such as Devices, and the links in a video's Used on posts & pages card, at the same 14px size as the rest of the widget text.
- Premium Analytics: Fix Jetpack icon alignment and spacing in page headers.
- Premium Analytics: Fix short figures such as 9.5 lakh showing as 9 lakh in Hindi and other locales with their own units.
- Premium Analytics: Fix the date arrows landing on a partial day, week or month after clicking today's chart bar.
- Premium Analytics: Improve page transitions between reports and detail views.
- Premium Analytics: Keep a video's Retention rate chart inside its plot when retention is above 100%.
- Premium Analytics: Keep Stats under My Home in the admin menu on WordPress.com, where it had dropped below Hosting and Upgrades.
- Premium Analytics: Keep the days, the Locations tab and the video an old Stats link names when it opens the dashboard.
- Premium Analytics: Keep the Download CSV action in place while a widget refreshes its data, so the Traffic summary chart no longer jumps when returning to the tab.
- Premium Analytics: Keep the Download CSV button on report pages while the report refreshes, so it no longer blinks or drops keyboard focus.
- Premium Analytics: Keep the month in month labels for Japanese, Chinese and Korean sites, which showed a day marker instead (2021年1日 rather than 2021年1月).
- Premium Analytics: Keep the place of a hidden Stats v2 tab when the tab order is saved.
- Premium Analytics: Keep the side padding on the longer option of a card's view toggle, such as Posts & pages on the Top pages card.
- Premium Analytics: Keep the widget title from being cut off beside a toggle, so the toggle folds into the widget controls menu at the same width whichever way the widget is resized.
- Premium Analytics: Keep Year in review and Subscriber highlights in columns after switching dashboard tabs.
- Premium Analytics: Load Stats report rows as the table scrolls, so a report with thousands of rows opens without freezing the browser.
- Premium Analytics: Mark the posts and pages published in the selected period in Top pages, as classic Stats did.
- Premium Analytics: Move an old Year to date or All time link to today's window when its saved interval no longer fits, so the address bar matches the charts.
- Premium Analytics: Move a preset's dates to the new day when a page is left open past midnight, so the numbers and the date controls include today.
- Premium Analytics: Name an untitled post, author or video in the last breadcrumb of its page, as the header does.
- Premium Analytics: Open the dashboard for old Stats links on WordPress 7.2 instead of a page-not-found error.
- Premium Analytics: Open the matching report for old Stats links to a summary page, such as referrers or search terms, and today by the hour for the old hourly Traffic link, instead of the Traffic tab or the dashboard root.
- Premium Analytics: Read a preset as the window it names today in the date controls, the interval menu and the comparison, as the widgets do, so a bookmark with older dates no longer names last week in the date tooltip and the calendar, or compares this week against the wrong one.
- Premium Analytics: Retry loading the site settings after a failed load, so the Homepage link in Posts & Pages and the Settings page can recover without reloading the page.
- Premium Analytics: Shorten the breadcrumb trail and hide the Customizing badge on phones, instead of letting them cover the header buttons.
- Premium Analytics: Show metric cards as a list when the card is too narrow for every metric to fit side by side, instead of cutting off the figures.
- Premium Analytics: Stop a long post title from widening the page on desktop, so the header buttons stay in view.
- Premium Analytics: Stop long row names in cards such as Top UTM from running under the views count on hover.
- Premium Analytics: Stop screen readers from announcing widget content as dimmed outside edit mode.
- Premium Analytics: Stop the customize buttons covering the breadcrumb trail on a narrow screen.
- Premium Analytics: Stop the pinned report header from jumping when a trackpad scroll overshoots the end of a report.
- Premium Analytics: Use the locale's default date format when the site's Date Format setting lacks a day, month or year, so chart labels and the date selector stay unambiguous.
- Premium Analytics: Wrap long titles in the report tables so the other columns stay in view on narrow screens.
- Safe Mode: Show the WordPress.com address correctly instead of reversed after Safe Mode checks the connection again.
- Safe Mode: Stop showing the Safe Mode screen to non-admins once an admin has chosen to stay in Safe Mode.
- Show the upgrade page prices in your local currency when your WordPress.com account is not connected to the site.
- Show view counts in the Pages list, and any list with more than 100 posts, instead of leaving them blank.
- Stats: Open Stats v2 from old Stats links and stop offering to switch back to classic Stats once the classic Stats page is retired.
- Stats card: Announce the chart correctly to screen readers.
- Stats v2: Leave the plan usage card out of the Settings tab when the plan has no view limit, instead of saying usage isn't available.
- Stop showing free-plan paywalls in wp-admin on a site whose plan already includes those stats.
- Stop store money charts repeating y-axis labels, such as $1, $1, $2, when the store shows fewer decimals than its amounts carry.
- Stop the pricing grid from coming back for up to 5 minutes after choosing Start for free.
- Stop the upgrade screen from briefly offering Jetpack Complete before Jetpack Pro.
- WooCommerce: Keep report widgets loading while a new store's analytics data is prepared, instead of showing an error.

## 1.0.0 - 2026-09-23
### Added
- Initial release of Jetpack Stats as a standalone plugin.

[1.1.0-alpha]: https://github.com/Automattic/jetpack-stats-plugin/compare/1.0.0...1.1.0-alpha
