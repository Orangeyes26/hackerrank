# eRD Cowork — prototype

Single-file interactive prototype of the eRD Cowork semiconductor R&D analytics
workspace. Open `erd-cowork.html` directly in a browser — no build, no server,
no network access required (React, ECharts and the icon set are bundled).

## What is in this build

- **Cowork studio** — chat column + artifact preview panel, resizable, with a
  collapsible artifact panel (rail on the right edge when collapsed).
- **Data sources** — connectors and uploaded files, shown together on the
  artifact panel's top-right pill and snapshotted per artifact version.
- **Artifact sharing** — 4-step request wizard (recipients → purpose → approval
  evidence → review), save-as-draft, multi-approver, pasted evidence with
  lightbox preview.
- **Access guidance** — full-page sign-in wall and in-flow share gate for users
  without the required A4 role, with the group name, role, entitlements and
  admin contact.
- **Language toggle** — the share flow and the access-guidance screens follow
  the 中 / EN switch in the avatar menu. The rest of the UI is Chinese.
- **Environment / version tags** — UAT / UAT·dev / UAT·sbx / STG / PROD pills in
  the header, with build and deploy info in the avatar menu.

## Demo switches

The avatar menu (top right) has a **DEMO · 模擬權限** section that toggles the
`ERD_COWORK_USER` and `ERD_COWORK_SHARE_USER` entitlements, so the two
no-permission flows can be shown without a backend. The same menu cycles the
environment tag.
