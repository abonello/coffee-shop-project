# Coffee Shop project

## built with Gatsby

## Create new project and launch developer server

```
gatsby new coffee-shop
cd coffee-shop
gatsby develop
```

## Add project images and do some spring cleaning

Deleted

- src/components/header.js
- src/pages/page-2.js
- src/images/gatsby-astronaut.png
- src/images/gatsby-icon.png

Modified

- src/pages/index.js
- src/components/layout.js
- gatsby-config.js

The icon for fav-icon is from [www.iconfinder.com](https://www.iconfinder.com)
Needs attribution:

```
https://www.iconfinder.com/icons/185113/coffee_streamline_icon
Creative Commons (Attribution 3.0 Unported);
https://www.iconfinder.com/webalys
```

## Bootstrap

We will use the Bootstrap download. Download the zip file and copy `bootstrap.min.css` to the components folder. Import this file in the layout.js component.

## React Icons for the cart icon

Install this package. If the server is running, stop it or open a new command line window.

```
npm install react-icons --save
```

Notice the following warning:  
_npm WARN tsutils@3.17.1 requires a peer of typescript@>=2.8.0 || >= 3.2.0-dev || >= 3.3.0-dev || >= 3.4.0-dev || >= 3.5.0-dev || >= 3.6.0-dev || >= 3.6.0-beta || >= 3.7.0-dev || >= 3.7.0-beta but none is installed. You must install peer dependencies yourself._

---

We will need to import specific icons. Ex.

```
import {FaGulp} from 'react-icons/fa'
import { FaBeer } from 'react-icons/fa';
```

For now just a few test icons.

To use the icons, within the jsx

```
<FaGulp />
<FaBeer />
```
