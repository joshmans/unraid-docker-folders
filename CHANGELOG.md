# Changelog

## 2026.09.13
- refactor(sort): share the folder sort decision and extract sort fields once
- feat(header): show the container and folder counts inside the search field
- feat(settings): group the settings page by what each setting affects
- feat(sort): add a "Sort folders too" toggle to the sort menu
- fix(folders): apply the toolbar sort to folder contents
- build: use content-hashed asset filenames
- fix(folders): do not count removed containers as hidden
- docs: add a contributing guide and require dev as the PR base
- fix(folders): repair the #9 merge and add the sort menu
- Add auto-sort options for folders and folder contents (#9)
- chore: update docs
- refactor: share the paused-start rule and tidy the issue fixes
- feat(updates): add Force Update to the container menu (#11)
- feat(schedules): add a Resume action and let Start resume a paused container (#7)
- fix(docker): resume a paused container from the card and the API (#7)
- fix(schedules): evaluate and show schedule times in the server timezone (#7)
- fix(folders): persist the manual order of unfoldered containers (#12)
- refactor: share the move-to-folder action and the select modal
- feat(updates): name the containers in the update notification
- feat(folders): add a folder picker to the container menu
- fix(compose): rename the Stack Details menu item to Edit Stack
- feat(docker): show the inline log panel in card view
- test(docker): pin the managed-with-autostart-off branch
- fix(docker): correct three faults the browser check found
- feat(docker): put Adopt on the container, not only in the kebab menu
- fix(docker): escape adopted values before they reach Unraid's shell
- feat(docker): adopt CLI-created containers into Unraid's container manager
- fix(ui): keep an open kebab menu inside the frame instead of scrolling
- fix(ui): stop the unfoldered section clipping open kebab menus
- fix(folders): only add/remove containers that changed when saving a folder
- feat(settings): add a "Buy me a coffee" Ko-fi link
- feat(ui): collapse the create buttons into one menu, widen the search
- feat: rename to "Docker Folders" and shorten the page URLs
- feat(ui): one update button, and a re-check inside the confirm modal
- feat(ui): collapse the three create buttons to "+" plus an icon
- fix(ui): render the update-check controls before settings land
- docs: summarize each release in CHANGELOG, stop regenerating it
- chore: drop the beta label from Image Updates settings
- fix(ui): stop compose buttons blinking in while availability is checked
- test: fix session tests broken by PHPUnit output, silence constant warnings
- fix(security): validate every user-influenced filesystem path
- chore: prepare repo for Community Applications submission
- feat: show release notes in the update confirm modal
- feat: list containers before updating, and update several at once
- feat: show a container's schedules in its expanded card
- fix: read logs from TTY containers, brighten secondary text, link container icons
- feat: replace container status dot/bar with a halo around the icon
- feat: restructure expanded container card and widen its click target
- fix: modals and add create container button
- fix: schedules modal
- Faint tint on collapsed folders; fix expand animation snapping open
- Replace folder left-border accent with expanded-state gradient tint
- Add design guardrails (DESIGN.md) and migrate off palette colors
- Remove live connection status indicator from main header
- Hide icon-only Docker Containers title bar variant
- Fix legacy button hiding on the native Docker page
- Add settings to hide legacy Docker containers and buttons
- Add targeted update checks for containers and compose stacks
- Sync package-lock.json with package.json
- Add GitHub Actions release workflows for main and dev
- Fix cron registration: write to plugin config dir, drop user field
- Pin yarn in .prototools to match packageManager
- Show conflicting ports in expanded container details
- Add port conflict badge for stopped containers
- Fix update-check cron registration and link Update badge to release notes
- Add container/stack scheduling and backup system
- Add container expand/collapse animation and brighten info text
- Optimize container stats with cgroup reads and slow-data caching
- Add compose file version history with rollback support
- Fix modal close button alignment, populate faded preview from compose file
- Consolidate modals, simplify compose folder UI, fix validation env
- Compose editor: logs tab, recompose flow, save lock, YAML highlighting
- Disable text wrapping in compose/env monospace textareas
- Add Logs tab to edit-stack modal with auto-refresh, fix modal layout bugs
- Force textarea resize/fill with !important to beat Unraid global CSS
- Stream compose stack start, fix create-stack textarea and banner flash
- Fix compose plugin import banner for users without compose.manager
- Render all modals in parent window to escape iframe clipping
- Fix folder counts, cleanup deleted containers, unify modals, delete image option
- Fix autostart: read/write Unraid's flat file, not just XML templates
- Fix: hide .title div before inject comment, not after
- Hide empty .title div generated by Unraid for inject page
- Fix autostart detection, add delay support, modal UIs, accordion width
- Extract icons into reusable components; uniform sizes; always-visible globe/autostart
- Add Create Stack button and container autostart toggle
- Fix compose UX: conditional play/stop, container sync, PortBindings
- add test files
- Fix compose SHA256 hash, empty folder UX, and import banner persistence
- Fix Docker Compose v2.32.4 SHA256 hash after upstream binary update
- Render compose modal in parent page DOM to avoid iframe clipping
- Lock parent scroll when modal open via wheel/touch/key event prevention
- Elevate iframe z-index when modal open; fix input/textarea styling
- Fix modal buttons and tabs overridden by Unraid button reset
- Fix modal overlay coverage, sizing, tab styling; add compose export feature
- Fix modal clipping: cap overlay to available iframe space instead of expanding iframe
- Fix scroll feedback loop: lock parent scroll while modal is open
- Fix modal clipping in iframe: direct height floor + correct max-height
- Fix compose modal visibility in iframe and title color
- Fix compose import file migration, modal z-index, and editor styling
- Fix compose UI: controls visibility, import banner, mock data alignment
- Add Docker Compose management feature
- Fix CHANGELOG.md entries for 2026.03.06 release
- Fix SHA digest stored as container image, stop/restart timeouts, cron restore on boot, and modal viewport centering in iframe
- Show container actions in kebab menu only for mobile list view
- Mobile responsive overhaul, inline logs polish, and kebab menu improvements
- Add inline logs panel in list view expanded details
- Fix 502 error on container Console and Logs actions
- Add "Clear" button to update check log viewer
- Fix stale update badges after checks find no updates
- Resolve SHA image refs to tags when recreating containers
- Fix false positive update detection after pulling images
- Fix ExposedPorts/Volumes empty object encoding in container recreate
- Surface Docker API errors in recreate flow, add plugin log entries
- Make post-pull operations resilient to prevent stream from dying
- Fix post-pull red X and add auto-recreate container support
- Fix Database::prepare() not existing, use query() instead
- Add PHP tests for checkAllImageUpdates update check logic
- Fix iframe not shrinking on folder collapse, harden update loop
- Fix update check timeout and uneven card button sizing
- Fix update checks only completing for first container
- Fix build script bugs and improve robustness
- Fix folder stats bars, add StatsBar tests, update project docs
- Extract reusable components, refactor backend config and stats
- Fix concurrent container action loading states, add dev/stable release channels
- Add logging to manual update checks, gitignore phpunit cache
- chore: update gitignore
- Add update check logging with viewer in settings
- Fix session check: csrf_token is runtime-only, not in session file
- Fix session validation for Unraid's custom session cookie
- Add Docker-based PHPUnit tests for auth layer
- Fix PUT/DELETE CSRF validation and folder collapse persistence
- Fix form controls using nonexistent --input-background variable
- Fix dropdown text color on dark themes in settings page
- Revamp settings page: dark theme, grouped sections, container exclude modal
- Fix auth: read Unraid's Flask session cookie instead of PHP session
- Fix iframe auth: add credentials to all fetch calls, aggregate changelog by date
- chore: update build script
- Harden API endpoints: enable auth, add input validation, fix injection patterns
- Add container update rework: cron scheduling, batch pulls, folder badges, exclude list
- Remove Plugin Information section from settings page
- Fix list view kebab menu clipped by overflow-hidden
- Unify KebabMenu component, fix responsive overflow, and add tests
- Add view mode slider toggle, folder menu padding, and update mock data
- Polish folder context menu padding and replace view toggle with icon slider
- Fix z-index, hover flicker, action spinner + add hide stopped toggle
- Fix drag-drop duplication, card padding, folder kebab menu, and z-index
- Pass Unraid CSS variables into iframe for dark theme support
- Load app in iframe to isolate from Unraid global CSS
- Add Markdown="false" to DockerFoldersMain.page to fix styles not loading
- Add container action feedback, image update checking, and pull with progress
- Add UI animations: folder collapse, modal transitions, state pulse, card fade-in
- Always show app on Folders tab regardless of replace setting
- Simplify inject page to only collapse native Docker section
- Wrap native Docker section in collapsed accordion instead of hiding
- remove changelog
- Fix Docker section replacement race condition with async rendering
- Include CHANGELOG.md in release commit
- Auto-generate CHANGELOG.md from git history during release builds
- Generate release notes from commits since last tag
- Update docs to reflect container search, live stats, and UI polish
- Make labels and volumes sections horizontally scrollable
- Add container search to filter by name or image
- Fix duplicate #app elements when replace_docker_section is enabled
- Stack health, command, and labels vertically in card view
- Add container details (command, health, labels) to expanded accordion
- Swap volume display order to source -> destination
- Add link icon next to image URLs and volume paths
- Redesign list view row layout
- Gray out folder count badge when no containers are running
- Fix folder associations lost when containers are recreated
- Make entire list row clickable to expand/collapse
- Fix stats, ports, image, and status hidden in iframe
- Hide drag handles when drag & drop is locked
- Update PLG changes section with latest changelog
- Move settings icon to far left of header
- Fix Create Folder button text hidden in iframe
- Fix header layout on desktop and reduce list view expanded margin
- Add collapsible unfoldered containers section
- Add mobile-responsive layout with sm breakpoints
- can't remember hahaa
- Improve dark theme text contrast, modal fixes, and nav layout
- Fix stats polling for faster load and persistent cache
- Add folder-level stats, globe WebUI icon, and text sizing fixes
- Add folder ports, WebUI icon, text sizing, and dark theme fixes
- Add changelog, improve Docker section takeover and settings page
- UI polish: confirm modals, folder UX, edit in kebab menu
- loading states and more details for settings
- various improvements
- add supporting links
- add linkable volumes
- fix spacing and alignment
- fix styling and stats not displaying. unraid is really mucking with styling.
- fix unraid styles taking over
- make composed folders easier to identify
- added better icon and updated plugin icon
- add settings to turn off live
- automatically group composed containers
- fix polling for stats
- more metric improvmenets and other little changes
- add container stats
- update current state
- chore: move to settings page
- add additional docker details and settings
- add edit buttons to containers
- change how drag and drop works, folders take icons from containers
- add list or card view and fix some other bugs
- add dev server and fix a couple bugs
- chore remove iframe
- fix crsf issue
- move to tailwind
- move away from modern naming
- fix sorting and craeting folders
- update text docs
- feat: phase 3 realtime pipeline
- chore: update icon
- fix: settings
- fix: pages
- Add CLAUDE.md for future Claude Code instances
- Add quick start guide for resuming development
- Add project status and current issue documentation
- Fix Docker.page to properly integrate with Unraid UI (no full HTML doc)
- Fix page headers: add Type attribute and use FontAwesome icons
- Change Docker menu title to just 'Folders' for clean URL
- Switch from PDO to SQLite3 for better Unraid compatibility
- Add automatic GitHub release creation to build script
- Fix XML parsing by wrapping INLINE scripts in CDATA sections
- Phase 2: Create folder Vue components
- Phase 2: Implement folder management frontend stores
- Phase 2: Implement folder management backend
- Fix package ownership and remove macOS metadata files
- version updatE
- Add timestamp-based versioning and Settings page
- Fix Vite base path for correct asset loading
- Rename plugin to unraid-docker-folders-modern and rebuild
- rename folder
- Update PLG file with build MD5 checksum
- Fix TypeScript and vue-tsc compatibility issues
- Add PLG installer file for Unraid plugin system
- Add build system for packaging plugin
- Implement database schema and migration system
- Implement backend PHP classes and API
- Set up frontend with Vue 3, TypeScript, and Vite
- Initial project structure for unraid-docker-modern plugin
- refactor(sort): share the folder sort decision and extract sort fields once
- feat(header): show the container and folder counts inside the search field
- feat(settings): group the settings page by what each setting affects
- feat(sort): add a "Sort folders too" toggle to the sort menu
- fix(folders): apply the toolbar sort to folder contents
- build: use content-hashed asset filenames
- fix(folders): do not count removed containers as hidden
- docs: add a contributing guide and require dev as the PR base
- fix(folders): repair the #9 merge and add the sort menu
- Add auto-sort options for folders and folder contents (#9)
- chore: update docs
- refactor: share the paused-start rule and tidy the issue fixes
- feat(updates): add Force Update to the container menu (#11)
- feat(schedules): add a Resume action and let Start resume a paused container (#7)
- fix(docker): resume a paused container from the card and the API (#7)
- fix(schedules): evaluate and show schedule times in the server timezone (#7)
- fix(folders): persist the manual order of unfoldered containers (#12)

## 2026.09.12
- refactor: share the move-to-folder action and the select modal
- feat(updates): name the containers in the update notification
- feat(folders): add a folder picker to the container menu
- fix(compose): rename the Stack Details menu item to Edit Stack
- feat(docker): show the inline log panel in card view

## 2026.08.22
- test(docker): pin the managed-with-autostart-off branch
- fix(docker): correct three faults the browser check found
- feat(docker): put Adopt on the container, not only in the kebab menu
- fix(docker): escape adopted values before they reach Unraid's shell
- feat(docker): adopt CLI-created containers into Unraid's container manager
- fix(ui): keep an open kebab menu inside the frame instead of scrolling
- fix(ui): stop the unfoldered section clipping open kebab menus

## 2026.08.19
- fix(folders): only add/remove containers that changed when saving a folder

## 2026.08.17
- feat(settings): add a "Buy me a coffee" Ko-fi link
- feat(ui): collapse the create buttons into one menu, widen the search
- feat: rename to "Docker Folders" and shorten the page URLs
- feat(ui): one update button, and a re-check inside the confirm modal
- feat(ui): collapse the three create buttons to "+" plus an icon

## 2026.08.16
- fix(ui): render the update-check controls before settings land
- docs: summarize each release in CHANGELOG, stop regenerating it
- chore: drop the beta label from Image Updates settings
- fix(ui): stop compose buttons blinking in while availability is checked
- test: fix session tests broken by PHPUnit output, silence constant warnings
- fix(security): validate every user-influenced filesystem path
- chore: prepare repo for Community Applications submission

## 2026.08.10
The update confirm modal now shows the release notes for each image.

## 2026.07.26
Reworked the container card. The status dot became a halo around the container
icon, the expanded card was restructured, and its click target is now wider.
Added batch image updates: you can review the affected containers before the
pull and update several at once. A container's schedules now appear in its
expanded card. Fixed log reading for TTY containers.

## 2026.07.25
Fixed the schedules modal.

## 2026.07.18
Added a design system (`DESIGN.md`) and moved the UI onto theme tokens. Folders
gained a tint that shows their expanded state, replacing the left-border accent.
Added settings to hide the legacy Docker containers and buttons, and added
update checks that target one container or one compose stack. Releases now run
from GitHub Actions.

## 2026.07.10
Maintenance release.

## 2026.06.06
Fixed cron registration. The plugin now writes to its own config directory.

## 2026.05.30
Added port conflict detection. A stopped container whose ports are already bound
shows a badge, and the expanded card lists the containers it conflicts with.

## 2026.04.22
Fixed update-check cron registration. The Update badge now links to the release
notes for that image.

## 2026.04.12
Added scheduling and backups. You can run container and stack actions on a cron
schedule, and back up container data on the same schedule.

## 2026.04.11
Overhauled the compose editor: a logs tab, a recompose flow, YAML highlighting,
and a save lock. Added compose file version history with rollback. Container
stats now read from cgroups and cache their slow data, which cut load time.

## 2026.04.07
Modals now render in the parent window, so the iframe no longer clips them.
Fixed the compose import banner for users without the compose.manager plugin.

## 2026.03.21
Added a Create Stack button and a per-container autostart toggle. Fixed
autostart so it reads and writes Unraid's flat file rather than only the XML
template. Extracted icons into reusable components and fixed folder counts,
cleanup of deleted containers, and several modal styling problems.

## 2026.03.15
Added Docker Compose management. Fixed a set of iframe problems: modal
clipping, scroll feedback between the modal and the parent page, and z-index.

## 2026.03.06
Maintenance release.

## 2026.02.28
Mobile overhaul. The layout is responsive, container actions move into the kebab
menu on small screens, and list view gained an inline logs panel. Fixed a 502
error on the Console and Logs actions.

## 2026.02.27
Fixed image update accuracy. Update badges no longer go stale after a check
finds nothing, SHA image references resolve to tags when a container is
recreated, and pulling an image no longer causes a false update report.

## 2026.02.25
Containers can now be recreated automatically after a pull. Fixed update checks
that stopped after the first container, and fixed the folder collapse animation
leaving the iframe at the wrong height. Added the first PHP tests.

## 2026.02.24
Hardened the API: authentication is enforced on every endpoint, input is
validated, and CSRF works for PUT and DELETE. Rewrote the settings page with a
dark theme and grouped sections. Added image update checking with cron
scheduling, batch pulls, folder badges, and an exclude list.

## 2026.02.23
Moved the app into an iframe to isolate it from Unraid's global CSS, and passed
Unraid's theme variables in so dark mode works. Unified the kebab menu into one
component, added a card/list view toggle, and fixed drag-and-drop duplication.

## 2026.02.15
The largest release. Added container search, live resource stats, image update
checking with pull progress, and a mobile-responsive layout. Compose containers
group into folders automatically. Expanded cards gained command, health, labels,
and volume details. Folder associations now survive a container being recreated.
The changelog itself became generated from git history.

## 2026.02.14
First working plugin. Set up the Vue 3 frontend, the PHP backend and its API,
the SQLite schema and migrations, and the build system that packages the plugin
and creates the GitHub release. Folder management landed here. Switched from PDO
to SQLite3, which Unraid supports.
