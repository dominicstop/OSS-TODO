# TODO



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
	- [ ] `react-native-ios-popover` — **Refactor**: Make swift classes + types public. 
	- [ ] `react-native-ios-utilities` — **Release**: Publish a new pre-release version.
	- [x] `react-native-ios-popover` —  **Update**: Bump `react-native-ios-utilities` version dependency to use new pre-release version.
	- [ ] `react-native-ios-popover` —  **Test**: Run and test example to make sure everything works.
	- [ ] `react-native-ios-popover` —  **Release**: Publish a new pre-release version.
	- [ ] `react-native-ios-popover` —  **Test**: Run and test example to make sure everything works.
	- [ ] `react-native-ios-popover` — **Docs**: Add dependency + package version compatibility table.
	- [ ] `react-native-ios-utilities` — **Release**: Publish a new major version.
		* **Version**: `0.x` -> `2.x`
	
	<br>
	
	- [ ] `react-native-ios-popover` —  **Package**: Use semantic versioning for peer dependency to  `react-native-ios-utilities`.
		* Lock peer dependency version to a specific major version
			* `react-native-ios-popover`: `1.x` -> `2.x`
			* `react-native-ios-context-menu`: `2.x` -> `3.x`
			* `react-native-ios-utilities`: `0.x` -> `2.x`
		* `react-native-ios-utilities` - `2.x`
			* `react-native-ios-popover` - `2.x`
		* `react-native-ios-utilities` - `3.x`
			* `react-native-ios-modal` - `3.x`
			* `react-native-ios-popover` - `3.x`

<br>

- [ ] `react-native-ios-modal`: Re-write library.
	- [ ] Create a `wip` branch.
	- [ ] Transplant project configuration
	- [ ] Types - Add placeholder types.