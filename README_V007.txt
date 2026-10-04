Tool Pocket Generator — V007
Release status: Validation build.

Provenance
- Built directly from Tool_Pocket_Generator_V005_CORRECTED.zip.
- V006 was not used as the source.

Authorised change
- New Tool is selectable whether the current working tool came from a photo workflow or Import JSON.
- Selecting New Tool uses the existing complete clean-slate reset, clearing the photo, imported/current project state, physical-grid confirmation, detected outline, all points, added points, straight/curve states, current-tool dimensions, Geometry Check state, relief/editing/transient state, current tool ID and workspace state.
- A fresh New Tool workspace is then presented.

No impact to outline detection
- detectPhoto() unchanged byte-for-byte from V005.
- detectWorkspaceRectangle() unchanged byte-for-byte from V005.
- Import JSON restoration, JSON/STL generation/download, and variable export versioning unchanged.

Checks
- V005 direct source.
- Requested reset state verified in newTool().
- Only updateModeUI() changed functionally.
- V007 title/heading/app title aligned.
- JSON/STL export filenames still use GENERATOR_VERSION.
- ZIP integrity checked.

User validation
1. Import JSON.
2. Confirm New Tool is selectable.
3. Select New Tool.
4. Confirm the imported tool and all working state are cleared.
5. Confirm fresh New Tool workspace.
6. Run fresh photo/grid outline detection and confirm it behaves as before.
