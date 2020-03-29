# Coffee Shop project

## built with Gatsby

## Deployment

[Coffee Shop Deployment](https://coffee-shop-25.netlify.com/)

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

## Deploying on Netlify

This allows continuous deployment from github. After creating a new github repository and pushing the project there, go to Netlify and click the `New site from Git` button. From the options, select `Github`. If asked to, authorise Netlify to access github. Once you select the project's repository click on the `Deploy site` button.

Note: Netlify will run the `gatsby build` command and will use the produced `public/` folder for deployment.

We can change the site name, which will be used for the site subdomain from the **Settings** tab.
I called this _coffee-shop-25_.

Every time we push changes to GitHub, it will trigger a new build and deploy on Netlify.

## The Navbar

Create a new folder called `globals` in the components folder. This will hold components that will be reused throughout the page. Create a `navbar.js` file in the globals folder.

Add **Cart Icon**.

Write the logic for `navbarHandler`.

Note: deleted default styles in layout.css

Add logo with attribution note. This links back to home page.

Created navbar toggler button

Add some basic styles. We will use css variables.
