#### 3.1.0-beta.1: Beta Release


Editor

 - NEW: Locking Flows (#3938) @knolleary
 - NEW: Improve UX around hiding flows via context menu (#3930) @knolleary
 - NEW: Add support for inline image in markdown editor by drag and drop of an image file (#4006) @HiroyasuNishiyama
 - NEW: Add support for mermaid diagram to markdown editor (#4007) @HiroyasuNishiyama
 - NEW: Support uri fragments for nodes and groups including edit support (#3870) @knolleary
 - NEW: Add global environment variable feature (#3941) @HiroyasuNishiyama

 - Remember compact/pretty flow export user choice (#3974) @Steve-Mcl
 - fix .red-ui-notification class (#4035) @xiaobinqt
 - Fix border radius on Modules list header (#4038) @bonanitech
 - fix workspace reference error in case of empty tabs (#4029) @HiroyasuNishiyama
 - Disable delete tab menu when single tab exists (#4030) @HiroyasuNishiyama
 - Disable hide all menu if all tabs hidden (#4031) @HiroyasuNishiyama
 - fix hide subflow tooltip (#4033) @HiroyasuNishiyama
 - Fix disabled menu items in project feature (#4027) @kazuhitoyokoi
 - Let themes change radialMenu text colors (#3995) @bonanitech
 - Add Japanese translations for v3.0.3 (#4012) @kazuhitoyokoi
 - Add Japanese translation for v3.1.0-beta.0 (#3997) @kazuhitoyokoi
 - Add Japanese translation for v3.1.0-beta.0 (#3916) @kazuhitoyokoi
 - Hide subflow category after deleting subflow (#3980) @kazuhitoyokoi
 - Prevent dbl-click opening node edit dialog with text selected (#3970) @knolleary
 - Handle replacing unknown node inside group or subflow (#3921) @knolleary
 - Fix #3939, red border red-ui-typedInput-container (#3949) @Steveorevo
 - i18n item URL copy notification & add Japanese message (#3946) @HiroyasuNishiyama
 - add Japanese message for item url copy actions (#3947) @HiroyasuNishiyama
 - Fix autocomplete entry for responseUrl (#3884) @knolleary
 - Fix Japanese translation for JSONata editor (#3872) @HiroyasuNishiyama
 - Fix search type with spaces (#3841) @Steve-Mcl
 - Fix error hanndling of JSONata expression editor for extended functions (#3871) @HiroyasuNishiyama
 - Add button type to the adding SSH key button (#3866) @kazuhitoyokoi
 - Check radio button as default in project dialog (#3879) @kazuhitoyokoi
 - Add $clone as supported function (#3874) @HiroyasuNishiyama
 - Env var jsonata (#3807) @HiroyasuNishiyama
 - Add Japanese translation for v3.0.2 (#3852) @kazuhitoyokoi

Runtime

 - Force IPv4 name resolution to have priority (#4019) @dceejay
 - Fix async loading of modules containing both nodes and plugins (#3999) @knolleary
 - Use main branch as default in project feature (#4036) @kazuhitoyokoi
 - Rename package var to avoid strict mode error (#4020) @knolleary
 - Fix typos in settings.js (#4013) @ypid
 - Ensure credentials object is removed before returning node in getFlow request (#3971) @knolleary
 - Ignore commit error in project feature (#3987) @kazuhitoyokoi
 - Update dependencies (#3969) @knolleary
 - Add check that node sends object rather than primitive type (#3909) @knolleary
 - Ensure key_path is quoted in GIT_SSH_COMMAND in case of spaces in pathname (#3912) @knolleary
 - Fix nodesDir scan when node package has js/html in sub dir to package.json (#3867) @Steve-Mcl
 - Fix file permissions (#3917) @kazuhitoyokoi
 - ci: add minimum GitHub token permissions for workflows (#3907) @boahc077

Nodes

 - Catch: fix typo in catch.html (#3965) @we11adam
 - Change: Fix change node overwriting msg with itself (#3899) @dceejay
 - Comment node: Clarify where the text will appear (#4004) @dirkjanfaber
 - CSV: change replace to replaceAll (#3990) @dceejay
 - CSV node: check header properties for ' and " (#3920) @dceejay
 - CSV: Fix for CSV undefined property (#3906) @dceejay
 - Delay: let delay node handle both flush then reset (#3898) @dceejay
 - Function: Limit number of ports in function node (#3886) @kazuhitoyokoi
 - Function: Remove dot from variable name for external module in function node (#3880) @kazuhitoyokoi
 - Function: add function node monaco types util and promisify (#3868) @Steve-Mcl
 - HTTP In: Ensure msg.req.headers is enumerable (#3908) @knolleary
 - HTTP Request: Support form-data arrays (#3991) @hardillb
 - HTTP Request: Fix httprequest tests to be more lenient on error message (#3922) @knolleary
 - HTTP Request: Add missing property to node object HTTPRequest (#3842) @hardillb
 - HTTP Request/Response: Support sortable list on property UI of http request and http response nodes (#3857) @kazuhitoyokoi
 - HTTP Response: Ensure statusCode is a number (#3894) @hardillb
 - Inject: Allow Inject node to work with async context stores (#4021) @knolleary
 - Join/Batch: Add count to join and batch node labels (#4028) @dceejay
 - MQTT: Fix birth topic handling in MQTT node (#3905) @Steve-Mcl
 - MQTT: Fix pull-down menus of MQTT configuration node (#3890) @kazuhitoyokoi
 - MQTT: Prevent invalid mqtt birth topic crashing node-red (#3869) @Steve-Mcl
 - MQTT: ensure sessionExpiry(Interval) is applied (#3840) @Steve-Mcl
 - MQTT: Fix mqtt nodes not reconnecting on modified-flows deploy (#3992) @knolleary
 - MQTT: fix single subscription mqtt node status (#3966) @Steve-Mcl
 - Range: Add drop mode to range node (#3935) @dceejay
 - Remove done from describe (#3873) @HiroyasuNishiyama
 - Split node: avoid duplicate done call for buffer split (#4000) @knolleary
 - Status: Fix typo in 25-status.html (#3981) @kazuhitoyokoi
 - TCP Node: ensure newline substitution applies to whole message (#4009) @dceejay
 - Template: Add information about environment variable to template node (#3882) @kazuhitoyokoi
 - Trigger: Hide trigger node repeat send option if sending nothing (#4023) @dceejay
 - Watch: fix watch node test on MacOS/ARM (#3942) @HiroyasuNishiyama

#### 3.0.2: Maintenance Release

Editor

 - Fix workspace chart bottom property (#3812) @bonanitech
 - Update german translation (#3802) @Dennis14e
 - Support color reset to the default in subflow and group (#3801) @kazuhitoyokoi
 - Allow generateNodeNames to handle names containing regex control chars (#3817) @knolleary
 - Hide scrollbars until they're needed (#3808) @bonanitech
 - Include junctions/groups when exporting subflows plus related fixes (#3816) @knolleary
 - remove console.log (#3820) @Steve-Mcl

Runtime

 - Register subflow module instance node with parent flow (#3818) @knolleary

Nodes

 - HTTP Request: Allow HTTP Headers not in spec (#3776) @hardillb

#### 3.0.1: Maintenance Release

Editor

 - Allow codeEditor theme to be set even if `codeEditor` is not set in settings.js (#3794) @Steve-Mcl
 - Sys info (diagnostics report) amendments (#3793) @Steve-Mcl
 - Allow `mode` and `title` to be omitted in `options` argument for `createEditor` (#3791) @Steve-Mcl
 - Fix focus issues (#3789) @Steve-Mcl
 - Ensure all typedInput buttons have button type set (#3788) @knolleary
 - Do not flag hasUsers=false nodes as unused in search (#3787) @knolleary
 - Properly position quick-add dialog in all cases (#3786) @knolleary
 - Ensure quick-add dialog does not obscure ghost node when shifted (#3785) @knolleary
 - Remove use of Object.hasOwn (#3784) @knolleary

#### 3.0.0: Milestone Release

Editor

 - Use theme page and header values if settings.js values are not present (#3767) @Steve-Mcl
 - Focus editor for undo after some actions in menu (#3759) @kazuhitoyokoi
 - Ensure node icon shade has properly rounded corners (#3763) @knolleary
 - Fix storing subflow credential type when input has multiple types (#3762) @knolleary
 - Ensure global-config and flow-config have info in the hierarchy popover (#3752) @Steve-Mcl
 - Include dirty state in history event (#3748) @Steve-Mcl
 - Fix display direction of context sub-menu (#3746) @knolleary
 - Fix clear pinned paths of debug sidebar menu (#3745) @HiroyasuNishiyama
 - prevent exception generating tooltip for deleted nodes (#3742) @Steve-Mcl
 - Fix context menu issues ready for v3 beta.5 (#3741) @Steve-Mcl
 - Do not generate new node-ids when pasting a cut flow (#3729) @knolleary
 - Fix to prevent node from moving out of workspace (#3731) @HiroyasuNishiyama
 - Don't let themes change disabled config node background color (#3736) @bonanitech
 - Move colors left behind in #3692 to CSS variables (#3737) @bonanitech
 - Fix handling of global debug message (#3733) @HiroyasuNishiyama
 - Fix label overflow @ config-node palette (#3730) @ralphwetzel
 - Fix defaulting to monaco if settings does not contain codeEditor (#3732) @knolleary
 - Disable keyboard shortcut mapping when showing Edit[..]Dialog (#3700) @ralphwetzel
 - Update add-junction menu to work in more cases (#3727) @knolleary
 - Ensure importMap is not null when using import UI (#3723) @Steve-Mcl
 - Add Japanese translations for v3.0-beta.4 (#3724) @kazuhitoyokoi
 - Fix "split with" on virtual links (#3766) @Steve-Mcl

Runtime

 - Do not remove unknown credentials of Subflow Modules (#3728) @knolleary
 - Add missing entries from beta.4 changelog (#3721) @knolleary

Nodes

 - Change: Fix change node, not handling from field properly when using context (#3754) @Fadoli
 - Link Call: Fix linkcall registry bugs (#3751) @Steve-Mcl
 - WebSocket: Fix close timeout of websocket node (#3734) @HiroyasuNishiyama

#### 3.0.0-beta.4: Beta Release

Editor

 - Move all colours to CSS variables (#3692) @bonanitech
 - Fix clicking on node in workspace to hide context menu (#3696) @knolleary
 - Fix credential type input item of subflow template (#3703) @HiroyasuNishiyama
 - Add option flag `reimport` to `importNodes` (#3718) @Steve-Mcl
 - Update german translation (#3691) @Dennis14e
 - List welcome tours in help sidebar (#3717) @knolleary
 - Ensure 'hidden flow' count doesn't include subflows (#3715) @knolleary
 - Fix Chinese translate (#3706) @hotlong
 - Fix use default button for node icon (#3714) @kazuhitoyokoi
 - Fix select boxes vertical alignment (#3698) @bonanitech
 - Ensure workspace clean after undoing dropped node (#3708) @Steve-Mcl
 - Use solid colour as config node icon background to hide text overflow (#3710) @Steve-Mcl
 - Increase quick-add height to reveal 2 most recent entries (#3711) @Steve-Mcl
 - Set default editor to monaco in absence of user preference (#3702) @knolleary
 - Add Japanese translations for v3.0-beta.3 (#3688) @kazuhitoyokoi
 - Fix handling of spacebar inside JSON visual editor (#3687) @knolleary
 - Fix menu padding to handle both icons and submenus (#3686) @knolleary
 - Include scroll offset when positioning quick-add dialog (#3685) @knolleary

Runtime

 - Allow flows to be stopped and started manually (#3719) @knolleary
 - Import default export if node is a transpiled es module (#3669) @dschmidt
 - Leave Monaco theme commented out by default (#3704) @bonanitech

Nodes

 - CSV: Fix CSV node to handle when outputting text fields (#3716) @dceejay
 - Delay: Fix delay rate limit last timing when empty (#3709) @dceejay
 - Link: Ensure link-call cache is updated when link-in is modified (#3695) @Steve-Mcl
 - Join: Join node in reduce mode doesn't keep existing msg properties (#3670) @dceejay
 - Template: Add support for evalulating {{env.<var>}} within a template node (#3690) @cow0w

#### 3.0.0-beta.3: Beta Release

Editor

 - Add Right-Click content menu (#3678) @knolleary
 - Fix disable junction (#3671) @HiroyasuNishiyama
 - Add Japanese translations for v2.2.3 (#3672) @kazuhitoyokoi
 - Reset mouse state when switching tabs (#3643) @knolleary
 - Fix uncorrect fix of junction to subflow conversion (#3666) @HiroyasuNishiyama
 - Fix undoing junction to subflow (#3653) @HiroyasuNishiyama
 - Fix conversion of junction to subflow (#3652) @HiroyasuNishiyama
 - Fix to include junction to exported nodes (#3650) @HiroyasuNishiyama
 - Fix z-index value for shade to cover nodes in palette (#3649) @kazuhitoyokoi
 - Fix to extend escaped subflow category characters (#3647) @HiroyasuNishiyama
 - Fix to sanitize tab name (#3646) @HiroyasuNishiyama
 - Fix selector placement (#3644) @bonanitech
 - Add Japanese translations for v3.0-beta.2 (#3622) @kazuhitoyokoi
 - Fix new folder menu of save to library dialog (#3633) @HiroyasuNishiyama
 - Fix layer of palette node (#3638) @HiroyasuNishiyama
 - Fix to place a node dragged from palette within the workspace (#3637) @HiroyasuNishiyama
 - Fix typo in CSS (#3628) @bonanitech
 - Use the correct variable for the gutter text color (#3615) @bonanitech


Runtime

 - Support loading node modules from `nodesdir` (#3676) @Steve-Mcl
 - fix buffer parse error message of evaluateNodeProperty (#3624) @HiroyasuNishiyama

Nodes

 - File: Further simplify file node filename entry UX (v3) (#3677) @Steve-Mcl
 - Function: Fix initial cursor position of init/finalize tab of function node (#3674) @HiroyasuNishiyama
 - Function: Fix ESM module loading in Function node (#3645) @knolleary
 - Inject: Fix JSONata evaluation of inject button (#3632) @HiroyasuNishiyama
 - TCP: Dont delete TCP socket twice (#3630) @Steve-Mcl
 - MQTT Node: define noproxy variable (#3626) @Steve-Mcl
 - Debug: i18n debug sidebar node label (#3623) @HiroyasuNishiyama

#### 3.0.0-beta.2: Beta Release

**Migration from 2.x**

 - The 'slice wires' action has changed from Ctrl-RightMouseButton to Alt-LeftMouseButton

Editor

 - Rework Junctions to be more node like in their event handling (#3607) @knolleary
 - Change slicing / slice-junction operations over to mouse button 0 (Left Mouse Button) (#3609) @Steve-Mcl
 - Do not slice-junction link node wires (#3608) @knolleary
 - Handle many-to-one slicing of wires (#3604) @knolleary
 - Ensure ACE worker options are set (#3611) @Steve-Mcl
 - Remove duplicate history add of ungroup event (#3605) @knolleary
 - use text width instead of number of characters for deciding select fi… (#3603) @HiroyasuNishiyama
 - Update Japanese info of link call node reflecting update of English info (#3600) @HiroyasuNishiyama
 - Fix typedInput label not visible on themes (#3580) @bonanitech
 - Fix project switching when junctions are present (#3595) @Steve-Mcl
 - Fix junction: when wiring from a regular nodes INPUT, backwards to a junction (#3591) @Steve-Mcl
 - Fix error initialising flow tab editor (#3585) @Steve-Mcl
 - Add Japanese translations for v3.0-beta.1 (#3576) @kazuhitoyokoi
 - Fix image paths where `red/image/typedInput/XXXX.png` should be `red/image/typedInput/XXXX.svg` (#3592) @kazuhitoyokoi
 - Fix browser console error Uncaught TypeError when searching certain terms (#3584) @Steve-Mcl

Runtime

 - fix error on system-info action (#3589) @HiroyasuNishiyama

Nodes

 - I18n switch rule selector (#3602) @HiroyasuNishiyama
 - Handle removal of event handlers to allow mqtt client.end() to work (#3594) @PhilDay-CT
 - update link-call node info according to current behavior (#3597) @HiroyasuNishiyama


#### 3.0.0-beta.1: Beta Release

**Migration from 2.x**

 - Node-RED now requires Node.js 14.x or later.
 - New installs of Node-RED will default to the monaco editor.


Editor

 - Add Junctions (#3462) @knolleary
 - Allow node name to be auto-generated when added (#3478, #3538) @knolleary
 - Set monaco as default code editor as of v3.x (#3543) @Steve-Mcl
 - Update Monaco to V0.33.0 (#3522) @Steve-Mcl
 - Auto-complete Improvements (#3521) @Steve-Mcl
 - Add a tooltip to debug sidebar messages to reveal full path to node (#3503) @knolleary
 - Fix down arrow triggering menu in search box (#3507) @Steve-Mcl
 - Add Japanese translations for v3.0 (#3512) @kazuhitoyokoi
 - Add feature: Continuous search tools (search previous, search next) (#3405) @Steve-Mcl
 - Add feature: split-wire-to-links (#3399, #3476) @Steve-Mcl
 - Add copy button to node properties tables (#3390) @knolleary
 - Add info-tab search options dropdown to the regular search (#3395) @Steve-Mcl
 - New Feature: Add ability to find modified nodes/flows. (#3392) @Steve-Mcl
 - Code editor ux improvements around remembering state of each code editor in a flow (#3553) @Steve-Mcl
 - Make it easier to apply themes on SVG icons (#3515) @bonanitech
 - Add support of property validation message (#3438) @HiroyasuNishiyama
 - Ensure node validation tooltip is closed when field becomes valid (#3570) @knolleary
 - Add "search for" buttons to notifications (#3567) @Steve-Mcl
 - Don't let themes change node config colors (#3564) @bonanitech
 - Fix gap between typedInput containers borders (#3560) @bonanitech
 - Fix recording removed links in edit history (#3547) @knolleary
 - Remove unused SASS vars (#3536) @bonanitech
 - Add custom style for jQuery widgets borders (#3537) @bonanitech
 - fix out of scope reference of hasUnusedConfig variable (#3535) @HiroyasuNishiyama
 - correct "non string" check parenthesis (#3524) @Steve-Mcl
 - Ensure i18n of scoped package name (#3516) @Steve-Mcl
 - Prevent shortcut deploy when deploy button shaded (#3517) @Steve-Mcl
 - Fix: Sidebar "Configuration" filter button tooltip (#3500) @ralphwetzel
 - Add the ability to customize diff colors even more (#3499) @bonanitech
 - Do JSON comparison of old value/new value in editor (#3481) @Steve-Mcl
 - Fix nodes losing their wires when in an iframe (#3484) @zettca
 - Improve scroll into view (#3468) @Steve-Mcl
 - Do not show 1st tab if hidden when loading (#3464) @Steve-Mcl

Runtime

 - Fix importing external module from node-red module (#3541) @knolleary
 - Add support for multiple static paths with optional static root (#3542) @Steve-Mcl
 - Store external token when authenticating if provided (#3460) @ArFe
 - Support OAuth/OpenID logout (#3388) @mw75
 - Allow adminAuth to auto-login users when using passport strategy (#3519) @knolleary
 - Add runtime diagnostics admin endpoint (#3511) @Steve-Mcl
 - Don't start if user has no home directory (#3540) @hardillb
 - Error on invalid encrypted credentials (#3498) @sammachin

Nodes

 - Debug: Add message count option to Debug status (#3544 #3551) @rafaelmuynarsk @knolleary
 - File: Change basic Filename field to a typedInput (#3533) @Steve-Mcl
 - HTTP Request: Add UI for Http Request node headers (#3488) @Steve-Mcl
 - Inject: let inject optionally fire at start in only at time mode. (#3385) @dceejay
 - Link Call: Dynamic link call (#3463) @Steve-Mcl
 - Link Call: Display link targets of nodes in a regular flow, for Link Call nodes inside a subflow (#3528) @Steve-Mcl
 - MQTT: MQTT payload auto parsing improvements (#3530) @Steve-Mcl
 - MQTT: Add client and Runtime MQTT topic validation (#3563) @Steve-Mcl [dev]
 - MQTT: save and restore v5 config user props (#3562) @Steve-Mcl
 - MQTT: Fix incorrect MQTT status (#3552) @Steve-Mcl
 - MQTT: fix reference error of msg.status in debug node (#3526) @HiroyasuNishiyama
 - MQTT: Add unit tests for MQTT nodes (#3497) @Steve-Mcl
 - MQTT: fix typo of will properties (#3502) @Steve-Mcl
 - MQTT: ensure mqtt v5 props can be set false (#3472) @Steve-Mcl
 - Switch: add check for NaN in is of type number to be false (#3409) @dceejay
 - TCP: TCP node better split (#3465) @dceejay
 - Watch: Update Watch node to use node-watch module (#3559 #3569) @knolleary
 - WebSocket: call done after ws disconnects (#3531) @Steve-Mcl

#### Older Releases

Change logs for older releases are available on GitHub: https://github.com/node-red/node-red/releases
