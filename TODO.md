# TODO

List of things to do...

<br><br>

## Misc

- [ ] Update email address in library packages + github.

<br><br>

## WIP

- [ ] `react-native-ios-modal`: Initial Rewrite #1.

	* Next Version: `1.0` — Initial rewrite to use modern project template + add types.
		* Do not re-write logic yet or add any features yet.

	- [x] Create a `wip` branch.
	- [ ] Create a new project, and transplant the old project into the newly created project.
		- [x] Create a new template project.
		- [ ] Build and run template project.
		- [ ] Re-Configure template project and remove any unnecessary additions/packages/etc. 
			- [ ] Temporarily reconfigure `tsconfig` to make it less strict.
		- [ ] Migrate project into the new project.
			- [ ] Remove generated template/placeholder files
			- [ ] Migrate iOS project
			- [ ] Migrate example files
			- [ ] Migrate js files.
		- [ ] Test and make sure it builds and compiles. 
		- [ ] Transfer the old git history into the new project.
		- [ ] Commit changes and release.
	- [ ] Types - Add placeholder types.
	- [ ] Example - Update example.
	- [ ] Docs - Add "Rewrite WIP" in library README.

<br>

- [ ] `react-native-ios-modal`: Initial Rewrite #2

	* Next Version: `2.0` — Rewrite to use `react-native-ios-utilities`

	- [ ] **Refactor**: Use `RNIWrapperView` for holding the modal content.
	- [ ] **Refactor**: Use `RNIJSComponentWillUnmountNotifiable` for cleanup.

<br><br>

## Completed

- [x] **Update**: `react-native-ios-context-menu`

  - [x] **Git**: Create `wip` branch
  - [x] **Refactor**: Types —  `RNIContextMenuViewModule.notifyComponentWillUnmount` Create corresponding typescript type + update existing usage to use that type via a union.
  - [x] **Refactor**: Types — Extract types from `src/types/ImageItemConfig` to their own files inside a directory called `ImageItemConfig`.
  
- [x] **Update**: `react-native-ios-utilities` and `react-native-ios-popover`

	- [x] `react-native-ios-utilities` — **Update**: Sync changes from `react-native-ios-context-menu`
		- [x] `RNIJSComponentWillUnmountNotifiable`
		- [x] `RNICleanupMode`
		- [x] `RNIUtilitiesModule`
		- [x] `RNIImage`

	<br>

	- [x] `react-native-ios-popover` — **Refactor**: Update to use `RNIJSComponentWillUnmountNotifiable`. 
	- [x] `react-native-ios-popover` — **Refactor**: Make swift classes + types public. 
	- [x] `react-native-ios-utilities` — **Release**: Publish a new pre-release version.
	- [x] `react-native-ios-popover` —  **Update**: Bump `react-native-ios-utilities` version dependency to use new pre-release version.
	- [x] `react-native-ios-popover` —  **Test**: Run and test example to make sure everything works.
	- [x] `react-native-ios-popover` —  **Release**: Publish a new pre-release version.
	- [x] `react-native-ios-popover` —  **Test**: Run and test example to make sure everything works.
	- [x] `react-native-ios-utilities` — **Release**: Publish a new major version.
		* **Version**: `0.x` -> `2.x`
	
	<br>
	
	- [x] `react-native-ios-popover` — **Docs**: Add dependency + package version compatibility table.
	- [x] `react-native-ios-popover` —  **Package**: Use semantic versioning for peer dependency to  `react-native-ios-utilities`.
		* Lock peer dependency version to a specific major version
			* `react-native-ios-popover`: `1.x` -> `2.x`
			* `react-native-ios-context-menu`: `2.x` -> `3.x`
			* `react-native-ios-utilities`: `0.x` -> `2.x`
		* `react-native-ios-utilities` - `2.x`
			* `react-native-ios-popover` - `2.x`
		* `react-native-ios-utilities` - `3.x`
			* `react-native-ios-modal` - `3.x`
			* `react-native-ios-popover` - `3.x`
