# 0.70.0

* **Flet 1.0 Alpha Released** – [Read the announcement](https://flet.dev/blog/introducing-flet-1-0-alpha)
* **New:** Declarative and reactive programming style, alongside imperative
* **New:** Automatic page updates after event handler completion
* **New:** Service controls for non-visual functionality
* **New:** WebAssembly support for running web apps in the browser
* **New:** Offline mode support for web apps
* **New:** Ability to embed Flet web apps into multiple HTML elements on a page
* **New:** Modern, future-proof architecture:
  * Controls in Python are now defined as plain dataclasses
  * Unified diffing algorithm supports both imperative and declarative styles
  * Refactored Flutter layer using inherited widgets and `Provider`
* See the list of [breaking changes](https://github.com/flet-dev/flet/issues/5238)

# 0.28.3

* Fixed: Local Images Not Rendering in Android App using Flet 0.27.6 ([#5198](https://github.com/flet-dev/flet/issues/5198))
* Fixed: FilePicker.save_file() opens blank gray screen in APK build (works fine in VS) ([#5301](https://github.com/flet-dev/flet/issues/5301))

# 0.28.2

* Fixed missing imports in `__init__.py` ([#5292](https://github.com/flet-dev/flet/pull/5292)).
* Fixed: GestureDetector should have at least one event handler defined ([#5293](https://github.com/flet-dev/flet/pull/5293)).

# 0.28.0

* New Features and Flutter 3.29 ([#4891](https://github.com/flet-dev/flet/issues/4891))
* Fixed: `Dropdown.expand` has no effect ([#5042](https://github.com/flet-dev/flet/pull/5042))
* feat: custom `ReorderableListView` drag handle listeners ([#5051](https://github.com/flet-dev/flet/pull/5051))
* Fixed: `LineChartDataPoint.tooltip` not properly rendered ([#5105](https://github.com/flet-dev/flet/pull/5105))
* Remove Flet v0.25 deprecations ([#5155](https://github.com/flet-dev/flet/pull/5155))
* Prevent platform back button from popping a route with pop confirmation event ([#5280](https://github.com/flet-dev/flet/issues/5280))
* Fixed: SearchBar does not handle capitalization correctly ([#5014](https://github.com/flet-dev/flet/issues/5014))
* Fixed: `FilePicker` upload fails if original filename is modified ([#5037](https://github.com/flet-dev/flet/issues/5037))

# 0.27.6

* Fix `flet build`: allow dependencies with commas ([#5033](https://github.com/flet-dev/flet/issues/5033))
* Show app startup screen by default ([#5036](https://github.com/flet-dev/flet/issues/5036))
* fix: `Textfield` cursor position changes when modifying field content in `on_change` ([#5019](https://github.com/flet-dev/flet/issues/5019))
* Remove deperecated `Control.update_async()` method ([#5005](https://github.com/flet-dev/flet/issues/5005))
* fix: incorrect positioning of non-FAB controls assigned to page.floating_action_button ([#5049](https://github.com/flet-dev/flet/issues/5049))

# 0.27.5

* Added `FletApp.showAppStartupScreen` and `FletApp.appStartupScreenMessage` properties.
* Added `tool.flet.splash.icon_bgcolor` and `tool.flet.splash.icon_dark_bgcolor` settings for Android splash screen icon image.
* Added `tool.flet.app.boot_screen` and `tool.flet.app.startup_screen` settings for customizing Flet app "loading" screens.
* feat: `Dropdown.menu_width` property ([#5007](https://github.com/flet-dev/flet/issues/5007))
* PBKDF2 iteration count increased to 600,000 ([#5023](https://github.com/flet-dev/flet/issues/5023))

# 0.27.4

* Fix: do not remove `flutter-packages` on re-build if `dev_packages` configured.

# 0.27.3

* Fixes to make `flet build` work in CI environment ([#4993](https://github.com/flet-dev/flet/issues/4993))

# 0.27.2

* Error on second flet build run "Because {app} depends on flet_{package} from path which doesn't exist" ([#4955](https://github.com/flet-dev/flet/issues/4955))
* Editable packages in pyproject.toml to install from a path by flet build command ([#4963](https://github.com/flet-dev/flet/issues/4963))
* Setting Android manifest `<application>` element properties in `pyproject.toml` ([#4977](https://github.com/flet-dev/flet/issues/4977))
* Fixed regression: Added back `Control.build()` method.

# 0.27.1

* Fixed: binary file operations should not specify encoding.

# 0.27.0

* `DropdownMenu` control ([#1088](https://github.com/flet-dev/flet/issues/1088))
* feat: `ReorderableListView` Control ([#4865](https://github.com/flet-dev/flet/pull/4865))
* Remove v0.24.0 deprecations [#4932](https://github.com/flet-dev/flet/pull/4932))
* Implement `Container.dark_theme` property ([#4857](https://github.com/flet-dev/flet/issues/4857))
* Upgrade to Pyodide 0.27 for `httpx` Support ([#4840](https://github.com/flet-dev/flet/issues/4840))
* Remove `CupertinoCheckbox.inactive_color` in favor of `fill_color` ([#4837](https://github.com/flet-dev/flet/issues/4837))
* `flet build`: use Provisioning Profile to sign iOS app archive (`.ipa`), deprecate `--team` option ([#4869](https://github.com/flet-dev/flet/issues/4869))
* feat: `flet doctor` CLI command ([#4803](https://github.com/flet-dev/flet/pull/4803))
* feat: implement button themes (for `ElevatedButton`, `OutlinedButton`, `TextButton`, `FilledButton`, `IconButton `) ([#4872](https://github.com/flet-dev/flet/pull/4872))
* `ControlEvent.data` should be of type `Optional[str]` and default to `None` ([#4786](https://github.com/flet-dev/flet/issues/4786))
* `flet build`: add `--source-packages` to allow installing certain Python packages from source distros ([#4762](https://github.com/flet-dev/flet/issues/4762))
* disable markup for flet-cli stdout logs ([#4796](https://github.com/flet-dev/flet/pull/4796))
* Fixed: Disable rich's Markup for stdout logs ([#4795](https://github.com/flet-dev/flet/issues/4795))
* Fixed: Setting `SearchBar.bar_border_side` isn't visually honoured ([#4767](https://github.com/flet-dev/flet/issues/4767))
* Fixed: Dropdown: Long options cause the down-arrow to oveflow ([#4838](https://github.com/flet-dev/flet/issues/4838))
* Fixed: CupertinoSlider initialisation does not allow values less then zero/greater then 1 ([#4853](https://github.com/flet-dev/flet/issues/4853))
* Fixed: Same code shows different appearance in Flet APP/Web/PC local. ([#4855](https://github.com/flet-dev/flet/issues/4855))
* Fixed: Transforming scale renders a grey screen ([#4759](https://github.com/flet-dev/flet/issues/4759))
* Fixed: UnicodeDecodeError when using accented characters in manifest.json ([#4713](https://github.com/flet-dev/flet/issues/4713))
* Fixed: Implement `SearchBar.blur()` to programmatically unfocus the bar ([#4827](https://github.com/flet-dev/flet/issues/4827))

# 0.26.0

* Flutter extensions: `flet_*` packages moved to separate repositories ([#4721](https://github.com/flet-dev/flet/pull/4721))
* Automatic installation of Flutter, JDK and Android SDK ([#4721](https://github.com/flet-dev/flet/pull/4721))
* Migrated to Flutter 3.27.0 ([#4593](https://github.com/flet-dev/flet/pull/4593))
* New control properties, Flutter 3.27 fixes ([#4703](https://github.com/flet-dev/flet/pull/4703))
* Optional on-demand creation of `ListView.controls` ([#3931](https://github.com/flet-dev/flet/issues/3931))
* Reset `InteractiveViewer` tranformations ([#4391](https://github.com/flet-dev/flet/issues/4391))
* Passthrough of mouse events from main window to other applications ([#1438](https://github.com/flet-dev/flet/issues/1438))
* Remove v0.26.0-related deprecations ([#4456](https://github.com/flet-dev/flet/issues/4456))
* Implemented `Window.ignore_mouse_events` ([#4465](https://github.com/flet-dev/flet/pull/4465))
* Adding Google/Android TV platform support ([#4581](https://github.com/flet-dev/flet/pull/4581))
* Remove `Optional[]` from predefined typing `*Value`s ([#4702](https://github.com/flet-dev/flet/pull/4702))
* Throttle `InteractiveViewer` update events ([#4704](https://github.com/flet-dev/flet/pull/4704))
* Fixed: Update project_dependencies.py ([#4459](https://github.com/flet-dev/flet/pull/4459))
* Fixed: `SafeArea` object has no attribute `_SafeArea__minimum` ([#4500](https://github.com/flet-dev/flet/pull/4500))
* Fixed: Tooltip corruption in `Segment` and `BarChartRod` on `update()` ([#4525](https://github.com/flet-dev/flet/pull/4525))
* Fixed: Setting `CheckBox.border_side.stroke_align` to an Enum fails ([#4526](https://github.com/flet-dev/flet/pull/4526))
* Fixed: `ControlState` should be resolved based on user-defined order ([#4556](https://github.com/flet-dev/flet/pull/4556))
* Fixed: broken `Dismissible.dismiss_direction` ([#4557](https://github.com/flet-dev/flet/pull/4557))
* Fixed: Fix Rive not updating ([#4582](https://github.com/flet-dev/flet/pull/4582))
* Fixed: `DatePicker` regression with first and last dates ([#4661](https://github.com/flet-dev/flet/pull/4661))
* `flet build` command: Copy `flutter-packages`, support for platform-specific dependencies ([#4667](https://github.com/flet-dev/flet/pull/4667))
* Fixed: `CupertinoBottomSheet` applies a red color and yellow underline to `Text`  content ([#4673](https://github.com/flet-dev/flet/pull/4673))
* Fixed: setting `ButtonTheme` displays a grey screen ([#4731](https://github.com/flet-dev/flet/pull/4731))
* Fixed: `Textfield` input border color considers user-specified `border_color` property ([#4735](https://github.com/flet-dev/flet/pull/4735))
* Fixed: make `Tooltip.message` a required parameter ([#4736](https://github.com/flet-dev/flet/pull/4736))

# 0.25.2

## Bug fixes

* Fix `flet publish` creates broken website if no `requirements.txt` or `pyproject.toml` found ([#4493](https://github.com/flet-dev/flet/pull/4493)).
* Fix PyInstaller hook to avoid download Flet app bundle on first run ([#4549](https://github.com/flet-dev/flet/pull/4549)).
* Support `git`, `path`, `url` Poetry-style dependencies in `pyproject.toml` ([#4554](https://github.com/flet-dev/flet/pull/4554)).
* Fixed broken `Map.center_on()` and default animations ([#4519](https://github.com/flet-dev/flet/pull/4519)).
* Fixed Tooltip corruption in `Segment` and `BarChartRod` on `update()` ([#4525](https://github.com/flet-dev/flet/pull/4525)).
* Fixed Setting `CheckBox.border_side.stroke_align` to an Enum fails ([#4526](https://github.com/flet-dev/flet/pull/4526)).
* Fixed `ControlState should` be resolved based on user-defined order ([#4556](https://github.com/flet-dev/flet/pull/4556)).
* Fixed broken `Dismissible.dismiss_direction` ([#4557](https://github.com/flet-dev/flet/pull/4557)).

# 0.25.1

## Changes

* Added InteractiveViewer programmatic transformations ([#4451](https://github.com/flet-dev/flet/pull/4451)).

## Bug fixes

* Fixed `flet build` creates bundle but running it gives `ImportError: No module named main` error ([#4444](https://github.com/flet-dev/flet/pull/4444)).
* Fixed hook-flet with wrong import module ([#4447](https://github.com/flet-dev/flet/pull/4447)).
* Fixed "flutter/runtime/dart_vm_initializer.cc" error on Linux ([#4443](https://github.com/flet-dev/flet/pull/4443)).

# 0.25.0

## New controls

* Mobile Ads (`Banner` and `Interstitial`) ([details and example](https://github.com/flet-dev/flet/pull/3288)).
* `Button` control ([#4265](https://github.com/flet-dev/flet/pull/4265)) - which is just an alias for `ElevatedButton` control.

## Breaking changes

* Refactor `Badge` Control to a Dataclass; added new `badge` property to all controls ([#4077](https://github.com/flet-dev/flet/pull/4077)).

## Other changes

* Added `{value_length}`, `{max_length}`, and `{symbols_left}` placeholders to `TextField.counter_text` ([#4403](https://github.com/flet-dev/flet/pull/4403)).
* Added `--skip-flutter-doctor` to build cli command ([#4388](https://github.com/flet-dev/flet/pull/4388)).
* `WebView` enhancements ([#4018](https://github.com/flet-dev/flet/pull/4018)).
* `Map` control enhancements ([#3994](https://github.com/flet-dev/flet/pull/3994)).
* Exposed more `Theme` props ([#4278](https://github.com/flet-dev/flet/pull/4278), [#4278](https://github.com/flet-dev/flet/pull/4278)).
* Exposed more properties in multiple Controls ([#4105](https://github.com/flet-dev/flet/pull/4105))
* Added `__contains__` methods in container-alike Controls ([#4374](https://github.com/flet-dev/flet/pull/4374)).
* Added a custom `Markdown` code theme ([#4343](https://github.com/flet-dev/flet/pull/4343)).
* Added `barrier_color` prop to dialogs ([#4236](https://github.com/flet-dev/flet/pull/4236)).
* Merged `icon` and `icon_content` props into `icon: str | Control` ([#4305](https://github.com/flet-dev/flet/pull/4305)).
* Migrated `colors` and `icons` variables to Enums ([#4180](https://github.com/flet-dev/flet/pull/4180)).
* TextField: `suffix_icon`, `prefix_icon` and `icon` can be `Control` or `str` ([#4173](https://github.com/flet-dev/flet/pull/4173)).
* Added `--pyinstaller-build-args` to `flet pack` CLI command ([#4187](https://github.com/flet-dev/flet/pull/4187)).
* Made SearchBar's view height adjustable; added new properties ([#4039](https://github.com/flet-dev/flet/pull/4039)).
* Bumped Rive version and fixed Linux app build template for `rive_common`.

## Bug fixes

* Fixed `Icon` rotation ([#4384](https://github.com/flet-dev/flet/pull/4384)).
* Fixed regression in `Markdown.code_theme` when using `MarkdownCodeTheme` enum ([#4373](https://github.com/flet-dev/flet/pull/4373)).
* Fixed `Segment` and `NavigationBarDestination` accept only string tooltips ([#4326](https://github.com/flet-dev/flet/pull/4326)).
* Display informative message when `date` has wrong format ([#4019](https://github.com/flet-dev/flet/pull/4019)).
* Fixed `MapConfiguration.interaction_configuration` is not honoured ([#3976](https://github.com/flet-dev/flet/pull/3976)).
* Fixed `Video.jump_to()` fails with negative indexes ([#4294](https://github.com/flet-dev/flet/pull/4294)).
* Fixed condition in `AppBar.tooltip_opacity` ([#4280](https://github.com/flet-dev/flet/pull/4280)).
* Fixed wrong type (asyncio.Future -> concurrent.futures.Future) and handle `CancelledError` ([#4268](https://github.com/flet-dev/flet/pull/4268)).
* Fixed clicking on `CupertinoContextMenuAction` doesn't close context menu ([#3948](https://github.com/flet-dev/flet/pull/3948)).
* Fixed dropdown `max_menu_height` ([#3974](https://github.com/flet-dev/flet/pull/3974)).
* Fixed prevent button style from being modified in `before_update()` ([#4181](https://github.com/flet-dev/flet/pull/4181)).
* Fixed disabling filled buttons is not visually respected ([#4090](https://github.com/flet-dev/flet/pull/4090)).
* when `label` is set, use `MainAxisSize.min` for the `Row` ([#3998](https://github.com/flet-dev/flet/pull/3998)).
* Fixed `NavigationBarDestination.disabled` has no visual effect ([#4073](https://github.com/flet-dev/flet/pull/4073)).
* Fixed autofill in `CupertinoTextField` ([#4103](https://github.com/flet-dev/flet/pull/4103)).
* Linechart: `jsonDecode` tooltip before displaying ([#4069](https://github.com/flet-dev/flet/pull/4069)).
* Fixed button's `bgcolor`, `color` and `elevation` ([#4126](https://github.com/flet-dev/flet/pull/4126)).
* Fixed scrolling issues on Windows ([#4145](https://github.com/flet-dev/flet/pull/4145)).
* Skip running flutter doctor on windows if `no_rich_output` is `True` ([#4108](https://github.com/flet-dev/flet/pull/4108)).
* Fixed `TextField` freezes on Linux Mint #4422](https://github.com/flet-dev/flet/pull/4422)).

# 0.24.1

* FIXED: `Tooltip` displays wrong message when used with `IconButton`, `FloatingActionButton` and `PopupMenuButton` ([#3922](https://github.com/flet-dev/flet/issues/3922))
* FIXED: `Image.src.base64` ([#3919](https://github.com/flet-dev/flet/issues/3919))

# 0.24.0

* NEW: `Placeholder` Control ([#3646](https://github.com/flet-dev/flet/issues/3646))
* NEW: `InteractiveViewer` Control ([#3645](https://github.com/flet-dev/flet/issues/3645))
* NEW: Adding Background/Foreground Services to GeoLocator UPDATE ([#3803](https://github.com/flet-dev/flet/issues/3803))
* NEW: `Container.ignore_interactions` property ([#3639](https://github.com/flet-dev/flet/issues/3639))
* NEW: Add `rtl` prop to more controls ([#3641](https://github.com/flet-dev/flet/issues/3641))
* NEW: `TextField.counter` property ([#3676](https://github.com/flet-dev/flet/issues/3676))
* NEW: window.icon: make the usage of relative paths possible ([#3825](https://github.com/flet-dev/flet/issues/3825))
* NEW: Add event to `flet_video` to know what song is playing ([#3772](https://github.com/flet-dev/flet/issues/3772))
* NEW: adds `floating_action_button_theme` property to `Theme` ([#3771](https://github.com/flet-dev/flet/issues/3771))
* NEW: Added `on_completed` event to `flet_video` ([#3758](https://github.com/flet-dev/flet/issues/3758))
* NEW: Add `focus`, `on_focus`, `on_blur` to `SearchBar` ([#3417](https://github.com/flet-dev/flet/issues/3417), [#3752](https://github.com/flet-dev/flet/issues/3752))
* NEW: `--no-rich-output` flag to prevent rich output ([#3708](https://github.com/flet-dev/flet/issues/3708))
* CHANGED: make `Tooltip` a dataclass which can be used in `Control.tooltip` ([#3837](https://github.com/flet-dev/flet/issues/3837))
* CHANGED: wrap `View`s into a background container ([#3820](https://github.com/flet-dev/flet/issues/3820))
* FIXED: export BottomSheetTheme ([#3858](https://github.com/flet-dev/flet/issues/3858))
* FIXED: setting SearchBar.value to an empty string is not respected ([#3872](https://github.com/flet-dev/flet/issues/3872))
* FIXED: add full-screen events to WindowEventType ([#3857](https://github.com/flet-dev/flet/issues/3857))
* FIXED: snackbar margin ([#3856](https://github.com/flet-dev/flet/issues/3856))
* FIXED: not error on inputfield when errorText is empty ([#3855](https://github.com/flet-dev/flet/issues/3855))
* FIXED: `flet.map` is not available after building app ([#3845](https://github.com/flet-dev/flet/issues/3845))
* FIXED: `InputFilter` clears `TextField` when an invalid character is entered ([#3779](https://github.com/flet-dev/flet/issues/3779))
* FIXED: `Dropdown.alignment` not respected ([#3737](https://github.com/flet-dev/flet/issues/3737))
* FIXED: scrolling issues in `CupertinoPicker` ([#3678](https://github.com/flet-dev/flet/issues/3678))
* FIXED: scrolling controls are not able to scroll due to wrong super class call ([#3702](https://github.com/flet-dev/flet/issues/3702))
* FIXED: Dismissible ([#3690](https://github.com/flet-dev/flet/issues/3690))
* FIXED: `PieChartEvent.type` on web ([#3611](https://github.com/flet-dev/flet/issues/3611))
* FIXED: `Switch.width` and `height` properties ([#3670](https://github.com/flet-dev/flet/issues/3670))
* FIXED: parsing issues in `TextStyle` and `*Event` classes ([#3551](https://github.com/flet-dev/flet/issues/3551))
* FIXED: issues with `*Button`s ([#3582](https://github.com/flet-dev/flet/issues/3582))
* Handle Multiple Trailing Controls in `CupertinoAppBar` ([#3603](https://github.com/flet-dev/flet/issues/3603))
* Event: implement str and repr magic methods ([#3601](https://github.com/flet-dev/flet/issues/3601))
* CHORE: remove handler-subscription and enhance event typing ([#3808](https://github.com/flet-dev/flet/issues/3808))
* CHORE: improve type hint for OptionalEventCallable ([#3659](https://github.com/flet-dev/flet/issues/3659))
* CHORE: Using `Sequence` instead of `list` ([#3661](https://github.com/flet-dev/flet/issues/3661))
* CHORE: Bump Flutter packages ([#3719](https://github.com/flet-dev/flet/issues/3719))
* CHORE: Cleanup ([#3640](https://github.com/flet-dev/flet/issues/3640))

# 0.23.2

* CHANGED: Enhance Typing of Event Handlers ([#3523](https://github.com/flet-dev/flet/issues/3523))
* CHANGED: Delete Page.window.on_resize | deprecate Page.on_resize in favor of Page.on_resized ([#3516](https://github.com/flet-dev/flet/issues/3516))
* CHANGED: View is not opened on tap ([#3513](https://github.com/flet-dev/flet/issues/3513))
* FIXED: `Slider.value` defaults to `min` ([#3503](https://github.com/flet-dev/flet/issues/3503))
* FIXED: add "hide" and "show" to WindowEventType enum ([#3505](https://github.com/flet-dev/flet/issues/3505))
* FIXED: TypeError raised for isinstance check with Union in before_update method ([#3499](https://github.com/flet-dev/flet/issues/3499))
* FIXED: Corrected `isinstance` check in `SnackBar.before_update` to use a tuple of types instead of Union, resolving TypeError: "Subscripted generics cannot be used with class and instance checks".
* FIXED: `Page.open()` breaking after multiple calls.
* FIXED: Typo in on_resized setter decorator

# 0.23.1

* FIX: Fix parseFloatingActionButtonLocation() to work on desktop ([#3496](https://github.com/flet-dev/flet/issues/3496))
* FIX: Flet 0.23 crashes on Ubuntu 22.04 ([#3495](https://github.com/flet-dev/flet/issues/3495))
* FIX: View.floating_action_button_location: conditionally use _set_attr.
* FIX: Import `ParamSpec` from `typing` for Python >3.10.
* FIX: replace `len(list(filter(...)))` by `any(...)`.
* FIX: Make window and browser_context_menu private, and expose respective getters.

# 0.23.0

* NEW: `PermissionHandler` control ([#3276](https://github.com/flet-dev/flet/issues/3276))
* NEW: `Map` control ([#3093](https://github.com/flet-dev/flet/issues/3093))
* NEW: `Geolocator control` ([#3179](https://github.com/flet-dev/flet/issues/3179))
* NEW: `AutoFillGroup` Control ([#3047](https://github.com/flet-dev/flet/issues/3047))
* NEW: Migrated to Flutter 3.22 ([#3396](https://github.com/flet-dev/flet/issues/3396))
* NEW: An ability to access PubSubHub from outside Flet app ([#3446](https://github.com/flet-dev/flet/issues/3446))
* NEW: `TextStyle` props: `overflow`, `word_spacing`, `baseline` ([#3435](https://github.com/flet-dev/flet/issues/3435))
* NEW: Enable/disable browser context menu ([#3434](https://github.com/flet-dev/flet/issues/3434))
* NEW: `Container.color_filter` property ([#3392](https://github.com/flet-dev/flet/issues/3392))
* NEW: `dropdown.Option.text_style` property ([#3293](https://github.com/flet-dev/flet/issues/3293))
* NEW: `dropdown.Option.content` property ([#3456](https://github.com/flet-dev/flet/issues/3456))
* NEW: `Video.configuration` property ([#3074](https://github.com/flet-dev/flet/issues/3074))
* NEW: Enable Impeller on Android and macOS ([#3458](https://github.com/flet-dev/flet/issues/3458))
* NEW: AutoComplete: add selected_index read-only property ([#3298](https://github.com/flet-dev/flet/issues/3298))
* NEW: Renamed `NavigationDestination` to `NavigationBarDestination` ([#3172](https://github.com/flet-dev/flet/issues/3172))
* CHANGED: Prettify "build" command cli output ([#3407](https://github.com/flet-dev/flet/issues/3407))
* CHANGED: Set colorScheme.primary as defaultSideColor ([#3421](https://github.com/flet-dev/flet/issues/3421))
* CHANGED: feat(map): add missing py-events, better typing ([#3464](https://github.com/flet-dev/flet/issues/3464))
* CHORE: Refactor `numbers.dart` utils ([#3263](https://github.com/flet-dev/flet/issues/3263))
* CHORE: Global Code Refactoring/Clean-up ([#3186](https://github.com/flet-dev/flet/issues/3186))
* CHORE: Cleanup ([#3406](https://github.com/flet-dev/flet/issues/3406))
* CHORE: Error handling enhancements ([#3175](https://github.com/flet-dev/flet/issues/3175))
* CHORE: Improve type hint for run_task and run_thread ([#3459](https://github.com/flet-dev/flet/issues/3459))
* CHORE: Move `page.window_*` and `page.browser_context_menu_*` properties to `Window` and `BrowserContextMenu` classes ([#3463](https://github.com/flet-dev/flet/issues/3463))
* FIX: `Container.on_tap_down` not called when `on_click` is not provided ([#3442](https://github.com/flet-dev/flet/issues/3442))
* FIX: SnackBar bug #3311 ([#3313](https://github.com/flet-dev/flet/issues/3313))

# 0.22.1

* `AutoComplete` control ([#3003](https://github.com/flet-dev/flet/issues/3003))
* Added `--exclude` option to `flet build` command ([#3125](https://github.com/flet-dev/flet/issues/3125))
* `CupertinoTimePicker.alignment` property ([#3036](https://github.com/flet-dev/flet/issues/3036))
* Bump `file_picker` dependency to 8.0.3.
* Fix latest flet-build-template version in development mode ([#3021](https://github.com/flet-dev/flet/issues/3021))
* Fix `flet --version` command for source checkout.
* LineChart: fix regression ([#3033](https://github.com/flet-dev/flet/issues/3033))
* Fixed: OAuth expiry of token will hang fastapi server ([#3150](https://github.com/flet-dev/flet/issues/3150))
* Fixed: Disabled the dropwown, but the color isnot gray ([#2989](https://github.com/flet-dev/flet/issues/2989))
* Fixed: `pubspec.yaml` for adding custom Flutter packages requires `dependency_overrides` ([#3187](https://github.com/flet-dev/flet/issues/3187))
* Fixed `disabled` dropdown ([#3183](https://github.com/flet-dev/flet/issues/3183))
* Fixed default value for scrollbar thickness ([#3147](https://github.com/flet-dev/flet/issues/3147))
* Fixed: autoreload, restrict eventhandler from restart on open ([#3098](https://github.com/flet-dev/flet/issues/3098))
* Fixed ([#3035](https://github.com/flet-dev/flet/issues/3035)) switch Flutter RichText to Text.rich ([#3066](https://github.com/flet-dev/flet/issues/3066))
* Fixed: Markdown code block is not selectable ([#1753](https://github.com/flet-dev/flet/issues/1753))

# 0.22.0

* Controls enhancement (see [#2882](https://github.com/flet-dev/flet/issues/2882) for details).
* `Theme` Enhancement ([#2955](https://github.com/flet-dev/flet/issues/2955)).
* `Rive` Control ([#2841](https://github.com/flet-dev/flet/issues/2841)).
* `Control.parent` property ([#2906](https://github.com/flet-dev/flet/issues/2906)).
* `Container.on_tap_down` event.
* Add `upload_endpoint_path` into `flet.fastapi.app` ([#2954](https://github.com/flet-dev/flet/issues/2954)).
* Add checkbox border side state ([#2973](https://github.com/flet-dev/flet/issues/2973)).
* Global context for session ([#2934](https://github.com/flet-dev/flet/issues/2934)).
* Fix silent error in `page.run_task` ([#2959](https://github.com/flet-dev/flet/issues/2959)).
* Web: patch html title with app_name ([#2909](https://github.com/flet-dev/flet/issues/2909)).
* `Container`: fix triggered both `on_click` and `on_long_press` events ([#2914](https://github.com/flet-dev/flet/issues/2914)).

# 0.21.2

* Fix for mobile Safari: Store session ID in SessionStorage instead of window.name.
* Bugfixing on Python side.

# 0.21.1

* Bugfixing.

# 0.21.0

* FastAPI instead of built-in Fletd server. Mixed async/sync apps. ([#2700](https://github.com/flet-dev/flet/issues/2700)).
* `CupertinoActivityIndicator` Control ([#2762](https://github.com/flet-dev/flet/issues/2762)).
* `Lottie`Control and `Video` v2 ([#2673](https://github.com/flet-dev/flet/issues/2673)).
* `CupertinoActionSheet` and `CupertinoActionSheetAction` controls ([#2763](https://github.com/flet-dev/flet/issues/2763)).
* `CupertinoSlidingSegmentedButton` and `CupertinoSegmentedButton` controls ([#2767](https://github.com/flet-dev/flet/issues/2767)).
* `CupertinoTimerPicker` and `CupertinorPicker` Controls ([#2743](https://github.com/flet-dev/flet/issues/2743)).
* `CupertinoContextMenu` and `CupertinoContextMenuAction` controls ([#2772](https://github.com/flet-dev/flet/issues/2772)).
* `CupertinoDatePicker` Control ([#2795](https://github.com/flet-dev/flet/issues/2795)).
* `Page.on_app_lifecycle_state_change` event ([#2800](https://github.com/flet-dev/flet/issues/2800)).
* More `Semantics` properties and `SemanticsService` control ([#2731](https://github.com/flet-dev/flet/issues/2731)).
* Fix container.dart for issue #2628 ([#2701](https://github.com/flet-dev/flet/issues/2701)).(#2701)
* Adaptive fixes ([#2720](https://github.com/flet-dev/flet/issues/2720)).
* `label_style` property for `Checkbox`, `Switch`, and `Radio` ([#2730](https://github.com/flet-dev/flet/issues/2730)).
* Additional properties ([#2736](https://github.com/flet-dev/flet/issues/2736)).
* Reorder `__init__` ([#2724](https://github.com/flet-dev/flet/issues/2724)).

# 0.20.2
* Move `system_overlay_style` from `AppBar` to `Theme` ([#2667](https://github.com/flet-dev/flet/issues/2667)).
* `flet build` command checks minimal Flutter SDK version.
* Buttons turn to `CupertinoDialogAction` controls inside adaptive dialogs.
* `FletApp` control takes control create factories from a parent app.

# 0.20.1

* Migrated to Flutter 3.19
* Fixed scrolling behavior changes in scrollable controls.
* Remove `Page.design` and replace with `Page.adaptive` ([#2650](https://github.com/flet-dev/flet/issues/2650)).
* Rename `Control.on_update` to `Control.before_update` ([#2642](https://github.com/flet-dev/flet/issues/2642)).

# 0.20.0

* `AppBar.system_overlay_style` property ([#2615](https://github.com/flet-dev/flet/issues/2615)).
* New `CupertinoButton` props: `filled`, `style.bgcolor`, `style.padding`, `text`, `icon`, `icon_color`.
* Added `NavigationBar.border` property which is used in adaptive mode only.
* `Page.design` and `Pagelet.design` properties to force Material, Cupertino or Adaptive design language on entire app ([#2607](https://github.com/flet-dev/flet/issues/2607)).
* `Page.media` property with the data about obstructed spaces on the device ([#2613](https://github.com/flet-dev/flet/issues/2613)).
* Adaptive buttons ([#2591](https://github.com/flet-dev/flet/issues/2591)).
* `Control.on_update()` method for better custom controls.
* `--include-packages` option and support for `pubspec.yaml` for custom Flutter packages plus API for adding custom Flutter packages.
* Add `rtl` property to multiple controls ([#2582](https://github.com/flet-dev/flet/issues/2582)).
* Fix: Material icon is shown instead of Cupertino icon if its name is thesame ([#2581](https://github.com/flet-dev/flet/issues/2581)).
* `TextStyle.letter_spacing`property ([#2574](https://github.com/flet-dev/flet/issues/2574)).
* `Audio`, `AudioRecorder`, `Video` and `WebView` controls moved into separate Flutter packages ([#2579](https://github.com/flet-dev/flet/issues/2579)).
* Introduced `Control.on_update()` overridable method ([#2578](https://github.com/flet-dev/flet/issues/2578)).
* New `AlertDialog` properties: `icon`, `bgcolor`, `elevation`.
* `expand_loose` property for Control and all controls that have `expand` property ([#2561](https://github.com/flet-dev/flet/issues/2561)).
* Pyodide v0.25.0.
* `flet create` command to show verbose output ([#2544](https://github.com/flet-dev/flet/issues/2544)).
* `AudioRecorder` control ([#2494](https://github.com/flet-dev/flet/issues/2494)).
* Bugfix: `flet pack --distpath` deletes `dist` directory ([#2500](https://github.com/flet-dev/flet/issues/2500)).
* Added recursive `adaptive` property to all container-alike controls.
* `TextField.text_vertical_align` property ([#2496](https://github.com/flet-dev/flet/issues/2496)).
* `CupertinoButton` Control ([#2495](https://github.com/flet-dev/flet/issues/2495)).
* `CupertinoListTile` control ([#2487](https://github.com/flet-dev/flet/issues/2487)).
* Support for custom Flutter controls ([#2482](https://github.com/flet-dev/flet/issues/2482)).
* `Pagelet` control ([#2469](https://github.com/flet-dev/flet/issues/2469)).
* Add `AppBar.adaptive` ([#2458](https://github.com/flet-dev/flet/issues/2458)).
* Cupertino Icons and Colors ([#2433](https://github.com/flet-dev/flet/issues/2433)).
* `CupertinoTextfield` control ([#2417](https://github.com/flet-dev/flet/issues/2417)).
* `FloatingActionButtonLocation` offset ([#2411](https://github.com/flet-dev/flet/issues/2411)).

# 0.19.0

* `flet build` to apply Python SSL fix when packaging for iOS and Android ([#2349](https://github.com/flet-dev/flet/issues/2349)).
* Upgrade Android Gradle in flet `build app` template ([#2350](https://github.com/flet-dev/flet/issues/2350)).
* `flet build -vv` should run pip install with verbose output ([#2351](https://github.com/flet-dev/flet/issues/2351)).
* Add Python output/logging to troubleshoot empty screens on startup of built app ([#2352](https://github.com/flet-dev/flet/issues/2352)).
* `flet build` should raise an error when trying to package an app with native modules for iOS or Android ([#2356](https://github.com/flet-dev/flet/issues/2356)).
* `flet build` to add timestamp (hash) asset with Flet Python app to re-extract when code changes ([#2289](https://github.com/flet-dev/flet/issues/2289)).
* Handle/bypass `if __name__ == "__main__"` check on Android.
* Support reading dependencies from `pyproject.toml`.
* `flet build` to fix `--base-url` with surrounding slashes ([#2369](https://github.com/flet-dev/flet/issues/2369)).
* `CupertinoAlertDialog`, `CupertinoDialogAction`, adaptive property for `AlertDialog` ([#2365](https://github.com/flet-dev/flet/issues/2365)).
* `Dismissible.confirmDismiss` prop ([#2359](https://github.com/flet-dev/flet/issues/2359)).
* `ListView.reverse` and `GridView.reverse` props ([#2335](https://github.com/flet-dev/flet/issues/2335)).
* `Text.style` type Deprecation warning ([#2286](https://github.com/flet-dev/flet/issues/2286)).
* Add `LineChartData.prevent_curve_over_shooting` and `LineChartData.prevent_curve_over_shooting_threshold` props ([#2354](https://github.com/flet-dev/flet/issues/2354)).
* `flet build` to add checks to allow certain build commands according to "build_on" platform ([#2343](https://github.com/flet-dev/flet/issues/2343)).
* Fixed: `flet build` gives "OSError: [WinError 193] %1 is not a valid Win32 application" for some users ([#2318](https://github.com/flet-dev/flet/issues/2318)).
* Fixed: PubSub is not shared between pages in the same FastAPI app ([#2368](https://github.com/flet-dev/flet/issues/2368)).
* Fixed: check for `DISPLAY` instead of `XDG_CURRENT_DESKTOP` to check if linux machine is GUIless or not ([#2373](https://github.com/flet-dev/flet/issues/2373)).

# 0.18.0

* `flet build` command to package Flet app for any platform ([docs](https://flet.dev/docs/guides/python/packaging-app-for-distribution)).
* Added TextStyle for the Text control ([#2270](https://github.com/flet-dev/flet/issues/2270)).
* Refactor code, add Enum deprecation utils ([#2259](https://github.com/flet-dev/flet/issues/2259)).
* `CupertinoAppBar` control ([#2278](https://github.com/flet-dev/flet/issues/2278)).
* Fix AlertDialog content updating ([#2277](https://github.com/flet-dev/flet/issues/2277)).
* Fix FLET_VIEW_PATH ignored on linux ([#2244](https://github.com/flet-dev/flet/issues/2244)).
* `MenuBar`, `SubMenuButton` and `MenuItemButton` controls ([#2252](https://github.com/flet-dev/flet/issues/2252)).
* convert 'key' to a super parameter ([#2258](https://github.com/flet-dev/flet/issues/2258)).

# 0.17.0

* `SearchBar` control ([#2212](https://github.com/flet-dev/flet/issues/2212)).
* `CupertinoNavigationBar` control ([#2241](https://github.com/flet-dev/flet/issues/2241)).

# 0.16.0

* `CupertinoSlider` control and `Slider.adaptive` ([#2224](https://github.com/flet-dev/flet/issues/2224)).
* `CupertinoRadio` control and `Radio.adaptive` ([#2225](https://github.com/flet-dev/flet/issues/2225)).
* Fix `NavigationBar.label_bahavior` ([#2229](https://github.com/flet-dev/flet/issues/2229)).
* `CupertinoSwitch` control ([docs](https://flet.dev/docs/controls/cupertinoswitch)).
* Disable fade-in effect on Flet app start.
* Tab alignment bug fix ([#2208](https://github.com/flet-dev/flet/issues/2208)).
* Tab visibility ([#2213](https://github.com/flet-dev/flet/issues/2213)).
* Dark window title for Windows ([#2204](https://github.com/flet-dev/flet/issues/2204)).
* Fix `ValueError` on web page resize ([#1564](https://github.com/flet-dev/flet/issues/1564)).

# 0.15.0

* `ExpansionPanel` and `ExpansionPanelList` controls ([docs](https://flet.dev/docs/controls/expansionpanel)).
* `CupertinoCheckBox` control, adaptive `CheckBox` ([docs](https://flet.dev/docs/controls/cupertinocheckbox)).
* Additional control props ([#2182](https://github.com/flet-dev/flet/issues/2182)):
  * `Card.shape`.
  * `NavigationDestination.tooltip`.
  * `NavigationRail`: `elevation`, `indicator_color`, `indicator_shape`.
  * `BottomSheet`: `bgcolor`, `elevation`.
* Added `Dropdown.Option.visible` property.
* Fix AlertDialog broken content when testing in Flet app ([#2192](https://github.com/flet-dev/flet/issues/2192)).

# 0.14.0

* `SelectionArea` control ([docs](https://flet.dev/docs/controls/selectionarea)).
* `SegmentedButton` control ([docs](https://flet.dev/docs/controls/segmentedbutton)).
* `ExpansionTile` control ([docs](https://flet.dev/docs/controls/expansiontile)).
* `BottomAppBar` control ([docs](https://flet.dev/docs/controls/bottomappbar)).
* Add console as a build argument ([#2146](https://github.com/flet-dev/flet/issues/2146)).
* `--uac-admin` flag added to `flet pack` command ([#2149](https://github.com/flet-dev/flet/issues/2149)).
* Bump Flutter dependencies.

# 0.13.0

* `Dismissible` Control ([#2124](https://github.com/flet-dev/flet/issues/2124)).
* `TimePicker` control ([#2129](https://github.com/flet-dev/flet/issues/2129)).
* Fixed: verify `value` limits ([#2121](https://github.com/flet-dev/flet/issues/2121)).
* Added `thumb_icon` to `Switch` ([#2116](https://github.com/flet-dev/flet/issues/2116)).
* Feature: `TextField` Input validation ([#2101](https://github.com/flet-dev/flet/issues/2101)).

# 0.12.2

* Flutter 3.16.0
* Added ´__repr__´ to `Control` class ([#2091](https://github.com/flet-dev/flet/issues/2091)).
* Added ´skip_route_change_event´ to ´page.go_async´ ([#2092](https://github.com/flet-dev/flet/issues/2092)).

# 0.12.1

* Ability to expand `ButtomSheet` to the top of the screen with `BottomSheet.is_scroll_controlled` property ([#2087](https://github.com/flet-dev/flet/issues/2087)).
* `BottomSheet.maintain_bottom_view_insets_padding` to avoid obstructing controls with on-screen keyboard ([#2010](https://github.com/flet-dev/flet/issues/2010)).
* Fixed: `NavigationDrawer` disappears when you move the window and is not opening again ([#2062](https://github.com/flet-dev/flet/issues/2062)).
* Fixed: alert dialog doesn't close ([#2011](https://github.com/flet-dev/flet/issues/2011)).
* Fixed: Resizing app's window with an opened BottomSheet triggers new addition to Overlay ([#2075](https://github.com/flet-dev/flet/issues/2075)).
* Fixed: on_window_event isnt handled after page navigation ([#2081](https://github.com/flet-dev/flet/issues/2081)).
* Fixed: Routing is not working in 0.12.0 ([#2082](https://github.com/flet-dev/flet/issues/2082)).
* Fixed: routing regression.
* Fixed: Multiple dialogs (AlertDialog) will create a ghost dialog ([#1670](https://github.com/flet-dev/flet/issues/1670)).

# 0.12.0

* `NavigationDrawer` control ([docs](https://flet.dev/docs/controls/navigationdrawer)).
* `Badge` control ([docs](https://flet.dev/docs/controls/badge)).
* `RangeSlider` control ([docs](https://flet.dev/docs/controls/rangeslider)).
* `WebView` control ([docs](https://flet.dev/docs/controls/webview)).
* `Cookiecutter` replaces `Copier` ([#2014](https://github.com/flet-dev/flet/issues/2014)).
* `page.go()`: ability to skip route change event ([#2039](https://github.com/flet-dev/flet/issues/2039)).
* Fixed: Two `Datepicker` Opening Issue ([#2025](https://github.com/flet-dev/flet/issues/2025)).
* Fixed: Using Audio and FilePicker at the same time, when click on the FilePicker, the audio automatically replays ([#1807](https://github.com/flet-dev/flet/issues/1807)).
* Fixed: Audio issue while Route Changing ([#1236](https://github.com/flet-dev/flet/issues/1236)).
* Fixed: Snackbar cause Audio stop playing ([#1772](https://github.com/flet-dev/flet/issues/1772)).
* Fixed: `scroll_to()` with zero duration does nothing ([#1659](https://github.com/flet-dev/flet/issues/1659)).
* Fixed: cannot get height and width for page ([#1960](https://github.com/flet-dev/flet/issues/1960)).
* Fixed: Put it the right version of flet ([#1997](https://github.com/flet-dev/flet/issues/1997)).
* Fixed: `Chip.selected` property type changed to bool ([#2048](https://github.com/flet-dev/flet/issues/2048)).
* Fixed: Unreliable detection of SVG images ([#2053](https://github.com/flet-dev/flet/issues/2053)).

# 0.11.0

* `DatePicker` control ([docs](https://flet.dev/docs/controls/datepicker)).
* `Chip` control ([docs](https://flet.dev/docs/controls/chip)).
* Pyodide v0.24.1.
* Python 3.12 support.
* Added `AlertDialog.inset_padding` property ([#1899](https://github.com/flet-dev/flet/issues/1899).
* Embedded mode to work with [`serious_python`](https://pub.dev/packages/serious_python).

# 0.10.3

* Add proxy_path parameter to flet_fastapi.app() ([#1882](https://github.com/flet-dev/flet/issues/1882)).
* Fix `flet create` crashes with an empty project name.

## 0.10.2

* Wrapped --codesign-identity & --add-binary for flet pack ([#1789](https://github.com/flet-dev/flet/issues/1789)).
* Fix incomplete code blocks in `flet_core/page.py`.
* Fix disabled color of FilledButtons.
* Add `AppView` and `WebRenderer` enums to flet-pyodide.
* Pyodide v0.24.0.

## 0.10.1

* Fix Cavas.Text drawing ([#1783](https://github.com/flet-dev/flet/issues/1783))
* Use alternative method to determine user computer's IP ([#1733](https://github.com/flet-dev/flet/issues/1733))

## 0.10.0

* Hosting Flet web apps in FastAPI ([docs](https://github.com/flet-dev/flet/blob/main/sdk/python/packages/flet-fastapi/README.md)).
* Migrated to Flutter 3.13.1.
* Pydantic 2.0 support (Copier upgraded to 8.2.0).
* BREAKING: `DataTable.data_row_height` replaced with `DataTable.data_row_min_height` and `DataTable.data_row_max_height`.

## 0.9.0

* Added `--android` option to `flet run` command.
* Added `page.debug` property ([#1649](https://github.com/flet-dev/flet/issues/1649))
* Added `page.platform_brightness` property and `page.platform_brightness_change` event ([#1630](https://github.com/flet-dev/flet/issues/1630))
* Store session ID in `html.window.name` ([#1629](https://github.com/flet-dev/flet/issues/1629))
* Do not assign random port on Windows with `--ios` flag ([#1620](https://github.com/flet-dev/flet/issues/1620))

## 0.8.4

* Bumping version as PyPi was out of space.

## 0.8.3

* Fixed: FilePicker crash the flet.app() after open directory dialog and choose one directory ([#1572](https://github.com/flet-dev/flet/issues/1572))

## 0.8.2

* Fix `flet pack` command on macOS ([#1580](https://github.com/flet-dev/flet/issues/1580)).
* Fixed: Assets dir and manifest does not work ([#1573](https://github.com/flet-dev/flet/issues/1573))
* Fixed: Flet CLI crashes if `git` is not installed ([#1581](https://github.com/flet-dev/flet/issues/1581))

## 0.8.1

* Fix `auth` and `PubSub` imports in `page.py` and `connection.py`.
* Fix broken `flet pack` command.

## 0.8.0

* 📱🎉 **iOS support** - build standalone iOS apps in Python:
  * [Flet](https://apps.apple.com/app/flet/id1624979699) app in App Store to test Flet projects on iOS devices.
  * New `--ios` switch for `flet run` command to test Flet app on your iOS device.
  * [Testing on iOS guide](https://flet.dev/docs/guides/python/testing-on-ios).
  * [serious_python](https://pub.dev/packages/serious_python) Flutter package to add Python support to a Flutter app.
  * [An example of Flutter app](https://github.com/flet-dev/serious-python/tree/main/example/flet_example) combining [serious_python](https://pub.dev/packages/serious_python) package, [flet](https://pub.dev/packages/flet) package and your Python program into a ready iOS app.
* Part of `flet` package logic moved to a new `flet-runtime` package. `flet` package depends on `flet-runtime`. The new `flet-embed` package introduced depending on `flet-runtime` - to run Python apps embedded into Flutter apps.
* Less annoying re-connecting logic and loading page for mobile Flet apps.
* Enum parameters for `ft.app()`s `view: ft.AppView` and `web_renderer: ft.WebRenderer` parameters (string values are still supported for backward compatibility), for example:

```python
ft.app(main, view=ft.AppView.WEB_BROWSER, web_renderer=ft.WebRenderer.HTML)
```

* Flet packages `version` is centralized in `flet_core.version`.
* 💥 **Breaking change:** OAuth providers must be imported from `flet.auth.providers` module, for example:

```python
from flet.auth.providers import GitHubOAuthProvider
```

* Added `Image.error_content` property - fallback content if image cannot be loaded.
* New `BottomSheet` properties: `dismissible`, `enable_drag`, `show_drag_handle`, `use_safe_area` ([#1468](https://github.com/flet-dev/flet/issues/1468)).
* `ListTile.toggle_inputs` property - clicking on a list tile should toggle the state of `Radio`, `Checkbox` or `Switch` inside the tile.
* New `page` methods for showing/closing overlays: `page.open_banner()`, `page.close_banner()`, `page.open_dialog()`, `page.close_dialog()`, `page.open_bottom_sheet()`, `page.close_bottom_sheet()`.
* New `FletApp` properties: `reconnect_interval_ms`, `reconnect_timeout_ms`, `on_error`.
* New `TextField` properties: `autocorrect`, `enable_suggestions`, `smart_dashes_type`, `smart_quotes_type`.
* New `SafeArea` control.
* New `SnackBar` properties: `behavior`, `dismiss_direction`, `show_close_icon`, `close_icon_color`, `margin`, `padding`, `width`, `elevation`.
* New `View.fullscreen_dialog` property.
* `ft.app()` assumes `assets_dir="assets"` by default.
* New `PaintSweepGradient.rotation` property.

## 0.7.4

* Added `use_color_emoji` to `ft.app()` in `flet-pyodide` ([#1416](https://github.com/flet-dev/flet/issues/1416)).

## 0.7.3

* Fix missing `FLET_APP_WEB` declaration in `flet-pyodide`.

## 0.7.2

* Fix: Route change by url is not working if `page.theme` specified ([#1406](https://github.com/flet-dev/flet/issues/1406)).
* Rollback flutter_svg to 1.1.6 to fix regressions in Plotly charts ([#1402](https://github.com/flet-dev/flet/issues/1402)).
* Force web server in desktop mode with `ft.app(view=ft.FLET_APP_WEB)`.

## 0.7.1

* `ButtonStyle` with `shape` or `side` params failed in flet 0.7.0 ([#1390](https://github.com/flet-dev/flet/issues/1390)).

## 0.7.0

* Programmatically [control scroll position](https://flet.dev/blog/scrolling-controls-and-theming#controlling-scroll-position) and subscribe to [scrolling notifications](https://flet.dev/blog/scrolling-controls-and-theming#receiving-scroll-notifications) in Page, View, Column, Row, ListView and GridView controls.
* [Material color scheme customization](https://flet.dev/blog/scrolling-controls-and-theming#color-scheme-customization)
* [Text theming](https://flet.dev/blog/scrolling-controls-and-theming#text-theming)
* [Scrollbars theming](https://flet.dev/blog/scrolling-controls-and-theming#scrollbar-theme)
* [Tabs theming](https://flet.dev/blog/scrolling-controls-and-theming#styling-tabs-control)
* [Nested page themes](https://flet.dev/blog/scrolling-controls-and-theming#nested-page-themes)
* Flutter upgraded to 3.10 with Dart 3.0 required. CanvasKit WASM size reduced from 2.8 to 1.5 MB.
* Bumped Flutter dependencies: window_manager 0.3.0 → 0.3.2, flutter_markdown 0.6.13 → 0.6.14, markdown 6.0.1 → 7.0.0, file_picker 5.2.5 → 5.3.0, flutter_svg 1.1.6 → 2.0.5, shake 2.1.0 → 2.2.0, fl_chart 0.61.0 → 0.62.0.
* Color emoji support in web apps with "canvaskit" renderer ([docs](https://flet.dev/docs/guides/python/publishing-static-website#color-emojis)).
* Add CLI option -m to run as module ([#1389](https://github.com/flet-dev/flet/issues/1389)).
* Selectable rich text control ([#1386](https://github.com/flet-dev/flet/issues/1386)).

## 0.6.2

* Fix `SnackBar` (and other controls) exit animation.
* Fix `Text` default style color.

## 0.6.1

* Fix regression in `AlertDialog` and `BottomSheet` controls ([#1344](https://github.com/flet-dev/flet/issues/1344))

## 0.6.0

* `Canvas` control ([docs](https://flet.dev/docs/controls/canvas)).
* Rich text support in [`Text` control](https://flet.dev/docs/controls/text#spans).
* Added `url` and `url_target` to controls with `on_click` event ([#1337](https://github.com/flet-dev/flet/pull/1337))
* Auto-follow links in `Markdown` ([docs](https://flet.dev/docs/controls/markdown#auto_follow_links)).
* Capturing web client info: IP and user agent ([#1302](https://github.com/flet-dev/flet/pull/1302))
* Fix: Make non-visual controls working with routing ([#1333](https://github.com/flet-dev/flet/pull/1333))
* Fix: Update `page.route` if typed in the URL ([#1289](https://github.com/flet-dev/flet/pull/1289))

## 0.5.2

* Fix: Dispose controls only on session closed event
* Fix "There is no current event loop" error in auth module

## 0.5.1

* Fix `page` reference in `will_unmount` method.

## 0.5.0

* Fixed: Memory usage continues to increase. ([#1223](https://github.com/flet-dev/flet/issues/1223))
* Fixed: possible memory leak ([#969](https://github.com/flet-dev/flet/issues/969))
* Color values can contain opacity, e.g. `color=red,0.5` or `ft.colors.with_opacity(0.5, "red")`
* 1st class Flet charts based on fl_chart package ([#1255](https://github.com/flet-dev/flet/issues/1255))
* Pyodide 0.23
* Use named loggers in Python ([#1157](https://github.com/flet-dev/flet/issues/1157))
* Fix Contribution guide as PDM is no longer used ([#1124](https://github.com/flet-dev/flet/issues/1124))
* Added focus() method, focus and blur events to Elevated, Outlined, Text and Icon buttons ([#1079](https://github.com/flet-dev/flet/issues/1079))
* New Card props: color, shadow_color, surface_tint_color ([#1078](https://github.com/flet-dev/flet/issues/1078))
* Added WindowDragArea.maximizable property ([#1077](https://github.com/flet-dev/flet/issues/1077))
* Added Container.blur and Container.shadow properties ([#1076](https://github.com/flet-dev/flet/issues/1076))
* Add template for Q&A discussions ([#1070](https://github.com/flet-dev/flet/issues/1070))

## 0.4.2

* Fix reading versioninfo for PyInstaller 5.8.0
* Fix `Dropdown.disable` property

## 0.4.1

* Slider.round to round slider value on a label
* Fix page.client_storage.get_keys() timeout 
* Fix encode() import in PyInstaller integration
* Fix "ConnectionAbortedError" error on Windows
* Consistent licensing across the code - Apache 2.0
* Fix assets loading in a sub-directory app ([#1019](https://github.com/flet-dev/flet/issues/1019))
* Add --distpath option to flet pack and flet publish commands ([#1018](https://github.com/flet-dev/flet/issues/1018))
* Updating manifest.json when using flet publish ([#1014](https://github.com/flet-dev/flet/issues/1014))
* Fix "Address already in use" error on flet run hot reload ([#1007](https://github.com/flet-dev/flet/issues/1007))
* Force Python sub-process to run with UTF-8 encoding ([#1002](https://github.com/flet-dev/flet/issues/1002))
* Fix: View with content crashes in some routing scenarios ([#1001](https://github.com/flet-dev/flet/issues/1001))

## 0.4.0

* Changed re-connection logic to make hot reload work ([#971](https://github.com/flet-dev/flet/issues/971))
* Pyodide publishing fixes and improvements ([#953](https://github.com/flet-dev/flet/issues/953))
* feat: Add PaddingValue to __init__.py ([#936](https://github.com/flet-dev/flet/issues/936))
* Standalone Flet web apps with Pyodide ([#913](https://github.com/flet-dev/flet/issues/913))
* modified `tooltip` attribute from `prefere*` to `prefer*` ([#909](https://github.com/flet-dev/flet/issues/909))
* Fix unicode encoding in `FletTcpSocketServerProtocol`
* Fix relative assets path in desktop app
* PDM changed to Poetry
* Add `--hidden-import` option to `flet pack` command
* Add transparancy to matplotlib ([#889](https://github.com/flet-dev/flet/issues/889))
* Replace Fletd server for desktop apps with a light-weight Python shim ([#838](https://github.com/flet-dev/flet/issues/838))
* add default values in Border dataclass ([#883](https://github.com/flet-dev/flet/issues/883))
* Fix for issue in control.py when checking add command ([#835](https://github.com/flet-dev/flet/issues/835))
* Fix async pubsub ([#868](https://github.com/flet-dev/flet/issues/868))
* add: Border, BorderSide, Scale Offset, Rotate to `__init__.py` ([#866](https://github.com/flet-dev/flet/issues/866))
* Loading images from a local file ([#817](https://github.com/flet-dev/flet/issues/817))
* Asyncio support ([#799](https://github.com/flet-dev/flet/issues/799))
* Set filled=True when setting bgcolor in TextField ([#807](https://github.com/flet-dev/flet/issues/807))
* Page transition without animation ([#809](https://github.com/flet-dev/flet/issues/809))

## 0.3.2

* Fix `flet pack` command on Windows and macOS ([#795](https://github.com/flet-dev/flet/issues/795))

## 0.3.1

* Fixed Flutter package CHANGELOG and README.

## 0.3.0

* `flet pack` CLI to create app bundles with custom icons and metadata ([#770](https://github.com/flet-dev/flet/issues/770))
* Control comments ([#681](https://github.com/flet-dev/flet/issues/681))
* Fix MaterialState error in ButtonStyle ([#689](https://github.com/flet-dev/flet/issues/689))
* Flet CLI moved into separate module ([#679](https://github.com/flet-dev/flet/issues/679))
* Added BorderRadius to `__init__.py` ([#691](https://github.com/flet-dev/flet/issues/691))
* Added dense property to TextField and Dropdown controls ([#696](https://github.com/flet-dev/flet/issues/696))
* Correctly handle control replacement ([#710](https://github.com/flet-dev/flet/issues/710))
* Fix "replace" when moving children in the collection ([#711](https://github.com/flet-dev/flet/issues/711))
* Remove hard-coded colors in Markdown default code theme ([#731](https://github.com/flet-dev/flet/issues/731))
* Authorization should allow to override, such as request_token() methods ([#776](https://github.com/flet-dev/flet/issues/776))

## 0.2.4

* Use correct Flet viewer path when installed from a source package ([#675](https://github.com/flet-dev/flet/issues/675))
* add `ControlEvent` to `__init__.py` ([#657](https://github.com/flet-dev/flet/issues/657))
* fix: handle a few corner cases ([#503](https://github.com/flet-dev/flet/issues/503))

## 0.2.2

* Make `Control.offset` work without animation enabled ([#632](https://github.com/flet-dev/flet/issues/632))
* Added `Dropdown.alignment` property ([#630](https://github.com/flet-dev/flet/issues/630))
* Remove beartype runtime check for all `value` properties
* Fix `page.scroll` to allow None and strings
* Literals to Enums ([#626](https://github.com/flet-dev/flet/issues/626))
* `gapless_playback` is `True` by default for base64 images
* Ability to change border shape of FAB control ([#621](https://github.com/flet-dev/flet/issues/621))
* Added Slider's `on_change_start` and `on_change_end` events ([#620](https://github.com/flet-dev/flet/issues/620))
* DataTable control: 1-to-1 mapping to Flutter ([#583](https://github.com/flet-dev/flet/issues/583))
* Implemented `page.can_launch_url()` ([#582](https://github.com/flet-dev/flet/issues/582))
* Update project changelog from very beginning ([#581](https://github.com/flet-dev/flet/issues/581))
* Publish pre releases to pypi.org ([#579](https://github.com/flet-dev/flet/issues/579))
* Theming Slider control ([#573](https://github.com/flet-dev/flet/issues/573))

## 0.1.65

* Fixed: Floating Action Button now showing on top left ([#567](https://github.com/flet-dev/flet/issues/567))
* Using variable fonts ([#21](https://github.com/flet-dev/flet/issues/21))
* Old flet client app versions do not launch on Mac ([#161](https://github.com/flet-dev/flet/issues/161))
* NavigationBar control ([#193](https://github.com/flet-dev/flet/issues/193))
* `ResponsiveRow` control ([#227](https://github.com/flet-dev/flet/issues/227))
* Add code syntax highlighter to markdown ([#294](https://github.com/flet-dev/flet/issues/294))
* feature: add mouse scroll wheel event ([#354](https://github.com/flet-dev/flet/issues/354))
* Tooltip class ([#367](https://github.com/flet-dev/flet/issues/367))
* BottomSheet control ([#483](https://github.com/flet-dev/flet/issues/483))
* Fixed: Calling `update()` inside `Control.did_mount()` causes deadlock ([#489](https://github.com/flet-dev/flet/issues/489))
* Add `page.window_maximizable` ([#494](https://github.com/flet-dev/flet/issues/494))
* Add an ability to change font family of `TextField` ([#511](https://github.com/flet-dev/flet/issues/511))
* Feature: Theming Switch and Checkbox component ([#523](https://github.com/flet-dev/flet/issues/523))
* Change shape of AlertDialog ([#537](https://github.com/flet-dev/flet/issues/537))
* Fixed: Saving and retreiving a string value from client storage adds quotation marks ([#545](https://github.com/flet-dev/flet/issues/545))
* Matplotlib and Plotly Charts ([#509](https://github.com/flet-dev/flet/issues/509))
* make control a cooperative object ([#490](https://github.com/flet-dev/flet/issues/490))

## 0.1.62

* Initial release of Flet Flutter package.
* GestureDetector and other fixes ([#459](https://github.com/flet-dev/flet/issues/459))
* removed all problems except dart:html problem because it needs material html kind of thing ([#461](https://github.com/flet-dev/flet/issues/461))
* fix: ensure correct version is fetched in dev mode ([#443](https://github.com/flet-dev/flet/issues/443))
* Fix controls setter for empty list input ([#454](https://github.com/flet-dev/flet/issues/454))
* make ink=True behavior consistent with ink=False ([#427](https://github.com/flet-dev/flet/issues/427))