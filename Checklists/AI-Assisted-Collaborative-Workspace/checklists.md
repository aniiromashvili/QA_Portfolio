# Checklist - AI-Assisted Collaborative Workspace

### Folder & Directory Management
- [ ] Verify that a user can create a nested folder structure up to 5 levels deep without system timeouts.
- [ ] Verify that dragging and dropping an asset between two directory trees updates the path instantly.
- [ ] Verify that creating a folder with an identical name inside the same directory triggers a duplicate naming error.
- [ ] Verify that deleting a parent folder recursively removes all nested sub-folders and updates the UI tree view.
- [ ] Verify that special characters (e.g., `_`, `-`, `@`) in folder names render cleanly without layout breaks.

### Editor & Formatting Interface
- [ ] Verify that a text block strictly locks and prevents further input once the 10,000 character boundary limit is reached.
- [ ] Verify that rich text modifiers (Bold, Italic, Bulleted Lists) persist their styling states after a page reload.
- [ ] Verify that simultaneous collaborative session changes sync in real-time across multiple active viewports.
- [ ] Verify that pasting formatted external clipboard content into the canvas does not break container padding rules.
