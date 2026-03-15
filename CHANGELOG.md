# Changelog

All notable changes to this project will be documented in this file.

## [1.1.8] - 2026-03-15

### Added
- **Contextual Quota Refresh**: A new "Refresh Quota" button in the Auth Files Management header. It intelligently refreshes credentials based on the active provider filter (e.g., refreshing only Codex files when the Codex filter is active).
- **Improved Filter for Problematic Credentials**: Credentials with real-time authentication errors (e.g., 401 Unauthorized detected during quota refresh) are now correctly identified and displayed when the "Only show problematic credentials" filter is enabled.
- **Smart Batch Deletion**: The "Delete Problematic Credentials" functionality now includes files with real-time quota errors, allowing for more comprehensive cleanup of invalid tokens.

### Changed
- Updated `AuthFilesPage` UI to include the new refresh action.
- Refined `useAuthFilesData` hook to better handle session-level invalid tokens.

### Localization
- Added new translation keys for quota refresh actions in both Chinese (`zh-CN.json`) and English (`en.json`).
