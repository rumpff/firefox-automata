![theme preview](https://raw.githubusercontent.com/rumpff/firefox-automata/refs/heads/master/.github/preview.gif)

_firefox theme with [sidebery](https://github.com/mbnuqw/sidebery) for vertical tabs, firefox color for browser theme and userChrome.css to remove native tabs_

## Installation instructions
- Clone the repo or [download ZIP](https://github.com/rumpff/firefox-automata/archive/refs/heads/master.zip)
  - Install fonts located in `/font/` on your system
- Install extensions
  - [sidebery](https://addons.mozilla.org/en-US/firefox/addon/sidebery/)
  - [Firefox Color](https://addons.mozilla.org/en-US/firefox/addon/firefox-color/)
- Open firefox settings
  - Set tabs to horizontal
  - Show sidebar off
- Apply firefox color theme [here](https://color.firefox.com/?theme=XQAAAAJSAgAAAAAAAABBqYhm849SCicxcUEYWXcGHf3p79EhVQAnmGJYqG4DoUDfxMlADprKotdniB9Quv508B4D3ngFlE3CEKl3ryTLYKet1lPtHse2GfKMQ0SK8jIslgBfZlT2zxb3tnSbeRlqbj7LCsA0worH-84obc0Aqy9HFCTw27buIk5b4Mmwb8kKnkK8b6bYaW1do7miJQDdEXV7Szoi1UhNIt44J_TDRwpk0qxKpIgSEAx66mU_LaKhKKowNiYNYgrjxP1M9KygDtayKwlSdaQxx0-pxQPOfS6wKzrtkT47BVXzAuO9ebxyJgdCKby7cvnyBfiL17XowxdoRTjuULb6NkbA7MqJ2YJyi7ZuxysMGoNDJG1qahv_sb49wA)
- Open sidebery settings
  - Scroll to Help and click on import addon data. import `/config/sidebery-data.json`
  - Scroll down and open the Styles editor
  - Copy contents of `/style/sidebery/sidebar.css` into right area
  - Click on Group page and copy contents of `/style/sidebery/group.css`
- Broswe to `about:config` and click Continue
  - Search for `toolkit.legacyUserProfileCustomizations.stylesheets` and click the toggle button to set it to `true`
- Open your firefox profile folder. (browse to `about:support` and open the profile directory)
  - Create folder `chrome` and copy `/style/firefox/userChrome.css` in it. (if it already exists, add contents to existing file)
  - Restart firefox
- Right click next to url bar and click Customize Toolbar. Drag the Sidebars icon left corner to the center. Click Done 
- Click the sidebery extension icon to open the tabs sidebar. (shortcut might be `F1` or `Ctrl+E`)
- Open new tab, click customize bottom right, Upload an image, select `/img/new-tab.png`

## Customization intrsuctions
- Open sidebery settings, tweak the following to your liking:
- Navigation bar:
  - Layout (default: horizontal)
  - Bottom bar of tabs panel: toggle off what you dont want
  - Enabled elements: Re order navigation bar elements here
- Group page
  - Choose between grid (default) or list
- Tabs tree
  - Disable tabs tree structure if you dont want indented tabs
- Tabs preview
  - Enable and grant permission if you want tab previews. Pick a preview mode you like
- Appearance
  - Choose a font size (default: L)
  - Animations. Choose speed (default: normal) or turn off all togehter
  - Color scheme. if you dont use firefox color make sure to select light here
- Cusomizing tab icons
  - Go to Styles editor and scroll down. (`ctrl+f favicon`)
  - To replace icons with squares remove the `/*` and `*/` _below_ `/* Uncomment for squares instead of favicons */`
  - To revert to colored icons remove everything below `/* -- styled favicons --- */`
  ## Update instructions
  - Sidebery doesn't allow for dynamically loading css yet. for now replace sidebar and group styles manually with latest version
