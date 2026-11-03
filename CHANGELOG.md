# Changelog

All user-visible changes. The format follows [Keep a Changelog](https://keepachangelog.com/).

## [Unreleased]

### Changed (breaking)
- Widget API 2 for Dashboard (formerly Homelab Dashboard, getdashboard.dev): the element is
  `dash-<id>`, the action event `dash-widget-action`, the theme properties `--dash-*`, and examples
  use `{{DASHBOARD_VAR_*}}`. The package is `dashboard-widget-example-counter`, the repository
  `stefanrenne/dashboard-widget-example`. Needs Dashboard 0.19.0.

## [1.2.0] - 2026-11-02

### Added
- A Reset button: `action` in server.js (widget API 1, dashboard 0.8.0) starts the change again
  from the next value; client.js sends `hd-widget-action` and is disabled while `busy`.
- Attributes `value` and `full` for a service's `filter:` (`filter: widget.full == false` hides
  the card until the number reaches max). Needs dashboard 0.12.0; older dashboards ignore them.

## [1.1.0] - 2026-10-25

### Added
- `npm run rename -- <id>`: gives the template your widget's id everywhere.

## [1.0.0] - 2026-10-24

### Added
- The `example-counter` widget: a number from a JSON API and its change since the last refresh.
