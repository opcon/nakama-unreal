# Change Log
All notable changes to this project are documented below.

The format is based on [keep a changelog](http://keepachangelog.com/) and this project uses [semantic versioning](http://semver.org/).

## [0.8.1] - 2017-09-28
### Changed
- Now targeting nakama 1.0.1

## [0.8.0] - 2017-09-28
### Added
- A paging cursor can now be serialized and restored.
- New storage partial update feature.
- New storage list feature.
- A session now exposes `.ExpiresAt` and `.Handle` from the token.

### Changed
- Added default builder for notification list and remove messages.
- A group self list operation now return the user's membership state with each group.
- A group leave operation now return a specific error code when the last admin attempts to leave.

## [0.7.0] - 2017-09-26
### Added
- Add new In-App Notification feature.
- Add new In-App Purchase Validation feature.   

### Changed
- Update Client to support the new batching API.

## [0.6.1] - 2017-06-03
### Changed
- Support for Nakama API 0.13.0
- New matchmaking feature.
- Optionally send match data to a subset of match participants.
- Expose a way to toggle `TCP_NODELAY` socket option.
- Send RPC messages to run custom code.
- Fetch users by handle.
- Add friend by handle.
- Filter by IDs in leaderboard list message.
- Storage messages can now set records with public read permission.
- Update user fetch add handle method name to match changes in nakama-unity 0.6.1.

### Fixed
- Dispatch callbacks when sending match data.
- Improve leaderboard list message to handle multiple filters.

## [0.5.1] - 2017-06-01
### Added
- Support for Nakama API 0.12.1
- Support for fetching groups by name.

## [0.5.0] - 2017-06-01
### Added
- Support for Nakama API 0.12.0
- Blueprint support
- Add support for dynamic leaderboards.
- Add error codes for error messages in server protocol.

### Changed
- Update session token parse code for user's handle.
- Update user presence protocol message to contain user handles.

## [0.4.2] - 2017-03-21
### Added
- Initial public release - modeled after nakama-unity 0.4.2
