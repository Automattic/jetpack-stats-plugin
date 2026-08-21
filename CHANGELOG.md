# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## 0.1.0-alpha - unreleased

This is an alpha version! The changes listed here are not final.

### Added
- Initial scaffold for the standalone Jetpack Stats plugin.

### Changed
- Document the WordPress.com Tracks service and link to the plugin source code in the readme.
- General: Update minimum WordPress version to 7.0.
- Link the Stats packages and the Odyssey Stats dashboard source in the readme.
- My Jetpack: Show what Paid Stats actually adds — UTM tracking, device stats, and region & city locations — instead of commercial use.
- Show the Stats dashboard on a site with no connection instead of redirecting to My Jetpack.
- Stop bundling the Blaze package, which nothing in the plugin starts.
- Tested up to WordPress 7.1.

### Fixed
- My Jetpack: Stop the Stats dashboard from asking which plan you want again after Start for Free was already chosen.
