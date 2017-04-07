# api documentation for  [react-mdl (v1.9.0)](https://github.com/tleunen/react-mdl#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-react-mdl.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-react-mdl) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-react-mdl.svg)](https://travis-ci.org/npmdoc/node-npmdoc-react-mdl)
#### React Components for Material Design Lite

[![NPM](https://nodei.co/npm/react-mdl.png?downloads=true)](https://www.npmjs.com/package/react-mdl)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-mdl/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-react-mdl_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-mdl/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-react-mdl/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-react-mdl/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Tommy Leunen",
        "email": "tommy.leunen@gmail.com",
        "url": "http://tommyleunen.com/"
    },
    "bugs": {
        "url": "https://github.com/tleunen/react-mdl/issues"
    },
    "dependencies": {
        "clamp": "^1.0.1",
        "classnames": "^2.2.3",
        "lodash.isequal": "^4.4.0"
    },
    "description": "React Components for Material Design Lite",
    "devDependencies": {
        "add-stream": "^1.0.0",
        "babel-cli": "^6.11.4",
        "babel-core": "^6.13.2",
        "babel-loader": "^6.2.5",
        "babel-plugin-__coverage__": "^11.0.0",
        "babel-plugin-transform-object-rest-spread": "^6.6.5",
        "babel-polyfill": "^6.13.0",
        "babel-preset-es2015": "^6.13.2",
        "babel-preset-react": "^6.5.0",
        "chai": "^3.5.0",
        "chai-enzyme": "^0.5.0",
        "conventional-changelog": "^1.1.0",
        "cross-env": "^2.0.0",
        "enzyme": "^2.4.1",
        "eslint": "^2.7.0",
        "eslint-config-airbnb": "^9.0.1",
        "eslint-plugin-import": "^1.13.0",
        "eslint-plugin-jsx-a11y": "^1.5.3",
        "eslint-plugin-react": "5.1.1",
        "expect": "^1.16.0",
        "gatsby": "^0.11.6",
        "gh-pages": "^0.11.0",
        "isparta": "^4.0.0",
        "isparta-loader": "^2.0.0",
        "json-loader": "^0.5.4",
        "karma": "^1.2.0",
        "karma-chai": "^0.1.0",
        "karma-chrome-launcher": "^1.0.1",
        "karma-cli": "^1.0.0",
        "karma-coverage": "^1.1.1",
        "karma-mocha": "^1.0.1",
        "karma-mocha-reporter": "^2.1.0",
        "karma-sinon": "^1.0.5",
        "karma-sourcemap-loader": "^0.3.7",
        "karma-webpack": "^1.8.0",
        "mocha": "^3.0.2",
        "react": "^15.3.1",
        "react-addons-test-utils": "^15.3.1",
        "react-dom": "^15.3.1",
        "react-router": "^2.6.1",
        "rimraf": "^2.5.4",
        "sinon": "^1.17.5",
        "standard-version": "^2.4.0",
        "webpack": "^1.13.2",
        "webpack-dev-server": "^1.14.1"
    },
    "directories": {},
    "dist": {
        "shasum": "e7f285c68639cab40f0c9fff0e91ec605563c4e8",
        "tarball": "https://registry.npmjs.org/react-mdl/-/react-mdl-1.9.0.tgz"
    },
    "gitHead": "3a6a75f808d8bd03e63d3e13088987b3ea2accbe",
    "homepage": "https://github.com/tleunen/react-mdl#readme",
    "jsnext:main": "src/index.js",
    "keywords": [
        "react",
        "react-component",
        "mdl",
        "material-design",
        "badge",
        "button",
        "card",
        "checkbox",
        "data-table",
        "fab-button",
        "icon",
        "icon-button",
        "icon-toggle",
        "radio",
        "radio-group",
        "switch",
        "textfield",
        "progress",
        "progress-bar",
        "spinner",
        "slider",
        "tooltip",
        "menu",
        "dropdown",
        "Layout",
        "Drawer",
        "Grid",
        "Tabs"
    ],
    "license": "MIT",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "tleunen",
            "email": "tommy.leunen@gmail.com"
        }
    ],
    "name": "react-mdl",
    "optionalDependencies": {},
    "peerDependencies": {
        "react": "0.14.x || ^15.0.0-rc",
        "react-dom": "0.14.x || ^15.0.0-rc"
    },
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/tleunen/react-mdl.git"
    },
    "scripts": {
        "build-docs": "cd docs && ./node_modules/.bin/gatsby build --prefix-links",
        "build-min": "cross-env NODE_ENV=production webpack -p src/index.js out/ReactMDL.min.js --output-library ReactMDL --output-library-target umd",
        "build-umd": "cross-env NODE_ENV=production webpack src/index.js out/ReactMDL.js --output-library ReactMDL --output-library-target umd",
        "clean": "rimraf coverage lib out",
        "compile": "rimraf lib && babel src --ignore __tests__ --out-dir lib",
        "lint": "eslint src scripts",
        "pretest": "npm run lint",
        "react:14": "npm run react:clean && npm i react@0.14 react-dom@0.14 react-addons-test-utils@0.14",
        "react:15": "npm run react:clean && npm i react@15 react-dom@15 react-addons-test-utils@15",
        "react:clean": "rimraf node_modules/react node_modules/react-dom node_modules/react-addons-test-utils",
        "release": "./scripts/release.sh",
        "release-docs": "gh-pages -d docs/public/ -m 'Updates v'$npm_package_version",
        "serve-docs": "cd docs && ./node_modules/.bin/gatsby develop",
        "test": "npm run test:react:14 && npm run test:react:15",
        "test:react:14": "npm run react:14 && npm run test:suite",
        "test:react:15": "npm run react:15 && npm run test:suite",
        "test:suite": "karma start --single-run",
        "test:watch": "karma start --auto-watch"
    },
    "version": "1.9.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module react-mdl](#apidoc.module.react-mdl)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>Badge (props)](#apidoc.element.react-mdl.Badge)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>Button ()](#apidoc.element.react-mdl.Button)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>Card (props)](#apidoc.element.react-mdl.Card)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>CardActions (props)](#apidoc.element.react-mdl.CardActions)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>CardMedia (props)](#apidoc.element.react-mdl.CardMedia)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>CardMenu (props)](#apidoc.element.react-mdl.CardMenu)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>CardText (props)](#apidoc.element.react-mdl.CardText)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>CardTitle (props)](#apidoc.element.react-mdl.CardTitle)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>Cell (props)](#apidoc.element.react-mdl.Cell)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>Checkbox ()](#apidoc.element.react-mdl.Checkbox)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>Chip (props)](#apidoc.element.react-mdl.Chip)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>ChipContact (props)](#apidoc.element.react-mdl.ChipContact)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>Content (props)](#apidoc.element.react-mdl.Content)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>DataTable (props)](#apidoc.element.react-mdl.DataTable)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>Dialog ()](#apidoc.element.react-mdl.Dialog)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>DialogActions (props)](#apidoc.element.react-mdl.DialogActions)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>DialogContent (props)](#apidoc.element.react-mdl.DialogContent)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>DialogTitle (props)](#apidoc.element.react-mdl.DialogTitle)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>Drawer (props)](#apidoc.element.react-mdl.Drawer)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>FABButton (props)](#apidoc.element.react-mdl.FABButton)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>Footer (props)](#apidoc.element.react-mdl.Footer)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>FooterDropDownSection (props)](#apidoc.element.react-mdl.FooterDropDownSection)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>FooterLinkList (props)](#apidoc.element.react-mdl.FooterLinkList)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>FooterSection (props)](#apidoc.element.react-mdl.FooterSection)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>Grid (props)](#apidoc.element.react-mdl.Grid)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>Header (props)](#apidoc.element.react-mdl.Header)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>HeaderRow (props)](#apidoc.element.react-mdl.HeaderRow)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>HeaderTabs (props)](#apidoc.element.react-mdl.HeaderTabs)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>Icon (props)](#apidoc.element.react-mdl.Icon)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>IconButton (props)](#apidoc.element.react-mdl.IconButton)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>IconToggle ()](#apidoc.element.react-mdl.IconToggle)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>Layout ()](#apidoc.element.react-mdl.Layout)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>List (props)](#apidoc.element.react-mdl.List)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>ListItem (props)](#apidoc.element.react-mdl.ListItem)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>ListItemAction (props)](#apidoc.element.react-mdl.ListItemAction)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>ListItemContent (props)](#apidoc.element.react-mdl.ListItemContent)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>MDLComponent ()](#apidoc.element.react-mdl.MDLComponent)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>Menu ()](#apidoc.element.react-mdl.Menu)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>MenuItem (props)](#apidoc.element.react-mdl.MenuItem)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>Navigation (props)](#apidoc.element.react-mdl.Navigation)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>ProgressBar ()](#apidoc.element.react-mdl.ProgressBar)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>Radio ()](#apidoc.element.react-mdl.Radio)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>RadioGroup (props)](#apidoc.element.react-mdl.RadioGroup)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>Slider ()](#apidoc.element.react-mdl.Slider)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>Snackbar (props)](#apidoc.element.react-mdl.Snackbar)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>Spacer (props)](#apidoc.element.react-mdl.Spacer)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>Spinner ()](#apidoc.element.react-mdl.Spinner)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>Switch ()](#apidoc.element.react-mdl.Switch)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>Tab (props)](#apidoc.element.react-mdl.Tab)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>TabBar (props)](#apidoc.element.react-mdl.TabBar)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>Table (props)](#apidoc.element.react-mdl.Table)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>TableHeader (props)](#apidoc.element.react-mdl.TableHeader)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>Tabs (props)](#apidoc.element.react-mdl.Tabs)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>Textfield ()](#apidoc.element.react-mdl.Textfield)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>Tooltip (props)](#apidoc.element.react-mdl.Tooltip)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>getColorClass (color, level)](#apidoc.element.react-mdl.getColorClass)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>getTextColorClass (color, level)](#apidoc.element.react-mdl.getTextColorClass)
1.  [function <span class="apidocSignatureSpan">react-mdl.</span>mdlUpgrade (Component)](#apidoc.element.react-mdl.mdlUpgrade)
1.  object <span class="apidocSignatureSpan">react-mdl.</span>ReactMDL

#### [module react-mdl.Button](#apidoc.module.react-mdl.Button)
1.  [function <span class="apidocSignatureSpan">react-mdl.Button.</span>default ()](#apidoc.element.react-mdl.Button.default)

#### [module react-mdl.Checkbox](#apidoc.module.react-mdl.Checkbox)
1.  [function <span class="apidocSignatureSpan">react-mdl.Checkbox.</span>default ()](#apidoc.element.react-mdl.Checkbox.default)

#### [module react-mdl.FABButton](#apidoc.module.react-mdl.FABButton)
1.  [function <span class="apidocSignatureSpan">react-mdl.FABButton.</span>default (props)](#apidoc.element.react-mdl.FABButton.default)

#### [module react-mdl.IconButton](#apidoc.module.react-mdl.IconButton)
1.  [function <span class="apidocSignatureSpan">react-mdl.IconButton.</span>default (props)](#apidoc.element.react-mdl.IconButton.default)

#### [module react-mdl.IconToggle](#apidoc.module.react-mdl.IconToggle)
1.  [function <span class="apidocSignatureSpan">react-mdl.IconToggle.</span>default ()](#apidoc.element.react-mdl.IconToggle.default)

#### [module react-mdl.Menu](#apidoc.module.react-mdl.Menu)
1.  [function <span class="apidocSignatureSpan">react-mdl.Menu.</span>MenuItem (props)](#apidoc.element.react-mdl.Menu.MenuItem)
1.  [function <span class="apidocSignatureSpan">react-mdl.Menu.</span>default ()](#apidoc.element.react-mdl.Menu.default)

#### [module react-mdl.ProgressBar](#apidoc.module.react-mdl.ProgressBar)
1.  [function <span class="apidocSignatureSpan">react-mdl.ProgressBar.</span>default ()](#apidoc.element.react-mdl.ProgressBar.default)

#### [module react-mdl.Radio](#apidoc.module.react-mdl.Radio)
1.  [function <span class="apidocSignatureSpan">react-mdl.Radio.</span>default ()](#apidoc.element.react-mdl.Radio.default)

#### [module react-mdl.RadioGroup](#apidoc.module.react-mdl.RadioGroup)
1.  [function <span class="apidocSignatureSpan">react-mdl.RadioGroup.</span>default (props)](#apidoc.element.react-mdl.RadioGroup.default)

#### [module react-mdl.ReactMDL](#apidoc.module.react-mdl.ReactMDL)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Badge (props)](#apidoc.element.react-mdl.ReactMDL.Badge)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Button ()](#apidoc.element.react-mdl.ReactMDL.Button)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Card (props)](#apidoc.element.react-mdl.ReactMDL.Card)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>CardActions (props)](#apidoc.element.react-mdl.ReactMDL.CardActions)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>CardMedia (props)](#apidoc.element.react-mdl.ReactMDL.CardMedia)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>CardMenu (props)](#apidoc.element.react-mdl.ReactMDL.CardMenu)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>CardText (props)](#apidoc.element.react-mdl.ReactMDL.CardText)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>CardTitle (props)](#apidoc.element.react-mdl.ReactMDL.CardTitle)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Cell (props)](#apidoc.element.react-mdl.ReactMDL.Cell)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Checkbox ()](#apidoc.element.react-mdl.ReactMDL.Checkbox)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Chip (props)](#apidoc.element.react-mdl.ReactMDL.Chip)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>ChipContact (props)](#apidoc.element.react-mdl.ReactMDL.ChipContact)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Content (props)](#apidoc.element.react-mdl.ReactMDL.Content)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>DataTable (props)](#apidoc.element.react-mdl.ReactMDL.DataTable)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Dialog ()](#apidoc.element.react-mdl.ReactMDL.Dialog)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>DialogActions (props)](#apidoc.element.react-mdl.ReactMDL.DialogActions)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>DialogContent (props)](#apidoc.element.react-mdl.ReactMDL.DialogContent)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>DialogTitle (props)](#apidoc.element.react-mdl.ReactMDL.DialogTitle)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Drawer (props)](#apidoc.element.react-mdl.ReactMDL.Drawer)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>FABButton (props)](#apidoc.element.react-mdl.ReactMDL.FABButton)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Footer (props)](#apidoc.element.react-mdl.ReactMDL.Footer)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>FooterDropDownSection (props)](#apidoc.element.react-mdl.ReactMDL.FooterDropDownSection)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>FooterLinkList (props)](#apidoc.element.react-mdl.ReactMDL.FooterLinkList)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>FooterSection (props)](#apidoc.element.react-mdl.ReactMDL.FooterSection)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Grid (props)](#apidoc.element.react-mdl.ReactMDL.Grid)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Header (props)](#apidoc.element.react-mdl.ReactMDL.Header)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>HeaderRow (props)](#apidoc.element.react-mdl.ReactMDL.HeaderRow)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>HeaderTabs (props)](#apidoc.element.react-mdl.ReactMDL.HeaderTabs)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Icon (props)](#apidoc.element.react-mdl.ReactMDL.Icon)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>IconButton (props)](#apidoc.element.react-mdl.ReactMDL.IconButton)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>IconToggle ()](#apidoc.element.react-mdl.ReactMDL.IconToggle)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Layout ()](#apidoc.element.react-mdl.ReactMDL.Layout)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>List (props)](#apidoc.element.react-mdl.ReactMDL.List)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>ListItem (props)](#apidoc.element.react-mdl.ReactMDL.ListItem)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>ListItemAction (props)](#apidoc.element.react-mdl.ReactMDL.ListItemAction)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>ListItemContent (props)](#apidoc.element.react-mdl.ReactMDL.ListItemContent)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>MDLComponent ()](#apidoc.element.react-mdl.ReactMDL.MDLComponent)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Menu ()](#apidoc.element.react-mdl.ReactMDL.Menu)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>MenuItem (props)](#apidoc.element.react-mdl.ReactMDL.MenuItem)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Navigation (props)](#apidoc.element.react-mdl.ReactMDL.Navigation)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>ProgressBar ()](#apidoc.element.react-mdl.ReactMDL.ProgressBar)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Radio ()](#apidoc.element.react-mdl.ReactMDL.Radio)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>RadioGroup (props)](#apidoc.element.react-mdl.ReactMDL.RadioGroup)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Slider ()](#apidoc.element.react-mdl.ReactMDL.Slider)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Snackbar (props)](#apidoc.element.react-mdl.ReactMDL.Snackbar)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Spacer (props)](#apidoc.element.react-mdl.ReactMDL.Spacer)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Spinner ()](#apidoc.element.react-mdl.ReactMDL.Spinner)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Switch ()](#apidoc.element.react-mdl.ReactMDL.Switch)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Tab (props)](#apidoc.element.react-mdl.ReactMDL.Tab)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>TabBar (props)](#apidoc.element.react-mdl.ReactMDL.TabBar)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Table (props)](#apidoc.element.react-mdl.ReactMDL.Table)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>TableHeader (props)](#apidoc.element.react-mdl.ReactMDL.TableHeader)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Tabs (props)](#apidoc.element.react-mdl.ReactMDL.Tabs)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Textfield ()](#apidoc.element.react-mdl.ReactMDL.Textfield)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Tooltip (props)](#apidoc.element.react-mdl.ReactMDL.Tooltip)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>getColorClass (color, level)](#apidoc.element.react-mdl.ReactMDL.getColorClass)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>getTextColorClass (color, level)](#apidoc.element.react-mdl.ReactMDL.getTextColorClass)
1.  [function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>mdlUpgrade (Component)](#apidoc.element.react-mdl.ReactMDL.mdlUpgrade)

#### [module react-mdl.Slider](#apidoc.module.react-mdl.Slider)
1.  [function <span class="apidocSignatureSpan">react-mdl.Slider.</span>default ()](#apidoc.element.react-mdl.Slider.default)

#### [module react-mdl.Spinner](#apidoc.module.react-mdl.Spinner)
1.  [function <span class="apidocSignatureSpan">react-mdl.Spinner.</span>default ()](#apidoc.element.react-mdl.Spinner.default)

#### [module react-mdl.Switch](#apidoc.module.react-mdl.Switch)
1.  [function <span class="apidocSignatureSpan">react-mdl.Switch.</span>default ()](#apidoc.element.react-mdl.Switch.default)

#### [module react-mdl.Textfield](#apidoc.module.react-mdl.Textfield)
1.  [function <span class="apidocSignatureSpan">react-mdl.Textfield.</span>default ()](#apidoc.element.react-mdl.Textfield.default)

#### [module react-mdl.Tooltip](#apidoc.module.react-mdl.Tooltip)
1.  [function <span class="apidocSignatureSpan">react-mdl.Tooltip.</span>default (props)](#apidoc.element.react-mdl.Tooltip.default)



# <a name="apidoc.module.react-mdl"></a>[module react-mdl](#apidoc.module.react-mdl)

#### <a name="apidoc.element.react-mdl.Badge"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>Badge (props)](#apidoc.element.react-mdl.Badge)
- description and source-code
```javascript
function Badge(props) {
    var children = props.children,
        className = props.className,
        text = props.text,
        overlap = props.overlap,
        noBackground = props.noBackground,
        rest = _objectWithoutProperties(props, ['children', 'className', 'text', 'overlap', 'noBackground']);

    // No badge if no children
    // TODO: In React 15, we can return null instead


    if (!_react2.default.Children.count(children)) return _react2.default.createElement('noscript', null);

    var element = typeof children === 'string' ? _react2.default.createElement(
        'span',
        null,
        children
    ) : _react2.default.Children.only(children);

    // No text -> No need of badge
    if (text === null || typeof text === 'undefined') return element;

    return _react2.default.cloneElement(element, _extends({}, rest, {
        className: (0, _classnames2.default)(className, element.props.className, 'mdl-badge', {
            'mdl-badge--overlap': !!overlap,
            'mdl-badge--no-background': !!noBackground
        }),
        'data-badge': text
    }));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.Button"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>Button ()](#apidoc.element.react-mdl.Button)
- description and source-code
```javascript
function Button() {
    _classCallCheck(this, Button);

    return _possibleConstructorReturn(this, (Button.__proto__ || Object.getPrototypeOf(Button)).apply(this, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.Card"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>Card (props)](#apidoc.element.react-mdl.Card)
- description and source-code
```javascript
function Card(props) {
    var className = props.className,
        shadow = props.shadow,
        children = props.children,
        otherProps = _objectWithoutProperties(props, ['className', 'shadow', 'children']);

    var hasShadow = typeof shadow !== 'undefined';
    var shadowLevel = (0, _clamp2.default)(shadow || 0, 0, _shadows2.default.length - 1);

    var classes = (0, _classnames2.default)('mdl-card', _defineProperty({}, _shadows2.default[shadowLevel], hasShadow), className
);

    return _react2.default.createElement(
        'div',
        _extends({ className: classes }, otherProps),
        children
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.CardActions"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>CardActions (props)](#apidoc.element.react-mdl.CardActions)
- description and source-code
```javascript
function CardActions(props) {
    var className = props.className,
        border = props.border,
        children = props.children,
        otherProps = _objectWithoutProperties(props, ['className', 'border', 'children']);

    var classes = (0, _classnames2.default)('mdl-card__actions', {
        'mdl-card--border': border
    }, className);

    return _react2.default.createElement(
        'div',
        _extends({ className: classes }, otherProps),
        children
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.CardMedia"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>CardMedia (props)](#apidoc.element.react-mdl.CardMedia)
- description and source-code
```javascript
function fn(props) {
    var className = props.className,
        children = props.children,
        otherProps = _objectWithoutProperties(props, ['className', 'children']);

    return _react2.default.createElement(element, _extends({
        className: (0, _classnames2.default)(defaultClassName, className)
    }, otherProps), children);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.CardMenu"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>CardMenu (props)](#apidoc.element.react-mdl.CardMenu)
- description and source-code
```javascript
function fn(props) {
    var className = props.className,
        children = props.children,
        otherProps = _objectWithoutProperties(props, ['className', 'children']);

    return _react2.default.createElement(element, _extends({
        className: (0, _classnames2.default)(defaultClassName, className)
    }, otherProps), children);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.CardText"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>CardText (props)](#apidoc.element.react-mdl.CardText)
- description and source-code
```javascript
function fn(props) {
    var className = props.className,
        children = props.children,
        otherProps = _objectWithoutProperties(props, ['className', 'children']);

    return _react2.default.createElement(element, _extends({
        className: (0, _classnames2.default)(defaultClassName, className)
    }, otherProps), children);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.CardTitle"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>CardTitle (props)](#apidoc.element.react-mdl.CardTitle)
- description and source-code
```javascript
function CardTitle(props) {
    var className = props.className,
        children = props.children,
        expand = props.expand,
        otherProps = _objectWithoutProperties(props, ['className', 'children', 'expand']);

    var classes = (0, _classnames2.default)('mdl-card__title', {
        'mdl-card--expand': expand
    }, className);

    var title = typeof children === 'string' ? _react2.default.createElement(
        'h2',
        { className: 'mdl-card__title-text' },
        children
    ) : children;

    return _react2.default.createElement(
        'div',
        _extends({ className: classes }, otherProps),
        title
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.Cell"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>Cell (props)](#apidoc.element.react-mdl.Cell)
- description and source-code
```javascript
function Cell(props) {
    var _classNames;

    var align = props.align,
        className = props.className,
        children = props.children,
        col = props.col,
        phone = props.phone,
        tablet = props.tablet,
        component = props.component,
        hideDesktop = props.hideDesktop,
        hidePhone = props.hidePhone,
        hideTablet = props.hideTablet,
        shadow = props.shadow,
        offset = props.offset,
        offsetDesktop = props.offsetDesktop,
        offsetTablet = props.offsetTablet,
        offsetPhone = props.offsetPhone,
        otherProps = _objectWithoutProperties(props, ['align', 'className', 'children', 'col', 'phone', 'tablet', 'component', '
hideDesktop', 'hidePhone', 'hideTablet', 'shadow', 'offset', 'offsetDesktop', 'offsetTablet', 'offsetPhone']);

    var hasShadow = isDefined(shadow);
    var shadowLevel = (0, _clamp2.default)(shadow || 0, 0, _shadows2.default.length - 1);

    var classes = (0, _classnames2.default)('mdl-cell', (_classNames = {}, _defineProperty(_classNames, 'mdl-cell--' + col + '-col
', isDefined(col)), _defineProperty(_classNames, 'mdl-cell--' + phone + '-col-phone', isDefined(phone)), _defineProperty(_classNames
, 'mdl-cell--' + tablet + '-col-tablet', isDefined(tablet)), _defineProperty(_classNames, 'mdl-cell--' + align, isDefined(align)),
_defineProperty(_classNames, 'mdl-cell--' + offset + '-offset', isDefined(offset)), _defineProperty(_classNames, 'mdl-cell--' +
offsetDesktop + '-offset-desktop', isDefined(offsetDesktop)), _defineProperty(_classNames, 'mdl-cell--' + offsetTablet + '-offset
-tablet', isDefined(offsetTablet)), _defineProperty(_classNames, 'mdl-cell--' + offsetPhone + '-offset-phone', isDefined(offsetPhone
)), _defineProperty(_classNames, 'mdl-cell--hide-desktop', hideDesktop), _defineProperty(_classNames, 'mdl-cell--hide-phone', hidePhone
), _defineProperty(_classNames, 'mdl-cell--hide-tablet', hideTablet), _defineProperty(_classNames, _shadows2.default[shadowLevel
], hasShadow), _classNames), className);

    return _react2.default.createElement(component || 'div', _extends({
        className: classes
    }, otherProps), children);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.Checkbox"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>Checkbox ()](#apidoc.element.react-mdl.Checkbox)
- description and source-code
```javascript
function Checkbox() {
    _classCallCheck(this, Checkbox);

    return _possibleConstructorReturn(this, (Checkbox.__proto__ || Object.getPrototypeOf(Checkbox)).apply(this, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.Chip"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>Chip (props)](#apidoc.element.react-mdl.Chip)
- description and source-code
```javascript
function Chip(props) {
    var className = props.className,
        onClick = props.onClick,
        onClose = props.onClose,
        children = props.children,
        otherProps = _objectWithoutProperties(props, ['className', 'onClick', 'onClose', 'children']);

    var childrenArray = _react2.default.Children.toArray(children);
    var contactIndex = childrenArray.findIndex(function (c) {
        return c.type === ChipContact;
    });

    var chipContent = [];

    if (contactIndex >= 0) {
        chipContent.push(childrenArray[contactIndex], _react2.default.createElement(
            ChipText,
            { key: 'text' },
            childrenArray.slice(0, contactIndex).concat(childrenArray.slice(contactIndex + 1))
        ));
    } else {
        chipContent.push(_react2.default.createElement(
            ChipText,
            { key: 'text' },
            children
        ));
    }

    if (onClose) {
        chipContent.push(_react2.default.createElement(
            'button',
            { key: 'btn', type: 'button', className: 'mdl-chip__action', onClick: onClose },
            _react2.default.createElement(_Icon2.default, { name: 'cancel' })
        ));
    }

    var elt = onClick ? 'button' : 'span';

    return _react2.default.createElement(elt, _extends({
        className: (0, _classnames2.default)('mdl-chip', {
            'mdl-chip--contact': contactIndex > -1,
            'mdl-chip--deletable': !!onClose
        }, className),
        type: onClick ? 'button' : null,
        onClick: onClick
    }, otherProps), chipContent);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ChipContact"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>ChipContact (props)](#apidoc.element.react-mdl.ChipContact)
- description and source-code
```javascript
function fn(props) {
    var className = props.className,
        children = props.children,
        otherProps = _objectWithoutProperties(props, ['className', 'children']);

    return _react2.default.createElement(element, _extends({
        className: (0, _classnames2.default)(defaultClassName, className)
    }, otherProps), children);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.Content"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>Content (props)](#apidoc.element.react-mdl.Content)
- description and source-code
```javascript
function Content(props) {
    var children = props.children,
        className = props.className,
        component = props.component,
        otherProps = _objectWithoutProperties(props, ['children', 'className', 'component']);

    var classes = (0, _classnames2.default)('mdl-layout__content', className);

    return _react2.default.createElement(component || 'div', _extends({
        className: classes
    }, otherProps), children);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.DataTable"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>DataTable (props)](#apidoc.element.react-mdl.DataTable)
- description and source-code
```javascript
function Sortable(props) {
    _classCallCheck(this, Sortable);

    var _this = _possibleConstructorReturn(this, (Sortable.__proto__ || Object.getPrototypeOf(Sortable)).call(this, props));

    _this.handleClickColumn = _this.handleClickColumn.bind(_this);

    if (props.sortable) {
        _this.state = initState(props);
    }
    return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.Dialog"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>Dialog ()](#apidoc.element.react-mdl.Dialog)
- description and source-code
```javascript
function Dialog() {
    _classCallCheck(this, Dialog);

    return _possibleConstructorReturn(this, (Dialog.__proto__ || Object.getPrototypeOf(Dialog)).apply(this, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.DialogActions"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>DialogActions (props)](#apidoc.element.react-mdl.DialogActions)
- description and source-code
```javascript
function DialogActions(props) {
    var className = props.className,
        fullWidth = props.fullWidth,
        children = props.children,
        otherProps = _objectWithoutProperties(props, ['className', 'fullWidth', 'children']);

    var classes = (0, _classnames2.default)('mdl-dialog__actions', {
        'mdl-dialog__actions--full-width': fullWidth
    }, className);

    return _react2.default.createElement(
        'div',
        _extends({ className: classes }, otherProps),
        children
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.DialogContent"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>DialogContent (props)](#apidoc.element.react-mdl.DialogContent)
- description and source-code
```javascript
function fn(props) {
    var className = props.className,
        children = props.children,
        otherProps = _objectWithoutProperties(props, ['className', 'children']);

    return _react2.default.createElement(element, _extends({
        className: (0, _classnames2.default)(defaultClassName, className)
    }, otherProps), children);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.DialogTitle"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>DialogTitle (props)](#apidoc.element.react-mdl.DialogTitle)
- description and source-code
```javascript
function DialogTitle(props) {
    var className = props.className,
        component = props.component,
        children = props.children,
        otherProps = _objectWithoutProperties(props, ['className', 'component', 'children']);

    return _react2.default.createElement(component || 'h4', _extends({
        className: (0, _classnames2.default)('mdl-dialog__title', className)
    }, otherProps), children);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.Drawer"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>Drawer (props)](#apidoc.element.react-mdl.Drawer)
- description and source-code
```javascript
function Drawer(props) {
    var className = props.className,
        title = props.title,
        children = props.children,
        otherProps = _objectWithoutProperties(props, ['className', 'title', 'children']);

    var classes = (0, _classnames2.default)('mdl-layout__drawer', className);

    return _react2.default.createElement(
        'div',
        _extends({ className: classes }, otherProps),
        title ? _react2.default.createElement(
            'span',
            { className: 'mdl-layout-title' },
            title
        ) : null,
        children
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.FABButton"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>FABButton (props)](#apidoc.element.react-mdl.FABButton)
- description and source-code
```javascript
function FABButton(props) {
    var mini = props.mini,
        className = props.className,
        children = props.children,
        otherProps = _objectWithoutProperties(props, ['mini', 'className', 'children']);

    var classes = (0, _classnames2.default)('mdl-button--fab', {
        'mdl-button--mini-fab': mini
    }, className);

    return _react2.default.createElement(
        _Button2.default,
        _extends({ className: classes }, otherProps),
        children
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.Footer"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>Footer (props)](#apidoc.element.react-mdl.Footer)
- description and source-code
```javascript
function Footer(props) {
    var className = props.className,
        size = props.size,
        children = props.children,
        otherProps = _objectWithoutProperties(props, ['className', 'size', 'children']);

    var classes = (0, _classnames2.default)(_defineProperty({}, 'mdl-' + size + '-footer', true), className);

    return _react2.default.createElement(
        'footer',
        _extends({ className: classes }, otherProps),
        (0, _cloneChildren2.default)(children, { size: size })
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.FooterDropDownSection"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>FooterDropDownSection (props)](#apidoc.element.react-mdl.FooterDropDownSection)
- description and source-code
```javascript
function DropDownSection(props) {
    var className = props.className,
        size = props.size,
        title = props.title,
        children = props.children,
        otherProps = _objectWithoutProperties(props, ['className', 'size', 'title', 'children']);

    var classes = (0, _classnames2.default)(_defineProperty({}, 'mdl-' + size + '-footer__drop-down-section', true), className);

    return _react2.default.createElement(
        'div',
        _extends({ className: classes }, otherProps),
        _react2.default.createElement('input', { className: 'mdl-' + size + '-footer__heading-checkbox', type: 'checkbox', defaultChecked
: true }),
        _react2.default.createElement(
            'h1',
            { className: 'mdl-' + size + '-footer__heading' },
            title
        ),
        (0, _cloneChildren2.default)(children, { size: size })
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.FooterLinkList"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>FooterLinkList (props)](#apidoc.element.react-mdl.FooterLinkList)
- description and source-code
```javascript
function LinkList(props) {
    var className = props.className,
        size = props.size,
        children = props.children,
        otherProps = _objectWithoutProperties(props, ['className', 'size', 'children']);

    var classes = (0, _classnames2.default)(_defineProperty({}, 'mdl-' + size + '-footer__link-list', true), className);

    return _react2.default.createElement(
        'ul',
        _extends({ className: classes }, otherProps),
        _react2.default.Children.map(children, function (child) {
            return _react2.default.createElement(
                'li',
                null,
                child
            );
        })
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.FooterSection"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>FooterSection (props)](#apidoc.element.react-mdl.FooterSection)
- description and source-code
```javascript
function Section(props) {
    var className = props.className,
        logo = props.logo,
        size = props.size,
        type = props.type,
        children = props.children,
        otherProps = _objectWithoutProperties(props, ['className', 'logo', 'size', 'type', 'children']);

    var classes = (0, _classnames2.default)(_defineProperty({}, 'mdl-' + size + '-footer__' + type + '-section', true), className
);

    return _react2.default.createElement(
        'div',
        _extends({ className: classes }, otherProps),
        logo ? _react2.default.createElement(
            'div',
            { className: 'mdl-logo' },
            logo
        ) : null,
        (0, _cloneChildren2.default)(children, { size: size })
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.Grid"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>Grid (props)](#apidoc.element.react-mdl.Grid)
- description and source-code
```javascript
function Grid(props) {
    var noSpacing = props.noSpacing,
        className = props.className,
        children = props.children,
        component = props.component,
        shadow = props.shadow,
        otherProps = _objectWithoutProperties(props, ['noSpacing', 'className', 'children', 'component', 'shadow']);

    var hasShadow = typeof shadow !== 'undefined';
    var shadowLevel = (0, _clamp2.default)(shadow || 0, 0, _shadows2.default.length - 1);

    var classes = (0, _classnames2.default)('mdl-grid', _defineProperty({
        'mdl-grid--no-spacing': noSpacing
    }, _shadows2.default[shadowLevel], hasShadow), className);

    return _react2.default.createElement(component || 'div', _extends({
        className: classes
    }, otherProps), children);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.Header"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>Header (props)](#apidoc.element.react-mdl.Header)
- description and source-code
```javascript
function Header(props) {
    var className = props.className,
        scroll = props.scroll,
        seamed = props.seamed,
        title = props.title,
        transparent = props.transparent,
        waterfall = props.waterfall,
        hideTop = props.hideTop,
        hideSpacer = props.hideSpacer,
        children = props.children,
        otherProps = _objectWithoutProperties(props, ['className', 'scroll', 'seamed', 'title', 'transparent', 'waterfall', 'hideTop
', 'hideSpacer', 'children']);

    var classes = (0, _classnames2.default)('mdl-layout__header', {
        'mdl-layout__header--scroll': scroll,
        'mdl-layout__header--seamed': seamed,
        'mdl-layout__header--transparent': transparent,
        'mdl-layout__header--waterfall': waterfall,
        'mdl-layout__header--waterfall-hide-top': waterfall && hideTop
    }, className);

    var isRowOrTab = false;
    _react2.default.Children.forEach(children, function (child) {
        if (child && (child.type === _HeaderRow2.default || child.type === _HeaderTabs2.default)) {
            isRowOrTab = true;
        }
    });

    return _react2.default.createElement(
        'header',
        _extends({ className: classes }, otherProps),
        isRowOrTab ? children : _react2.default.createElement(
            _HeaderRow2.default,
            { title: title, hideSpacer: hideSpacer },
            children
        )
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.HeaderRow"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>HeaderRow (props)](#apidoc.element.react-mdl.HeaderRow)
- description and source-code
```javascript
function HeaderRow(props) {
    var className = props.className,
        title = props.title,
        children = props.children,
        hideSpacer = props.hideSpacer,
        otherProps = _objectWithoutProperties(props, ['className', 'title', 'children', 'hideSpacer']);

    var classes = (0, _classnames2.default)('mdl-layout__header-row', className);

    return _react2.default.createElement(
        'div',
        _extends({ className: classes }, otherProps),
        title && _react2.default.createElement(
            'span',
            { className: 'mdl-layout-title' },
            title
        ),
        title && !hideSpacer && _react2.default.createElement(_Spacer2.default, null),
        children
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.HeaderTabs"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>HeaderTabs (props)](#apidoc.element.react-mdl.HeaderTabs)
- description and source-code
```javascript
function patchedComponent(props) {
    return React.createElement(
        _MDLComponent2.default,
        { recursive: recursive },
        component(props)
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.Icon"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>Icon (props)](#apidoc.element.react-mdl.Icon)
- description and source-code
```javascript
function Icon(props) {
    var className = props.className,
        name = props.name,
        otherProps = _objectWithoutProperties(props, ['className', 'name']);

    var classes = (0, _classnames2.default)('material-icons', className);

    return _react2.default.createElement(
        'i',
        _extends({ className: classes }, otherProps),
        name
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.IconButton"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>IconButton (props)](#apidoc.element.react-mdl.IconButton)
- description and source-code
```javascript
function IconButton(props) {
    var className = props.className,
        name = props.name,
        otherProps = _objectWithoutProperties(props, ['className', 'name']);

    var classes = (0, _classnames2.default)('mdl-button--icon', className);

    return _react2.default.createElement(
        _Button2.default,
        _extends({ className: classes }, otherProps),
        _react2.default.createElement(_Icon2.default, { name: name })
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.IconToggle"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>IconToggle ()](#apidoc.element.react-mdl.IconToggle)
- description and source-code
```javascript
function IconToggle() {
    _classCallCheck(this, IconToggle);

    return _possibleConstructorReturn(this, (IconToggle.__proto__ || Object.getPrototypeOf(IconToggle)).apply(this, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.Layout"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>Layout ()](#apidoc.element.react-mdl.Layout)
- description and source-code
```javascript
function Layout() {
    _classCallCheck(this, Layout);

    return _possibleConstructorReturn(this, (Layout.__proto__ || Object.getPrototypeOf(Layout)).apply(this, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.List"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>List (props)](#apidoc.element.react-mdl.List)
- description and source-code
```javascript
function fn(props) {
    var className = props.className,
        children = props.children,
        otherProps = _objectWithoutProperties(props, ['className', 'children']);

    return _react2.default.createElement(element, _extends({
        className: (0, _classnames2.default)(defaultClassName, className)
    }, otherProps), children);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ListItem"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>ListItem (props)](#apidoc.element.react-mdl.ListItem)
- description and source-code
```javascript
function ListItem(props) {
    var className = props.className,
        twoLine = props.twoLine,
        threeLine = props.threeLine,
        otherProps = _objectWithoutProperties(props, ['className', 'twoLine', 'threeLine']);

    var classes = (0, _classnames2.default)('mdl-list__item', {
        'mdl-list__item--two-line': twoLine && !threeLine,
        'mdl-list__item--three-line': !twoLine && threeLine
    }, className);

    var children = _react.Children.map(otherProps.children, function (child) {
        if (typeof child === 'string') {
            return _react2.default.createElement(
                _ListItemContent2.default,
                null,
                child
            );
        }
        if (child.type === _ListItemContent2.default) {
            return (0, _react.cloneElement)(child, {
                useBodyClass: !!threeLine
            });
        }
        return child;
    });

    return _react2.default.createElement(
        'li',
        _extends({ className: classes }, otherProps),
        children
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ListItemAction"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>ListItemAction (props)](#apidoc.element.react-mdl.ListItemAction)
- description and source-code
```javascript
function ListItemAction(props) {
    var children = props.children,
        className = props.className,
        info = props.info,
        otherProps = _objectWithoutProperties(props, ['children', 'className', 'info']);

    var classes = (0, _classnames2.default)('mdl-list__item-secondary-content', className);

    return _react2.default.createElement(
        'span',
        _extends({ className: classes }, otherProps),
        info && _react2.default.createElement(
            'span',
            { className: 'mdl-list__item-secondary-info' },
            info
        ),
        _react2.default.createElement(
            'span',
            { className: 'mdl-list__item-secondary-action' },
            children
        )
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ListItemContent"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>ListItemContent (props)](#apidoc.element.react-mdl.ListItemContent)
- description and source-code
```javascript
function ListItemContent(props) {
    var avatar = props.avatar,
        children = props.children,
        className = props.className,
        icon = props.icon,
        subtitle = props.subtitle,
        useBodyClass = props.useBodyClass,
        otherProps = _objectWithoutProperties(props, ['avatar', 'children', 'className', 'icon', 'subtitle', 'useBodyClass']);

    var classes = (0, _classnames2.default)('mdl-list__item-primary-content', className);
    var subtitleClassName = useBodyClass ? 'mdl-list__item-text-body' : 'mdl-list__item-sub-title';

    var iconElement = null;
    if (icon) {
        iconElement = createIcon('icon', icon);
    } else if (avatar) {
        iconElement = createIcon('avatar', avatar);
    }

    return _react2.default.createElement(
        'span',
        _extends({ className: classes }, otherProps),
        iconElement,
        _react2.default.createElement(
            'span',
            null,
            children
        ),
        subtitle && _react2.default.createElement(
            'span',
            { className: subtitleClassName },
            subtitle
        )
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.MDLComponent"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>MDLComponent ()](#apidoc.element.react-mdl.MDLComponent)
- description and source-code
```javascript
function MDLComponent() {
    _classCallCheck(this, MDLComponent);

    return _possibleConstructorReturn(this, (MDLComponent.__proto__ || Object.getPrototypeOf(MDLComponent)).apply(this, arguments
));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.Menu"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>Menu ()](#apidoc.element.react-mdl.Menu)
- description and source-code
```javascript
function Menu() {
    _classCallCheck(this, Menu);

    return _possibleConstructorReturn(this, (Menu.__proto__ || Object.getPrototypeOf(Menu)).apply(this, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.MenuItem"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>MenuItem (props)](#apidoc.element.react-mdl.MenuItem)
- description and source-code
```javascript
function fn(props) {
    var className = props.className,
        children = props.children,
        otherProps = _objectWithoutProperties(props, ['className', 'children']);

    return _react2.default.createElement(element, _extends({
        className: (0, _classnames2.default)(defaultClassName, className)
    }, otherProps), children);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.Navigation"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>Navigation (props)](#apidoc.element.react-mdl.Navigation)
- description and source-code
```javascript
function Navigation(props) {
    var className = props.className,
        children = props.children,
        otherProps = _objectWithoutProperties(props, ['className', 'children']);

    var classes = (0, _classnames2.default)('mdl-navigation', className);

    return _react2.default.createElement(
        'nav',
        _extends({ className: classes }, otherProps),
        (0, _cloneChildren2.default)(children, function (child) {
            return {
                className: (0, _classnames2.default)({ 'mdl-navigation__link': child.type !== _Spacer2.default }, child.props.className
)
            };
        })
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ProgressBar"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>ProgressBar ()](#apidoc.element.react-mdl.ProgressBar)
- description and source-code
```javascript
function ProgressBar() {
    _classCallCheck(this, ProgressBar);

    return _possibleConstructorReturn(this, (ProgressBar.__proto__ || Object.getPrototypeOf(ProgressBar)).apply(this, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.Radio"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>Radio ()](#apidoc.element.react-mdl.Radio)
- description and source-code
```javascript
function Radio() {
    _classCallCheck(this, Radio);

    return _possibleConstructorReturn(this, (Radio.__proto__ || Object.getPrototypeOf(Radio)).apply(this, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.RadioGroup"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>RadioGroup (props)](#apidoc.element.react-mdl.RadioGroup)
- description and source-code
```javascript
function RadioGroup(props) {
    var name = props.name,
        value = props.value,
        children = props.children,
        container = props.container,
        childContainer = props.childContainer,
        onChange = props.onChange,
        otherProps = _objectWithoutProperties(props, ['name', 'value', 'children', 'container', 'childContainer', 'onChange']);

    var hasOnChange = typeof onChange === 'function';
    var checked = hasOnChange ? 'checked' : 'defaultChecked';

    return _react2.default.createElement(container, otherProps, _react2.default.Children.map(children, function (child) {
        var _extends2;

        var clonedChild = _react2.default.cloneElement(child, _extends((_extends2 = {}, _defineProperty(_extends2, checked, child
.props.value === value), _defineProperty(_extends2, 'name', name), _defineProperty(_extends2, 'onChange', onChange), _extends2),
otherProps));

        return childContainer ? _react2.default.createElement(childContainer, {}, clonedChild) : clonedChild;
    }));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.Slider"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>Slider ()](#apidoc.element.react-mdl.Slider)
- description and source-code
```javascript
function Slider() {
    _classCallCheck(this, Slider);

    return _possibleConstructorReturn(this, (Slider.__proto__ || Object.getPrototypeOf(Slider)).apply(this, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.Snackbar"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>Snackbar (props)](#apidoc.element.react-mdl.Snackbar)
- description and source-code
```javascript
function Snackbar(props) {
    _classCallCheck(this, Snackbar);

    var _this = _possibleConstructorReturn(this, (Snackbar.__proto__ || Object.getPrototypeOf(Snackbar)).call(this, props));

    _this.clearTimer = _this.clearTimer.bind(_this);
    _this.timeoutId = null;
    _this.clearTimeoutId = null;
    _this.state = {
        open: false
    };
    return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.Spacer"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>Spacer (props)](#apidoc.element.react-mdl.Spacer)
- description and source-code
```javascript
function fn(props) {
    var className = props.className,
        children = props.children,
        otherProps = _objectWithoutProperties(props, ['className', 'children']);

    return _react2.default.createElement(element, _extends({
        className: (0, _classnames2.default)(defaultClassName, className)
    }, otherProps), children);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.Spinner"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>Spinner ()](#apidoc.element.react-mdl.Spinner)
- description and source-code
```javascript
function Spinner() {
    _classCallCheck(this, Spinner);

    return _possibleConstructorReturn(this, (Spinner.__proto__ || Object.getPrototypeOf(Spinner)).apply(this, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.Switch"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>Switch ()](#apidoc.element.react-mdl.Switch)
- description and source-code
```javascript
function Switch() {
    _classCallCheck(this, Switch);

    return _possibleConstructorReturn(this, (Switch.__proto__ || Object.getPrototypeOf(Switch)).apply(this, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.Tab"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>Tab (props)](#apidoc.element.react-mdl.Tab)
- description and source-code
```javascript
function Tab(props) {
    var _classNames;

    var active = props.active,
        className = props.className,
        component = props.component,
        children = props.children,
        cssPrefix = props.cssPrefix,
        onTabClick = props.onTabClick,
        style = props.style,
        tabId = props.tabId,
        otherProps = _objectWithoutProperties(props, ['active', 'className', 'component', 'children', 'cssPrefix', 'onTabClick', '
style', 'tabId']);

    var classes = (0, _classnames2.default)((_classNames = {}, _defineProperty(_classNames, cssPrefix + '__tab', true), _defineProperty
(_classNames, 'is-active', active), _classNames), className);

    style.cursor = 'pointer';

    return _react2.default.createElement(component || 'a', _extends({
        className: classes,
        onClick: function onClick() {
            return onTabClick(tabId);
        },
        style: style
    }, otherProps), children);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.TabBar"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>TabBar (props)](#apidoc.element.react-mdl.TabBar)
- description and source-code
```javascript
function TabBar(props) {
    _classCallCheck(this, TabBar);

    var _this = _possibleConstructorReturn(this, (TabBar.__proto__ || Object.getPrototypeOf(TabBar)).call(this, props));

    _this.handleClickTab = _this.handleClickTab.bind(_this);
    return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.Table"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>Table (props)](#apidoc.element.react-mdl.Table)
- description and source-code
```javascript
function Sortable(props) {
    _classCallCheck(this, Sortable);

    var _this = _possibleConstructorReturn(this, (Sortable.__proto__ || Object.getPrototypeOf(Sortable)).call(this, props));

    _this.handleClickColumn = _this.handleClickColumn.bind(_this);

    if (props.sortable) {
        _this.state = initState(props);
    }
    return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.TableHeader"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>TableHeader (props)](#apidoc.element.react-mdl.TableHeader)
- description and source-code
```javascript
function TableHeader(props) {
    var className = props.className,
        name = props.name,
        numeric = props.numeric,
        onClick = props.onClick,
        nosort = props.nosort,
        tooltip = props.tooltip,
        children = props.children,
        otherProps = _objectWithoutProperties(props, ['className', 'name', 'numeric', 'onClick', 'nosort', 'tooltip', 'children']);

    // remove unwanted props
    // see https://github.com/Hacker0x01/react-datepicker/issues/517#issuecomment-230171426


    delete otherProps.cellFormatter;
    delete otherProps.sortFn;

    var classes = (0, _classnames2.default)({
        'mdl-data-table__cell--non-numeric': !numeric
    }, className);

    var clickFn = !nosort && onClick ? function (e) {
        return onClick(e, name);
    } : null;

    return _react2.default.createElement(
        'th',
        _extends({ className: classes, onClick: clickFn }, otherProps),
        !!tooltip ? _react2.default.createElement(
            _Tooltip2.default,
            { label: tooltip },
            children
        ) : children
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.Tabs"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>Tabs (props)](#apidoc.element.react-mdl.Tabs)
- description and source-code
```javascript
function patchedComponent(props) {
    return React.createElement(
        _MDLComponent2.default,
        { recursive: recursive },
        component(props)
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.Textfield"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>Textfield ()](#apidoc.element.react-mdl.Textfield)
- description and source-code
```javascript
function Textfield() {
    _classCallCheck(this, Textfield);

    return _possibleConstructorReturn(this, (Textfield.__proto__ || Object.getPrototypeOf(Textfield)).apply(this, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.Tooltip"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>Tooltip (props)](#apidoc.element.react-mdl.Tooltip)
- description and source-code
```javascript
function Tooltip(props) {
    var label = props.label,
        large = props.large,
        children = props.children,
        position = props.position,
        otherProps = _objectWithoutProperties(props, ['label', 'large', 'children', 'position']);

    var id = Math.random().toString(36).substr(2);

    var newLabel = typeof label === 'string' ? _react2.default.createElement(
        'span',
        null,
        label
    ) : label;

    var element = void 0;
    if (typeof children === 'string') {
        element = _react2.default.createElement(
            'span',
            null,
            children
        );
    } else {
        element = _react2.default.Children.only(children);
    }

    return _react2.default.createElement(
        'div',
        _extends({ style: { display: 'inline-block' } }, otherProps),
        _react2.default.cloneElement(element, { id: id }),
        _react2.default.createElement(
            _MDLComponent2.default,
            null,
            _react2.default.cloneElement(newLabel, {
                htmlFor: id,
                className: (0, _classnames2.default)('mdl-tooltip', _defineProperty({
                    'mdl-tooltip--large': large
                }, 'mdl-tooltip--' + position, typeof position !== 'undefined'))
            })
        )
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.getColorClass"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>getColorClass (color, level)](#apidoc.element.react-mdl.getColorClass)
- description and source-code
```javascript
function getColorClass(color, level) {
    var lvlClass = level ? '-' + level : '';
    return 'mdl-color--' + color + lvlClass;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.getTextColorClass"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>getTextColorClass (color, level)](#apidoc.element.react-mdl.getTextColorClass)
- description and source-code
```javascript
function getTextColorClass(color, level) {
    var lvlClass = level ? '-' + level : '';
    return 'mdl-color-text--' + color + lvlClass;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.mdlUpgrade"></a>[function <span class="apidocSignatureSpan">react-mdl.</span>mdlUpgrade (Component)](#apidoc.element.react-mdl.mdlUpgrade)
- description and source-code
```javascript
mdlUpgrade = function (Component) {
    var recursive = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : false;
    return Component.prototype && Component.prototype.isReactComponent ? patchComponentClass(Component, recursive) : patchSFC(Component
, recursive);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-mdl.Button"></a>[module react-mdl.Button](#apidoc.module.react-mdl.Button)

#### <a name="apidoc.element.react-mdl.Button.default"></a>[function <span class="apidocSignatureSpan">react-mdl.Button.</span>default ()](#apidoc.element.react-mdl.Button.default)
- description and source-code
```javascript
function Button() {
    _classCallCheck(this, Button);

    return _possibleConstructorReturn(this, (Button.__proto__ || Object.getPrototypeOf(Button)).apply(this, arguments));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-mdl.Checkbox"></a>[module react-mdl.Checkbox](#apidoc.module.react-mdl.Checkbox)

#### <a name="apidoc.element.react-mdl.Checkbox.default"></a>[function <span class="apidocSignatureSpan">react-mdl.Checkbox.</span>default ()](#apidoc.element.react-mdl.Checkbox.default)
- description and source-code
```javascript
function Checkbox() {
    _classCallCheck(this, Checkbox);

    return _possibleConstructorReturn(this, (Checkbox.__proto__ || Object.getPrototypeOf(Checkbox)).apply(this, arguments));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-mdl.FABButton"></a>[module react-mdl.FABButton](#apidoc.module.react-mdl.FABButton)

#### <a name="apidoc.element.react-mdl.FABButton.default"></a>[function <span class="apidocSignatureSpan">react-mdl.FABButton.</span>default (props)](#apidoc.element.react-mdl.FABButton.default)
- description and source-code
```javascript
function FABButton(props) {
    var mini = props.mini,
        className = props.className,
        children = props.children,
        otherProps = _objectWithoutProperties(props, ['mini', 'className', 'children']);

    var classes = (0, _classnames2.default)('mdl-button--fab', {
        'mdl-button--mini-fab': mini
    }, className);

    return _react2.default.createElement(
        _Button2.default,
        _extends({ className: classes }, otherProps),
        children
    );
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-mdl.IconButton"></a>[module react-mdl.IconButton](#apidoc.module.react-mdl.IconButton)

#### <a name="apidoc.element.react-mdl.IconButton.default"></a>[function <span class="apidocSignatureSpan">react-mdl.IconButton.</span>default (props)](#apidoc.element.react-mdl.IconButton.default)
- description and source-code
```javascript
function IconButton(props) {
    var className = props.className,
        name = props.name,
        otherProps = _objectWithoutProperties(props, ['className', 'name']);

    var classes = (0, _classnames2.default)('mdl-button--icon', className);

    return _react2.default.createElement(
        _Button2.default,
        _extends({ className: classes }, otherProps),
        _react2.default.createElement(_Icon2.default, { name: name })
    );
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-mdl.IconToggle"></a>[module react-mdl.IconToggle](#apidoc.module.react-mdl.IconToggle)

#### <a name="apidoc.element.react-mdl.IconToggle.default"></a>[function <span class="apidocSignatureSpan">react-mdl.IconToggle.</span>default ()](#apidoc.element.react-mdl.IconToggle.default)
- description and source-code
```javascript
function IconToggle() {
    _classCallCheck(this, IconToggle);

    return _possibleConstructorReturn(this, (IconToggle.__proto__ || Object.getPrototypeOf(IconToggle)).apply(this, arguments));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-mdl.Menu"></a>[module react-mdl.Menu](#apidoc.module.react-mdl.Menu)

#### <a name="apidoc.element.react-mdl.Menu.MenuItem"></a>[function <span class="apidocSignatureSpan">react-mdl.Menu.</span>MenuItem (props)](#apidoc.element.react-mdl.Menu.MenuItem)
- description and source-code
```javascript
function fn(props) {
    var className = props.className,
        children = props.children,
        otherProps = _objectWithoutProperties(props, ['className', 'children']);

    return _react2.default.createElement(element, _extends({
        className: (0, _classnames2.default)(defaultClassName, className)
    }, otherProps), children);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.Menu.default"></a>[function <span class="apidocSignatureSpan">react-mdl.Menu.</span>default ()](#apidoc.element.react-mdl.Menu.default)
- description and source-code
```javascript
function Menu() {
    _classCallCheck(this, Menu);

    return _possibleConstructorReturn(this, (Menu.__proto__ || Object.getPrototypeOf(Menu)).apply(this, arguments));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-mdl.ProgressBar"></a>[module react-mdl.ProgressBar](#apidoc.module.react-mdl.ProgressBar)

#### <a name="apidoc.element.react-mdl.ProgressBar.default"></a>[function <span class="apidocSignatureSpan">react-mdl.ProgressBar.</span>default ()](#apidoc.element.react-mdl.ProgressBar.default)
- description and source-code
```javascript
function ProgressBar() {
    _classCallCheck(this, ProgressBar);

    return _possibleConstructorReturn(this, (ProgressBar.__proto__ || Object.getPrototypeOf(ProgressBar)).apply(this, arguments));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-mdl.Radio"></a>[module react-mdl.Radio](#apidoc.module.react-mdl.Radio)

#### <a name="apidoc.element.react-mdl.Radio.default"></a>[function <span class="apidocSignatureSpan">react-mdl.Radio.</span>default ()](#apidoc.element.react-mdl.Radio.default)
- description and source-code
```javascript
function Radio() {
    _classCallCheck(this, Radio);

    return _possibleConstructorReturn(this, (Radio.__proto__ || Object.getPrototypeOf(Radio)).apply(this, arguments));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-mdl.RadioGroup"></a>[module react-mdl.RadioGroup](#apidoc.module.react-mdl.RadioGroup)

#### <a name="apidoc.element.react-mdl.RadioGroup.default"></a>[function <span class="apidocSignatureSpan">react-mdl.RadioGroup.</span>default (props)](#apidoc.element.react-mdl.RadioGroup.default)
- description and source-code
```javascript
function RadioGroup(props) {
    var name = props.name,
        value = props.value,
        children = props.children,
        container = props.container,
        childContainer = props.childContainer,
        onChange = props.onChange,
        otherProps = _objectWithoutProperties(props, ['name', 'value', 'children', 'container', 'childContainer', 'onChange']);

    var hasOnChange = typeof onChange === 'function';
    var checked = hasOnChange ? 'checked' : 'defaultChecked';

    return _react2.default.createElement(container, otherProps, _react2.default.Children.map(children, function (child) {
        var _extends2;

        var clonedChild = _react2.default.cloneElement(child, _extends((_extends2 = {}, _defineProperty(_extends2, checked, child
.props.value === value), _defineProperty(_extends2, 'name', name), _defineProperty(_extends2, 'onChange', onChange), _extends2),
otherProps));

        return childContainer ? _react2.default.createElement(childContainer, {}, clonedChild) : clonedChild;
    }));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-mdl.ReactMDL"></a>[module react-mdl.ReactMDL](#apidoc.module.react-mdl.ReactMDL)

#### <a name="apidoc.element.react-mdl.ReactMDL.Badge"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Badge (props)](#apidoc.element.react-mdl.ReactMDL.Badge)
- description and source-code
```javascript
function Badge(props) {
	    var children = props.children,
	        className = props.className,
	        text = props.text,
	        overlap = props.overlap,
	        noBackground = props.noBackground,
	        rest = _objectWithoutProperties(props, ['children', 'className', 'text', 'overlap', 'noBackground']);
	
	    // No badge if no children
	    // TODO: In React 15, we can return null instead
	
	
	    if (!_react2.default.Children.count(children)) return _react2.default.createElement('noscript', null);
	
	    var element = typeof children === 'string' ? _react2.default.createElement(
	        'span',
	        null,
	        children
	    ) : _react2.default.Children.only(children);
	
	    // No text -> No need of badge
	    if (text === null || typeof text === 'undefined') return element;
	
	    return _react2.default.cloneElement(element, _extends({}, rest, {
	        className: (0, _classnames2.default)(className, element.props.className, 'mdl-badge', {
	            'mdl-badge--overlap': !!overlap,
	            'mdl-badge--no-background': !!noBackground
	        }),
	        'data-badge': text
	    }));
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.Button"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Button ()](#apidoc.element.react-mdl.ReactMDL.Button)
- description and source-code
```javascript
function Button() {
	        _classCallCheck(this, Button);
	
	        return _possibleConstructorReturn(this, (Button.__proto__ || Object.getPrototypeOf(Button)).apply(this, arguments));
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.Card"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Card (props)](#apidoc.element.react-mdl.ReactMDL.Card)
- description and source-code
```javascript
function Card(props) {
	    var className = props.className,
	        shadow = props.shadow,
	        children = props.children,
	        otherProps = _objectWithoutProperties(props, ['className', 'shadow', 'children']);
	
	    var hasShadow = typeof shadow !== 'undefined';
	    var shadowLevel = (0, _clamp2.default)(shadow || 0, 0, _shadows2.default.length - 1);
	
	    var classes = (0, _classnames2.default)('mdl-card', _defineProperty({}, _shadows2.default[shadowLevel], hasShadow), className
);
	
	    return _react2.default.createElement(
	        'div',
	        _extends({ className: classes }, otherProps),
	        children
	    );
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.CardActions"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>CardActions (props)](#apidoc.element.react-mdl.ReactMDL.CardActions)
- description and source-code
```javascript
function CardActions(props) {
	    var className = props.className,
	        border = props.border,
	        children = props.children,
	        otherProps = _objectWithoutProperties(props, ['className', 'border', 'children']);
	
	    var classes = (0, _classnames2.default)('mdl-card__actions', {
	        'mdl-card--border': border
	    }, className);
	
	    return _react2.default.createElement(
	        'div',
	        _extends({ className: classes }, otherProps),
	        children
	    );
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.CardMedia"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>CardMedia (props)](#apidoc.element.react-mdl.ReactMDL.CardMedia)
- description and source-code
```javascript
function fn(props) {
	        var className = props.className,
	            children = props.children,
	            otherProps = _objectWithoutProperties(props, ['className', 'children']);
	
	        return _react2.default.createElement(element, _extends({
	            className: (0, _classnames2.default)(defaultClassName, className)
	        }, otherProps), children);
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.CardMenu"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>CardMenu (props)](#apidoc.element.react-mdl.ReactMDL.CardMenu)
- description and source-code
```javascript
function fn(props) {
	        var className = props.className,
	            children = props.children,
	            otherProps = _objectWithoutProperties(props, ['className', 'children']);
	
	        return _react2.default.createElement(element, _extends({
	            className: (0, _classnames2.default)(defaultClassName, className)
	        }, otherProps), children);
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.CardText"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>CardText (props)](#apidoc.element.react-mdl.ReactMDL.CardText)
- description and source-code
```javascript
function fn(props) {
	        var className = props.className,
	            children = props.children,
	            otherProps = _objectWithoutProperties(props, ['className', 'children']);
	
	        return _react2.default.createElement(element, _extends({
	            className: (0, _classnames2.default)(defaultClassName, className)
	        }, otherProps), children);
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.CardTitle"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>CardTitle (props)](#apidoc.element.react-mdl.ReactMDL.CardTitle)
- description and source-code
```javascript
function CardTitle(props) {
	    var className = props.className,
	        children = props.children,
	        expand = props.expand,
	        otherProps = _objectWithoutProperties(props, ['className', 'children', 'expand']);
	
	    var classes = (0, _classnames2.default)('mdl-card__title', {
	        'mdl-card--expand': expand
	    }, className);
	
	    var title = typeof children === 'string' ? _react2.default.createElement(
	        'h2',
	        { className: 'mdl-card__title-text' },
	        children
	    ) : children;
	
	    return _react2.default.createElement(
	        'div',
	        _extends({ className: classes }, otherProps),
	        title
	    );
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.Cell"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Cell (props)](#apidoc.element.react-mdl.ReactMDL.Cell)
- description and source-code
```javascript
function Cell(props) {
	    var _classNames;
	
	    var align = props.align,
	        className = props.className,
	        children = props.children,
	        col = props.col,
	        phone = props.phone,
	        tablet = props.tablet,
	        component = props.component,
	        hideDesktop = props.hideDesktop,
	        hidePhone = props.hidePhone,
	        hideTablet = props.hideTablet,
	        shadow = props.shadow,
	        offset = props.offset,
	        offsetDesktop = props.offsetDesktop,
	        offsetTablet = props.offsetTablet,
	        offsetPhone = props.offsetPhone,
	        otherProps = _objectWithoutProperties(props, ['align', 'className', 'children', 'col', 'phone', 'tablet', 'component', '
hideDesktop', 'hidePhone', 'hideTablet', 'shadow', 'offset', 'offsetDesktop', 'offsetTablet', 'offsetPhone']);
	
	    var hasShadow = isDefined(shadow);
	    var shadowLevel = (0, _clamp2.default)(shadow || 0, 0, _shadows2.default.length - 1);
	
	    var classes = (0, _classnames2.default)('mdl-cell', (_classNames = {}, _defineProperty(_classNames, 'mdl-cell--' + col + '-
col', isDefined(col)), _defineProperty(_classNames, 'mdl-cell--' + phone + '-col-phone', isDefined(phone)), _defineProperty(_classNames
, 'mdl-cell--' + tablet + '-col-tablet', isDefined(tablet)), _defineProperty(_classNames, 'mdl-cell--' + align, isDefined(align)),
_defineProperty(_classNames, 'mdl-cell--' + offset + '-offset', isDefined(offset)), _defineProperty(_classNames, 'mdl-cell--' +
offsetDesktop + '-offset-desktop', isDefined(offsetDesktop)), _defineProperty(_classNames, 'mdl-cell--' + offsetTablet + '-offset
-tablet', isDefined(offsetTablet)), _defineProperty(_classNames, 'mdl-cell--' + offsetPhone + '-offset-phone', isDefined(offsetPhone
)), _defineProperty(_classNames, 'mdl-cell--hide-desktop', hideDesktop), _defineProperty(_classNames, 'mdl-cell--hide-phone', hidePhone
), _defineProperty(_classNames, 'mdl-cell--hide-tablet', hideTablet), _defineProperty(_classNames, _shadows2.default[shadowLevel
], hasShadow), _classNames), className);
	
	    return _react2.default.createElement(component || 'div', _extends({
	        className: classes
	    }, otherProps), children);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.Checkbox"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Checkbox ()](#apidoc.element.react-mdl.ReactMDL.Checkbox)
- description and source-code
```javascript
function Checkbox() {
	        _classCallCheck(this, Checkbox);
	
	        return _possibleConstructorReturn(this, (Checkbox.__proto__ || Object.getPrototypeOf(Checkbox)).apply(this, arguments));
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.Chip"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Chip (props)](#apidoc.element.react-mdl.ReactMDL.Chip)
- description and source-code
```javascript
function Chip(props) {
	    var className = props.className,
	        onClick = props.onClick,
	        onClose = props.onClose,
	        children = props.children,
	        otherProps = _objectWithoutProperties(props, ['className', 'onClick', 'onClose', 'children']);
	
	    var childrenArray = _react2.default.Children.toArray(children);
	    var contactIndex = childrenArray.findIndex(function (c) {
	        return c.type === ChipContact;
	    });
	
	    var chipContent = [];
	
	    if (contactIndex >= 0) {
	        chipContent.push(childrenArray[contactIndex], _react2.default.createElement(
	            ChipText,
	            { key: 'text' },
	            childrenArray.slice(0, contactIndex).concat(childrenArray.slice(contactIndex + 1))
	        ));
	    } else {
	        chipContent.push(_react2.default.createElement(
	            ChipText,
	            { key: 'text' },
	            children
	        ));
	    }
	
	    if (onClose) {
	        chipContent.push(_react2.default.createElement(
	            'button',
	            { key: 'btn', type: 'button', className: 'mdl-chip__action', onClick: onClose },
	            _react2.default.createElement(_Icon2.default, { name: 'cancel' })
	        ));
	    }
	
	    var elt = onClick ? 'button' : 'span';
	
	    return _react2.default.createElement(elt, _extends({
	        className: (0, _classnames2.default)('mdl-chip', {
	            'mdl-chip--contact': contactIndex > -1,
	            'mdl-chip--deletable': !!onClose
	        }, className),
	        type: onClick ? 'button' : null,
	        onClick: onClick
	    }, otherProps), chipContent);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.ChipContact"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>ChipContact (props)](#apidoc.element.react-mdl.ReactMDL.ChipContact)
- description and source-code
```javascript
function fn(props) {
	        var className = props.className,
	            children = props.children,
	            otherProps = _objectWithoutProperties(props, ['className', 'children']);
	
	        return _react2.default.createElement(element, _extends({
	            className: (0, _classnames2.default)(defaultClassName, className)
	        }, otherProps), children);
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.Content"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Content (props)](#apidoc.element.react-mdl.ReactMDL.Content)
- description and source-code
```javascript
function Content(props) {
	    var children = props.children,
	        className = props.className,
	        component = props.component,
	        otherProps = _objectWithoutProperties(props, ['children', 'className', 'component']);
	
	    var classes = (0, _classnames2.default)('mdl-layout__content', className);
	
	    return _react2.default.createElement(component || 'div', _extends({
	        className: classes
	    }, otherProps), children);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.DataTable"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>DataTable (props)](#apidoc.element.react-mdl.ReactMDL.DataTable)
- description and source-code
```javascript
function Sortable(props) {
	            _classCallCheck(this, Sortable);
	
	            var _this = _possibleConstructorReturn(this, (Sortable.__proto__ || Object.getPrototypeOf(Sortable)).call(this, props
));
	
	            _this.handleClickColumn = _this.handleClickColumn.bind(_this);
	
	            if (props.sortable) {
	                _this.state = initState(props);
	            }
	            return _this;
	        }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.Dialog"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Dialog ()](#apidoc.element.react-mdl.ReactMDL.Dialog)
- description and source-code
```javascript
function Dialog() {
	        _classCallCheck(this, Dialog);
	
	        return _possibleConstructorReturn(this, (Dialog.__proto__ || Object.getPrototypeOf(Dialog)).apply(this, arguments));
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.DialogActions"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>DialogActions (props)](#apidoc.element.react-mdl.ReactMDL.DialogActions)
- description and source-code
```javascript
function DialogActions(props) {
	    var className = props.className,
	        fullWidth = props.fullWidth,
	        children = props.children,
	        otherProps = _objectWithoutProperties(props, ['className', 'fullWidth', 'children']);
	
	    var classes = (0, _classnames2.default)('mdl-dialog__actions', {
	        'mdl-dialog__actions--full-width': fullWidth
	    }, className);
	
	    return _react2.default.createElement(
	        'div',
	        _extends({ className: classes }, otherProps),
	        children
	    );
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.DialogContent"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>DialogContent (props)](#apidoc.element.react-mdl.ReactMDL.DialogContent)
- description and source-code
```javascript
function fn(props) {
	        var className = props.className,
	            children = props.children,
	            otherProps = _objectWithoutProperties(props, ['className', 'children']);
	
	        return _react2.default.createElement(element, _extends({
	            className: (0, _classnames2.default)(defaultClassName, className)
	        }, otherProps), children);
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.DialogTitle"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>DialogTitle (props)](#apidoc.element.react-mdl.ReactMDL.DialogTitle)
- description and source-code
```javascript
function DialogTitle(props) {
	    var className = props.className,
	        component = props.component,
	        children = props.children,
	        otherProps = _objectWithoutProperties(props, ['className', 'component', 'children']);
	
	    return _react2.default.createElement(component || 'h4', _extends({
	        className: (0, _classnames2.default)('mdl-dialog__title', className)
	    }, otherProps), children);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.Drawer"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Drawer (props)](#apidoc.element.react-mdl.ReactMDL.Drawer)
- description and source-code
```javascript
function Drawer(props) {
	    var className = props.className,
	        title = props.title,
	        children = props.children,
	        otherProps = _objectWithoutProperties(props, ['className', 'title', 'children']);
	
	    var classes = (0, _classnames2.default)('mdl-layout__drawer', className);
	
	    return _react2.default.createElement(
	        'div',
	        _extends({ className: classes }, otherProps),
	        title ? _react2.default.createElement(
	            'span',
	            { className: 'mdl-layout-title' },
	            title
	        ) : null,
	        children
	    );
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.FABButton"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>FABButton (props)](#apidoc.element.react-mdl.ReactMDL.FABButton)
- description and source-code
```javascript
function FABButton(props) {
	    var mini = props.mini,
	        className = props.className,
	        children = props.children,
	        otherProps = _objectWithoutProperties(props, ['mini', 'className', 'children']);
	
	    var classes = (0, _classnames2.default)('mdl-button--fab', {
	        'mdl-button--mini-fab': mini
	    }, className);
	
	    return _react2.default.createElement(
	        _Button2.default,
	        _extends({ className: classes }, otherProps),
	        children
	    );
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.Footer"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Footer (props)](#apidoc.element.react-mdl.ReactMDL.Footer)
- description and source-code
```javascript
function Footer(props) {
	    var className = props.className,
	        size = props.size,
	        children = props.children,
	        otherProps = _objectWithoutProperties(props, ['className', 'size', 'children']);
	
	    var classes = (0, _classnames2.default)(_defineProperty({}, 'mdl-' + size + '-footer', true), className);
	
	    return _react2.default.createElement(
	        'footer',
	        _extends({ className: classes }, otherProps),
	        (0, _cloneChildren2.default)(children, { size: size })
	    );
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.FooterDropDownSection"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>FooterDropDownSection (props)](#apidoc.element.react-mdl.ReactMDL.FooterDropDownSection)
- description and source-code
```javascript
function DropDownSection(props) {
	    var className = props.className,
	        size = props.size,
	        title = props.title,
	        children = props.children,
	        otherProps = _objectWithoutProperties(props, ['className', 'size', 'title', 'children']);
	
	    var classes = (0, _classnames2.default)(_defineProperty({}, 'mdl-' + size + '-footer__drop-down-section', true), className);
	
	    return _react2.default.createElement(
	        'div',
	        _extends({ className: classes }, otherProps),
	        _react2.default.createElement('input', { className: 'mdl-' + size + '-footer__heading-checkbox', type: 'checkbox', defaultChecked
: true }),
	        _react2.default.createElement(
	            'h1',
	            { className: 'mdl-' + size + '-footer__heading' },
	            title
	        ),
	        (0, _cloneChildren2.default)(children, { size: size })
	    );
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.FooterLinkList"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>FooterLinkList (props)](#apidoc.element.react-mdl.ReactMDL.FooterLinkList)
- description and source-code
```javascript
function LinkList(props) {
	    var className = props.className,
	        size = props.size,
	        children = props.children,
	        otherProps = _objectWithoutProperties(props, ['className', 'size', 'children']);
	
	    var classes = (0, _classnames2.default)(_defineProperty({}, 'mdl-' + size + '-footer__link-list', true), className);
	
	    return _react2.default.createElement(
	        'ul',
	        _extends({ className: classes }, otherProps),
	        _react2.default.Children.map(children, function (child) {
	            return _react2.default.createElement(
	                'li',
	                null,
	                child
	            );
	        })
	    );
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.FooterSection"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>FooterSection (props)](#apidoc.element.react-mdl.ReactMDL.FooterSection)
- description and source-code
```javascript
function Section(props) {
	    var className = props.className,
	        logo = props.logo,
	        size = props.size,
	        type = props.type,
	        children = props.children,
	        otherProps = _objectWithoutProperties(props, ['className', 'logo', 'size', 'type', 'children']);
	
	    var classes = (0, _classnames2.default)(_defineProperty({}, 'mdl-' + size + '-footer__' + type + '-section', true), className
);
	
	    return _react2.default.createElement(
	        'div',
	        _extends({ className: classes }, otherProps),
	        logo ? _react2.default.createElement(
	            'div',
	            { className: 'mdl-logo' },
	            logo
	        ) : null,
	        (0, _cloneChildren2.default)(children, { size: size })
	    );
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.Grid"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Grid (props)](#apidoc.element.react-mdl.ReactMDL.Grid)
- description and source-code
```javascript
function Grid(props) {
	    var noSpacing = props.noSpacing,
	        className = props.className,
	        children = props.children,
	        component = props.component,
	        shadow = props.shadow,
	        otherProps = _objectWithoutProperties(props, ['noSpacing', 'className', 'children', 'component', 'shadow']);
	
	    var hasShadow = typeof shadow !== 'undefined';
	    var shadowLevel = (0, _clamp2.default)(shadow || 0, 0, _shadows2.default.length - 1);
	
	    var classes = (0, _classnames2.default)('mdl-grid', _defineProperty({
	        'mdl-grid--no-spacing': noSpacing
	    }, _shadows2.default[shadowLevel], hasShadow), className);
	
	    return _react2.default.createElement(component || 'div', _extends({
	        className: classes
	    }, otherProps), children);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.Header"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Header (props)](#apidoc.element.react-mdl.ReactMDL.Header)
- description and source-code
```javascript
function Header(props) {
	    var className = props.className,
	        scroll = props.scroll,
	        seamed = props.seamed,
	        title = props.title,
	        transparent = props.transparent,
	        waterfall = props.waterfall,
	        hideTop = props.hideTop,
	        hideSpacer = props.hideSpacer,
	        children = props.children,
	        otherProps = _objectWithoutProperties(props, ['className', 'scroll', 'seamed', 'title', 'transparent', 'waterfall', 'hideTop
', 'hideSpacer', 'children']);
	
	    var classes = (0, _classnames2.default)('mdl-layout__header', {
	        'mdl-layout__header--scroll': scroll,
	        'mdl-layout__header--seamed': seamed,
	        'mdl-layout__header--transparent': transparent,
	        'mdl-layout__header--waterfall': waterfall,
	        'mdl-layout__header--waterfall-hide-top': waterfall && hideTop
	    }, className);
	
	    var isRowOrTab = false;
	    _react2.default.Children.forEach(children, function (child) {
	        if (child && (child.type === _HeaderRow2.default || child.type === _HeaderTabs2.default)) {
	            isRowOrTab = true;
	        }
	    });
	
	    return _react2.default.createElement(
	        'header',
	        _extends({ className: classes }, otherProps),
	        isRowOrTab ? children : _react2.default.createElement(
	            _HeaderRow2.default,
	            { title: title, hideSpacer: hideSpacer },
	            children
	        )
	    );
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.HeaderRow"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>HeaderRow (props)](#apidoc.element.react-mdl.ReactMDL.HeaderRow)
- description and source-code
```javascript
function HeaderRow(props) {
	    var className = props.className,
	        title = props.title,
	        children = props.children,
	        hideSpacer = props.hideSpacer,
	        otherProps = _objectWithoutProperties(props, ['className', 'title', 'children', 'hideSpacer']);
	
	    var classes = (0, _classnames2.default)('mdl-layout__header-row', className);
	
	    return _react2.default.createElement(
	        'div',
	        _extends({ className: classes }, otherProps),
	        title && _react2.default.createElement(
	            'span',
	            { className: 'mdl-layout-title' },
	            title
	        ),
	        title && !hideSpacer && _react2.default.createElement(_Spacer2.default, null),
	        children
	    );
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.HeaderTabs"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>HeaderTabs (props)](#apidoc.element.react-mdl.ReactMDL.HeaderTabs)
- description and source-code
```javascript
function patchedComponent(props) {
	        return React.createElement(
	            _MDLComponent2.default,
	            { recursive: recursive },
	            component(props)
	        );
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.Icon"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Icon (props)](#apidoc.element.react-mdl.ReactMDL.Icon)
- description and source-code
```javascript
function Icon(props) {
	    var className = props.className,
	        name = props.name,
	        otherProps = _objectWithoutProperties(props, ['className', 'name']);
	
	    var classes = (0, _classnames2.default)('material-icons', className);
	
	    return _react2.default.createElement(
	        'i',
	        _extends({ className: classes }, otherProps),
	        name
	    );
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.IconButton"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>IconButton (props)](#apidoc.element.react-mdl.ReactMDL.IconButton)
- description and source-code
```javascript
function IconButton(props) {
	    var className = props.className,
	        name = props.name,
	        otherProps = _objectWithoutProperties(props, ['className', 'name']);
	
	    var classes = (0, _classnames2.default)('mdl-button--icon', className);
	
	    return _react2.default.createElement(
	        _Button2.default,
	        _extends({ className: classes }, otherProps),
	        _react2.default.createElement(_Icon2.default, { name: name })
	    );
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.IconToggle"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>IconToggle ()](#apidoc.element.react-mdl.ReactMDL.IconToggle)
- description and source-code
```javascript
function IconToggle() {
	        _classCallCheck(this, IconToggle);
	
	        return _possibleConstructorReturn(this, (IconToggle.__proto__ || Object.getPrototypeOf(IconToggle)).apply(this, arguments
));
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.Layout"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Layout ()](#apidoc.element.react-mdl.ReactMDL.Layout)
- description and source-code
```javascript
function Layout() {
	        _classCallCheck(this, Layout);
	
	        return _possibleConstructorReturn(this, (Layout.__proto__ || Object.getPrototypeOf(Layout)).apply(this, arguments));
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.List"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>List (props)](#apidoc.element.react-mdl.ReactMDL.List)
- description and source-code
```javascript
function fn(props) {
	        var className = props.className,
	            children = props.children,
	            otherProps = _objectWithoutProperties(props, ['className', 'children']);
	
	        return _react2.default.createElement(element, _extends({
	            className: (0, _classnames2.default)(defaultClassName, className)
	        }, otherProps), children);
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.ListItem"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>ListItem (props)](#apidoc.element.react-mdl.ReactMDL.ListItem)
- description and source-code
```javascript
function ListItem(props) {
	    var className = props.className,
	        twoLine = props.twoLine,
	        threeLine = props.threeLine,
	        otherProps = _objectWithoutProperties(props, ['className', 'twoLine', 'threeLine']);
	
	    var classes = (0, _classnames2.default)('mdl-list__item', {
	        'mdl-list__item--two-line': twoLine && !threeLine,
	        'mdl-list__item--three-line': !twoLine && threeLine
	    }, className);
	
	    var children = _react.Children.map(otherProps.children, function (child) {
	        if (typeof child === 'string') {
	            return _react2.default.createElement(
	                _ListItemContent2.default,
	                null,
	                child
	            );
	        }
	        if (child.type === _ListItemContent2.default) {
	            return (0, _react.cloneElement)(child, {
	                useBodyClass: !!threeLine
	            });
	        }
	        return child;
	    });
	
	    return _react2.default.createElement(
	        'li',
	        _extends({ className: classes }, otherProps),
	        children
	    );
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.ListItemAction"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>ListItemAction (props)](#apidoc.element.react-mdl.ReactMDL.ListItemAction)
- description and source-code
```javascript
function ListItemAction(props) {
	    var children = props.children,
	        className = props.className,
	        info = props.info,
	        otherProps = _objectWithoutProperties(props, ['children', 'className', 'info']);
	
	    var classes = (0, _classnames2.default)('mdl-list__item-secondary-content', className);
	
	    return _react2.default.createElement(
	        'span',
	        _extends({ className: classes }, otherProps),
	        info && _react2.default.createElement(
	            'span',
	            { className: 'mdl-list__item-secondary-info' },
	            info
	        ),
	        _react2.default.createElement(
	            'span',
	            { className: 'mdl-list__item-secondary-action' },
	            children
	        )
	    );
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.ListItemContent"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>ListItemContent (props)](#apidoc.element.react-mdl.ReactMDL.ListItemContent)
- description and source-code
```javascript
function ListItemContent(props) {
	    var avatar = props.avatar,
	        children = props.children,
	        className = props.className,
	        icon = props.icon,
	        subtitle = props.subtitle,
	        useBodyClass = props.useBodyClass,
	        otherProps = _objectWithoutProperties(props, ['avatar', 'children', 'className', 'icon', 'subtitle', 'useBodyClass']);
	
	    var classes = (0, _classnames2.default)('mdl-list__item-primary-content', className);
	    var subtitleClassName = useBodyClass ? 'mdl-list__item-text-body' : 'mdl-list__item-sub-title';
	
	    var iconElement = null;
	    if (icon) {
	        iconElement = createIcon('icon', icon);
	    } else if (avatar) {
	        iconElement = createIcon('avatar', avatar);
	    }
	
	    return _react2.default.createElement(
	        'span',
	        _extends({ className: classes }, otherProps),
	        iconElement,
	        _react2.default.createElement(
	            'span',
	            null,
	            children
	        ),
	        subtitle && _react2.default.createElement(
	            'span',
	            { className: subtitleClassName },
	            subtitle
	        )
	    );
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.MDLComponent"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>MDLComponent ()](#apidoc.element.react-mdl.ReactMDL.MDLComponent)
- description and source-code
```javascript
function MDLComponent() {
	        _classCallCheck(this, MDLComponent);
	
	        return _possibleConstructorReturn(this, (MDLComponent.__proto__ || Object.getPrototypeOf(MDLComponent)).apply(this, arguments
));
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.Menu"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Menu ()](#apidoc.element.react-mdl.ReactMDL.Menu)
- description and source-code
```javascript
function Menu() {
	        _classCallCheck(this, Menu);
	
	        return _possibleConstructorReturn(this, (Menu.__proto__ || Object.getPrototypeOf(Menu)).apply(this, arguments));
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.MenuItem"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>MenuItem (props)](#apidoc.element.react-mdl.ReactMDL.MenuItem)
- description and source-code
```javascript
function fn(props) {
	        var className = props.className,
	            children = props.children,
	            otherProps = _objectWithoutProperties(props, ['className', 'children']);
	
	        return _react2.default.createElement(element, _extends({
	            className: (0, _classnames2.default)(defaultClassName, className)
	        }, otherProps), children);
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.Navigation"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Navigation (props)](#apidoc.element.react-mdl.ReactMDL.Navigation)
- description and source-code
```javascript
function Navigation(props) {
	    var className = props.className,
	        children = props.children,
	        otherProps = _objectWithoutProperties(props, ['className', 'children']);
	
	    var classes = (0, _classnames2.default)('mdl-navigation', className);
	
	    return _react2.default.createElement(
	        'nav',
	        _extends({ className: classes }, otherProps),
	        (0, _cloneChildren2.default)(children, function (child) {
	            return {
	                className: (0, _classnames2.default)({ 'mdl-navigation__link': child.type !== _Spacer2.default }, child.props.className
)
	            };
	        })
	    );
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.ProgressBar"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>ProgressBar ()](#apidoc.element.react-mdl.ReactMDL.ProgressBar)
- description and source-code
```javascript
function ProgressBar() {
	        _classCallCheck(this, ProgressBar);
	
	        return _possibleConstructorReturn(this, (ProgressBar.__proto__ || Object.getPrototypeOf(ProgressBar)).apply(this, arguments
));
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.Radio"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Radio ()](#apidoc.element.react-mdl.ReactMDL.Radio)
- description and source-code
```javascript
function Radio() {
	        _classCallCheck(this, Radio);
	
	        return _possibleConstructorReturn(this, (Radio.__proto__ || Object.getPrototypeOf(Radio)).apply(this, arguments));
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.RadioGroup"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>RadioGroup (props)](#apidoc.element.react-mdl.ReactMDL.RadioGroup)
- description and source-code
```javascript
function RadioGroup(props) {
	    var name = props.name,
	        value = props.value,
	        children = props.children,
	        container = props.container,
	        childContainer = props.childContainer,
	        onChange = props.onChange,
	        otherProps = _objectWithoutProperties(props, ['name', 'value', 'children', 'container', 'childContainer', 'onChange']);
	
	    var hasOnChange = typeof onChange === 'function';
	    var checked = hasOnChange ? 'checked' : 'defaultChecked';
	
	    return _react2.default.createElement(container, otherProps, _react2.default.Children.map(children, function (child) {
	        var _extends2;
	
	        var clonedChild = _react2.default.cloneElement(child, _extends((_extends2 = {}, _defineProperty(_extends2, checked, child
.props.value === value), _defineProperty(_extends2, 'name', name), _defineProperty(_extends2, 'onChange', onChange), _extends2),
otherProps));
	
	        return childContainer ? _react2.default.createElement(childContainer, {}, clonedChild) : clonedChild;
	    }));
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.Slider"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Slider ()](#apidoc.element.react-mdl.ReactMDL.Slider)
- description and source-code
```javascript
function Slider() {
	        _classCallCheck(this, Slider);
	
	        return _possibleConstructorReturn(this, (Slider.__proto__ || Object.getPrototypeOf(Slider)).apply(this, arguments));
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.Snackbar"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Snackbar (props)](#apidoc.element.react-mdl.ReactMDL.Snackbar)
- description and source-code
```javascript
function Snackbar(props) {
	        _classCallCheck(this, Snackbar);
	
	        var _this = _possibleConstructorReturn(this, (Snackbar.__proto__ || Object.getPrototypeOf(Snackbar)).call(this, props));
	
	        _this.clearTimer = _this.clearTimer.bind(_this);
	        _this.timeoutId = null;
	        _this.clearTimeoutId = null;
	        _this.state = {
	            open: false
	        };
	        return _this;
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.Spacer"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Spacer (props)](#apidoc.element.react-mdl.ReactMDL.Spacer)
- description and source-code
```javascript
function fn(props) {
	        var className = props.className,
	            children = props.children,
	            otherProps = _objectWithoutProperties(props, ['className', 'children']);
	
	        return _react2.default.createElement(element, _extends({
	            className: (0, _classnames2.default)(defaultClassName, className)
	        }, otherProps), children);
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.Spinner"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Spinner ()](#apidoc.element.react-mdl.ReactMDL.Spinner)
- description and source-code
```javascript
function Spinner() {
	        _classCallCheck(this, Spinner);
	
	        return _possibleConstructorReturn(this, (Spinner.__proto__ || Object.getPrototypeOf(Spinner)).apply(this, arguments));
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.Switch"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Switch ()](#apidoc.element.react-mdl.ReactMDL.Switch)
- description and source-code
```javascript
function Switch() {
	        _classCallCheck(this, Switch);
	
	        return _possibleConstructorReturn(this, (Switch.__proto__ || Object.getPrototypeOf(Switch)).apply(this, arguments));
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.Tab"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Tab (props)](#apidoc.element.react-mdl.ReactMDL.Tab)
- description and source-code
```javascript
function Tab(props) {
	    var _classNames;
	
	    var active = props.active,
	        className = props.className,
	        component = props.component,
	        children = props.children,
	        cssPrefix = props.cssPrefix,
	        onTabClick = props.onTabClick,
	        style = props.style,
	        tabId = props.tabId,
	        otherProps = _objectWithoutProperties(props, ['active', 'className', 'component', 'children', 'cssPrefix', 'onTabClick', '
style', 'tabId']);
	
	    var classes = (0, _classnames2.default)((_classNames = {}, _defineProperty(_classNames, cssPrefix + '__tab', true), _defineProperty
(_classNames, 'is-active', active), _classNames), className);
	
	    style.cursor = 'pointer';
	
	    return _react2.default.createElement(component || 'a', _extends({
	        className: classes,
	        onClick: function onClick() {
	            return onTabClick(tabId);
	        },
	        style: style
	    }, otherProps), children);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.TabBar"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>TabBar (props)](#apidoc.element.react-mdl.ReactMDL.TabBar)
- description and source-code
```javascript
function TabBar(props) {
	        _classCallCheck(this, TabBar);
	
	        var _this = _possibleConstructorReturn(this, (TabBar.__proto__ || Object.getPrototypeOf(TabBar)).call(this, props));
	
	        _this.handleClickTab = _this.handleClickTab.bind(_this);
	        return _this;
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.Table"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Table (props)](#apidoc.element.react-mdl.ReactMDL.Table)
- description and source-code
```javascript
function Sortable(props) {
	            _classCallCheck(this, Sortable);
	
	            var _this = _possibleConstructorReturn(this, (Sortable.__proto__ || Object.getPrototypeOf(Sortable)).call(this, props
));
	
	            _this.handleClickColumn = _this.handleClickColumn.bind(_this);
	
	            if (props.sortable) {
	                _this.state = initState(props);
	            }
	            return _this;
	        }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.TableHeader"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>TableHeader (props)](#apidoc.element.react-mdl.ReactMDL.TableHeader)
- description and source-code
```javascript
function TableHeader(props) {
	    var className = props.className,
	        name = props.name,
	        numeric = props.numeric,
	        onClick = props.onClick,
	        nosort = props.nosort,
	        tooltip = props.tooltip,
	        children = props.children,
	        otherProps = _objectWithoutProperties(props, ['className', 'name', 'numeric', 'onClick', 'nosort', 'tooltip', 'children
']);
	
	    // remove unwanted props
	    // see https://github.com/Hacker0x01/react-datepicker/issues/517#issuecomment-230171426
	
	
	    delete otherProps.cellFormatter;
	    delete otherProps.sortFn;
	
	    var classes = (0, _classnames2.default)({
	        'mdl-data-table__cell--non-numeric': !numeric
	    }, className);
	
	    var clickFn = !nosort && onClick ? function (e) {
	        return onClick(e, name);
	    } : null;
	
	    return _react2.default.createElement(
	        'th',
	        _extends({ className: classes, onClick: clickFn }, otherProps),
	        !!tooltip ? _react2.default.createElement(
	            _Tooltip2.default,
	            { label: tooltip },
	            children
	        ) : children
	    );
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.Tabs"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Tabs (props)](#apidoc.element.react-mdl.ReactMDL.Tabs)
- description and source-code
```javascript
function patchedComponent(props) {
	        return React.createElement(
	            _MDLComponent2.default,
	            { recursive: recursive },
	            component(props)
	        );
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.Textfield"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Textfield ()](#apidoc.element.react-mdl.ReactMDL.Textfield)
- description and source-code
```javascript
function Textfield() {
	        _classCallCheck(this, Textfield);
	
	        return _possibleConstructorReturn(this, (Textfield.__proto__ || Object.getPrototypeOf(Textfield)).apply(this, arguments
));
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.Tooltip"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>Tooltip (props)](#apidoc.element.react-mdl.ReactMDL.Tooltip)
- description and source-code
```javascript
function Tooltip(props) {
	    var label = props.label,
	        large = props.large,
	        children = props.children,
	        position = props.position,
	        otherProps = _objectWithoutProperties(props, ['label', 'large', 'children', 'position']);
	
	    var id = Math.random().toString(36).substr(2);
	
	    var newLabel = typeof label === 'string' ? _react2.default.createElement(
	        'span',
	        null,
	        label
	    ) : label;
	
	    var element = void 0;
	    if (typeof children === 'string') {
	        element = _react2.default.createElement(
	            'span',
	            null,
	            children
	        );
	    } else {
	        element = _react2.default.Children.only(children);
	    }
	
	    return _react2.default.createElement(
	        'div',
	        _extends({ style: { display: 'inline-block' } }, otherProps),
	        _react2.default.cloneElement(element, { id: id }),
	        _react2.default.createElement(
	            _MDLComponent2.default,
	            null,
	            _react2.default.cloneElement(newLabel, {
	                htmlFor: id,
	                className: (0, _classnames2.default)('mdl-tooltip', _defineProperty({
	                    'mdl-tooltip--large': large
	                }, 'mdl-tooltip--' + position, typeof position !== 'undefined'))
	            })
	        )
	    );
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.getColorClass"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>getColorClass (color, level)](#apidoc.element.react-mdl.ReactMDL.getColorClass)
- description and source-code
```javascript
function getColorClass(color, level) {
	    var lvlClass = level ? '-' + level : '';
	    return 'mdl-color--' + color + lvlClass;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.getTextColorClass"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>getTextColorClass (color, level)](#apidoc.element.react-mdl.ReactMDL.getTextColorClass)
- description and source-code
```javascript
function getTextColorClass(color, level) {
	    var lvlClass = level ? '-' + level : '';
	    return 'mdl-color-text--' + color + lvlClass;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-mdl.ReactMDL.mdlUpgrade"></a>[function <span class="apidocSignatureSpan">react-mdl.ReactMDL.</span>mdlUpgrade (Component)](#apidoc.element.react-mdl.ReactMDL.mdlUpgrade)
- description and source-code
```javascript
mdlUpgrade = function (Component) {
	    var recursive = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : false;
	    return Component.prototype && Component.prototype.isReactComponent ? patchComponentClass(Component, recursive) : patchSFC(Component
, recursive);
	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-mdl.Slider"></a>[module react-mdl.Slider](#apidoc.module.react-mdl.Slider)

#### <a name="apidoc.element.react-mdl.Slider.default"></a>[function <span class="apidocSignatureSpan">react-mdl.Slider.</span>default ()](#apidoc.element.react-mdl.Slider.default)
- description and source-code
```javascript
function Slider() {
    _classCallCheck(this, Slider);

    return _possibleConstructorReturn(this, (Slider.__proto__ || Object.getPrototypeOf(Slider)).apply(this, arguments));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-mdl.Spinner"></a>[module react-mdl.Spinner](#apidoc.module.react-mdl.Spinner)

#### <a name="apidoc.element.react-mdl.Spinner.default"></a>[function <span class="apidocSignatureSpan">react-mdl.Spinner.</span>default ()](#apidoc.element.react-mdl.Spinner.default)
- description and source-code
```javascript
function Spinner() {
    _classCallCheck(this, Spinner);

    return _possibleConstructorReturn(this, (Spinner.__proto__ || Object.getPrototypeOf(Spinner)).apply(this, arguments));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-mdl.Switch"></a>[module react-mdl.Switch](#apidoc.module.react-mdl.Switch)

#### <a name="apidoc.element.react-mdl.Switch.default"></a>[function <span class="apidocSignatureSpan">react-mdl.Switch.</span>default ()](#apidoc.element.react-mdl.Switch.default)
- description and source-code
```javascript
function Switch() {
    _classCallCheck(this, Switch);

    return _possibleConstructorReturn(this, (Switch.__proto__ || Object.getPrototypeOf(Switch)).apply(this, arguments));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-mdl.Textfield"></a>[module react-mdl.Textfield](#apidoc.module.react-mdl.Textfield)

#### <a name="apidoc.element.react-mdl.Textfield.default"></a>[function <span class="apidocSignatureSpan">react-mdl.Textfield.</span>default ()](#apidoc.element.react-mdl.Textfield.default)
- description and source-code
```javascript
function Textfield() {
    _classCallCheck(this, Textfield);

    return _possibleConstructorReturn(this, (Textfield.__proto__ || Object.getPrototypeOf(Textfield)).apply(this, arguments));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-mdl.Tooltip"></a>[module react-mdl.Tooltip](#apidoc.module.react-mdl.Tooltip)

#### <a name="apidoc.element.react-mdl.Tooltip.default"></a>[function <span class="apidocSignatureSpan">react-mdl.Tooltip.</span>default (props)](#apidoc.element.react-mdl.Tooltip.default)
- description and source-code
```javascript
function Tooltip(props) {
    var label = props.label,
        large = props.large,
        children = props.children,
        position = props.position,
        otherProps = _objectWithoutProperties(props, ['label', 'large', 'children', 'position']);

    var id = Math.random().toString(36).substr(2);

    var newLabel = typeof label === 'string' ? _react2.default.createElement(
        'span',
        null,
        label
    ) : label;

    var element = void 0;
    if (typeof children === 'string') {
        element = _react2.default.createElement(
            'span',
            null,
            children
        );
    } else {
        element = _react2.default.Children.only(children);
    }

    return _react2.default.createElement(
        'div',
        _extends({ style: { display: 'inline-block' } }, otherProps),
        _react2.default.cloneElement(element, { id: id }),
        _react2.default.createElement(
            _MDLComponent2.default,
            null,
            _react2.default.cloneElement(newLabel, {
                htmlFor: id,
                className: (0, _classnames2.default)('mdl-tooltip', _defineProperty({
                    'mdl-tooltip--large': large
                }, 'mdl-tooltip--' + position, typeof position !== 'undefined'))
            })
        )
    );
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
