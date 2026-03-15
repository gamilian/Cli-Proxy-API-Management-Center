# Changelog

All notable changes to this project will be documented in this file.

## [1.1.8] - 2026-03-15

### Added
- **Page-based Quota Refresh**: A new "Refresh Quota" button in the Auth Files Management header. It intelligently refreshes credentials based on the **current provider filter** and **only for files on the current page**.
- **Improved Filter for Problematic Credentials**: Credentials with real-time authentication errors (e.g., 401 Unauthorized detected during quota refresh) are now correctly identified and displayed when the "Only show problematic credentials" filter is enabled.
- **Smart Batch Deletion**: The "Delete Problematic Credentials" functionality now includes files with real-time quota errors, allowing for more comprehensive cleanup of invalid tokens.

### Changed
- Updated `AuthFilesPage` UI to include the new refresh action.
- Refined `useAuthFilesData` hook to better handle session-level invalid tokens.

### Fixed
- **Quota Display in "All" View**: Fixed a bug where quota information was hidden when the filter was set to "All". Now all supported credentials display their quota status in all views.
