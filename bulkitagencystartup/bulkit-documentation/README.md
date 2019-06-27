# Welcome
First of all, Thank you so much for purchasing this template and for being our loyal customer. You are awesome! You are entitled to get free lifetime updates to this product and support from the css ninja team directly.

This documentation has been written to help you regarding each step of customization. Please go through the documentation carefully to understand how this template is made and how to edit this properly. HTML and CSS knowledge is required to customize this template.

!> Be careful before you start working with the template and read the documentation. If not edited properly, layouts may break completely. No support is provided for faulty customization.

# Getting started

## Support
If you have any trouble while editing this template or if you simply want to ask a question about something, feel free to contact us at **support@cssninja.io** or to post your request on our support forums at [cssninja.io](https://cssninja.io/forum) 

## Prerequisites
You will need the following tools to customize this template.

1. A good code editor of your choice
2. A supported web browser
3. A Sass preprocessor installed on your workstation (Ruby or Node based)
4. Intermediate `html` knowledge
5. Intermediate `scss` knowledge
6. Basic `javascript` knowledge

!> Be careful before you start working with the template and read the documentation. If not edited properly, layouts may break completely. No support is provided for faulty customization.

## Sass setup
But let's get straight to the point and get started with the template setup. As an `html` template, the setup is very simple. Start by unzipping your Bulkit folder located inside your main download file. Create a new folder for your project at a relevant location on your workspace and copy all the Bulkit files inside it. This new folder should be located in the public folder of a local webserver, you can either use [WAMP](http://www.wampserver.com/) , [MAMP](https://www.mamp.info/en/), [XAMPP](https://www.apachefriends.org/fr/index.html) or any local development environment of your choice.

### Installing Sass
If you already Have Sass installed on your machine, you can skip this section.

### Linux
If you're using a distribution of Linux, you'll need to install Ruby first. You can install Ruby through the apt package manager, rbenv, or rvm.

`sudo gem install sass --no-user-install`

### Windows
Before you start using Sass you will need to install Ruby. The fastest way to get Ruby on your Windows computer is to use [Ruby Installer](http://rubyinstaller.org/). It's a single-click installer that will get everything set up for you super fast. The installer will also install a Ruby command line powershell application that will let you use the Ruby libraries.

### Mac OS
If you prefer the command line over an application then getting Sass set up is a fairly quick process. Sass has a Ruby dependency but if you're using a Mac, congratulations, Ruby comes pre-installed.

### Command line
Here's the quickest way we've found to start using Sass by using the command line:

**1. Open your Terminal or Command Prompt**

On the Mac the Terminal.app comes installed by default. It's located in your "Utilities" folder. On Windows, run `cmd`.

**2. Install Sass**
Ruby uses Gems to manage its various packages of code like Sass. In your open terminal window type: 

`gem install sass`

**3. Install Sass**
This will install Sass and any dependencies for you. It's pretty magical. If you get an error message then it's likely you will need to use the `sudo` command to install the Sass gem. It would look like:

`sudo gem install sass`

**4. Double check**
You should now have Sass installed, but it never hurts to double-check. In your terminal application you can type:

`sass -v`

It should return your Sass version number. Nice ! Sass is now installed on your machine

## Starting Sass
Bulkit is developed with Sass using the Scss syntax, wich is more accessible to beginners as it looks pretty similar to traditionnal css. To edit bulkit styles, you will need to edit the existing Scss files, that will be compiled to css by the freshly installed preprocessor on your machine. Therefore, editing outputed css files is not recommended as you will have or no control over the template styles and components. To start sass, open your command prompt and change directory to your project folder (in wich you previously copied the theme files) :

`cd path/to/my/project`

Then, change directory to the assets folder, wich contains Bulkit CSS and SCSS folders:

`cd assets`

Once done, start the Sass watcher:

`sass --watch scss:css`

This will launch Sass and tell you that Sass is watching for changes. From now on, every modification you will make and save on one of the scss files will trigger a compilation of the related css core file. If you want your outputed css to be minified you can launch Sass and add a `--style` option :

`sass --watch scss:css --style compressed`

# Template structure
This section is about the Bulkit File structure. You will learn where to find the files you need to start working and how to order them. Bulkit has many files and it's easy to get lost. Let's dive into the folder structure.

## Global structure

```
Bulkit
|-- assets
|     |-- css
|     |-- fonts
|     |-- images
|     |-- js
|     |-- scss
|
|-- index.html        
 
```

The directory structure is very simple. All html files are sitting in the theme root folder, with `index.hmtl`. All theme assets are located in the `assets` folder. We will look at the assets details in the upcoming sections.

## Html files
All html files (demos, dashboard and components pages) live in the root of the Bulkit folder. There are 3 main types of html files inside Bulkit:

1. **Demo** pages files
2. **Component** pages files
3. **Dashboard** files

### Demo pages
Bulkit demo pages are regrouped in **6 standalone kits** that you can use to create your own website. Each kit loads needed components and has an additional specific stylesheet, and is tied to a theme. We will see later on how to work with the Themes.

* **Agency kit**

A creative agency ready demo template featuring a homepage, an about page, a portfolio page, a contact page, a blog page and two blog post page variations.

* **Startup kit**

A startup / business ready template featuring a homepage, a product page, an about page, a contact page, a login page and a sign up page.

* **Landing kit 1**

An app selling landing page kit including a landing page, a feature page, a pricing page, a login page and a sign up page.

* **Landing kit 2**

An app selling landing page kit including a landing page, a feature page, a pricing page, a login page and a sign up page.

* **Landing kit 3**

An app selling landing page kit including a landing page, a feature page, a pricing page, a login page and a sign up page.

* **Landing kit 4**

An app selling landing page kit including a landing page, a help center page, a help center categories page, a help article page, a pricing page, a login page and a sign up page.

!> Note that beside static assets like bulma.css, fonts or icons, bulkit html pages load a signgle compiled css stylesheet wich is always named with the following pattern : `core_*.css`

### Component pages
Bulkit features 32 component pages wich feature numerous UI elements and variations. These pages are named following this naming convention: `_components_*category_*component.html` . Each category features different components and variations. You'll find detailed explanations and code examples that you can immediatly copy to start developping. The following categories are available :

* **Layout **

Features building blocks that are relevant to layout such as **Grid system**, **Navbars**, **Video background**, **Headers**, **Footers**, **Typography** and **Colors**.

* **Sections **

Features premade sections that you can copy and paste in your project pages, with little or no customization needed. Available sections are: **Features sections**, **Pricing sections**, **Team sections**, **Testimonials sections**, **Client grids**, **Animated counters** and **Carousel sections**.

* **Basic UI **

Features premade first level components that you can easily reuse such as: **Cards**, **Buttons**, **Dropdowns**, **Lists**, **Modals**, **Tabs & pills**, **Accordions**, **Badges & labels** and **Popups**.

* **Advanced UI **

Features premade first level components that you can easily reuse such as: **Tables**, **Timeline**, **Boxes**, **Lists**, and **Messages**.

* **Forms **

Features premade inputs and form controls to help you build any kind of form including: **Inputs**, **Controls**, **Form layouts**, and **File uploader**.

* **Icons **

Each page in this section lists the different icon collections Bulkit features, with their embed code. Available sets are **Icons Mind**, **Font Awesome**, **Simple line Icons** and **Material Icons**.

!> Be careful not to use the `core_demo.scss` and `core_demo.css` files in production. They contain demo styles that are not suitable for production. You can however reuse some chunks of code in your own files if you want to.

### Dashboard pages

Because we care about our customers, Bulkit features an extra Dashboard kit to jumpstart app frontend development. Several pages are available at the moment. More will come in the future. Notice that only the first section of the sidebar has active links for the moment. All menu items marked with a small lock icon represent features that are not available yet and will likely be released in the future.

The dashboard kit uses its own layout, core file and theme. It uses however the same components as the website template.

## CSS files

Bulkit's CSS sits on top of [Bulma.io](https://bulma.io/) CSS framework, a CSS only trending framework based on Flexbox. Bulma's syntax is semantic, really easy to learn and to use. The layouts are mobile first but are very good on desktop too, with lots of modifiers available. Bulma is still at an early development stage, so we chose to rely on a certain version (bulma 0.3.2). CSS only means that there is no javascript shipped with it, like Bootstrap. Bulkit styles are written in SCSS, on top of Bulma. However, Bulkit introduces its own classes and Variables. There are 3 important css files :

* `bulma.css`

Core framework on top of witch Bulkit is built

* `core.css`

Bulkit stylesheet resutling from all scss files compilation

* `icons.min.css`

A library exceeding 3000 font icons. Includes Font Awesome, Simple Line Icons, Icons Mind and Material Icons (You can and you should split this file to use only the icons that you need).

!> Be sure to use the provided `bulma.css` file in your project and do not try to upgrade to a newer version unless you know what you are doing. Several breaking changes and class name changes have occured since Bulkit was developed. However, this is not an issue, as Bulma is just CSS.

## SCSS files
Bulkit relies on the powerful Sass features, letting you handle complex styles in a breeze.

### File structure
Bulkit relies on a heavy but modular scss structures. You only import in your core file the partials that you need. This how scss files are organized.


```
scss
|-- components
|     |-- _accordion.scss
|     |-- _boxes.scss
|     |-- _buttons.scss
|     |-- _cards.scss
|     |-- _dialogs.scss
|     |-- _dropdowns.scss
|     |-- _forms.scss
|     |-- _labels.scss
|     |-- _lists.scss
|     |-- _messages.scss
|     |-- _pricing.scss
|     |-- _tables.scss
|     |-- _tabs.scss
|     |-- _testimonials.scss
| 
|-- extensions
|     |-- _badge.scss
|     |-- _checkboxes.scss
|     |-- _quickview.scss
|     |-- _range.scss
|     |-- _ribbon.scss
|     |-- _slider.scss
|     |-- _switch.scss
|     |-- _timeline.scss
|     |-- _uploader.scss
| 
|-- layout
|     |-- _animations.scss
|     |-- _footer.scss  
|     |-- _helpers.scss
|     |-- _hero.scss  
|     |-- _navbar.scss
|     |-- _navigation.scss  
|     |-- _pageloader.scss
|     |-- _responsive.scss  
|     |-- _sections.scss  
|
|-- pages
|     |-- _agency.scss
|     |-- _auth.scss  
|     |-- _demo.scss
|     |-- _details.scss  
|     |-- _landing.scss
|     |-- _landing-v1.scss 
|     |-- _landing-v2.scss 
|     |-- _landing-v3.scss 
|     |-- _startup.scss
|
|-- themes
|     |-- _dashboard.scss
|     |-- _deep-blue.scss  
|     |-- _flashy.scss
|     |-- _green.scss  
|     |-- _lemonade.scss
|     |-- _main.scss 
|
|-- _colors.scss
|-- _mixins.scss
|-- core_deep-blue.scss
|-- core_demo.scss
|-- core_flashy.scss
|-- core_green.scss
|-- core_lemonade.scss
|-- dashboard.scss
 
```

### Core and partials
There are two main types of Scss files in Bulkit : Core files and Partial files.

**Partial files**

Partial SCSS file names **always** start with an underscore like this: `_testimonials.scss` . They act as chunks of code that you can import only if you need them. Of course some of them are mandatory for the project to work. For example, if you need to display cards in your project, you can import `scss/components/_cards.scss` to have access to the card components in your layout. We will see later that you need to load them in a specific order to avoid styling issues. SCSS partials are of several types:

  * Global partials: partials that are common to all demos : `scss/_colors.scss` and `scss/_mixins.scss` . Importing `_colors.scss` is mandatory.
  * Theme partials: for the moment, only one theme partial exists, the currently selected theme. Default is `scss/themes/_main.scss` . You have to import a theme in your core file. Otherwise your site will be broken.
  * Layout partials: Layout partials are all mandatory. You **have** to import them in order to setup a basic layout for your website. 
  * Component partials: Component partials are optional. However, you will need to add some to your project to hold the content you are planning publish. Bulkit's approach is modular, so you pick only what you use.
  * Extensions partials: Bulkit is shipped with extensions such as Quickview, Colored checkboxes and many more. Each extension has its own scss partial that you can import if you need some of its features. Sometimes a javascript file is needed for the extension to work.
  * Pages partials: Page partials are related to specific pages. Each demo kit has its own stylesheet, wich is not shared with others. For example, the Startup kit has its own partial named `_startup.scss`. You can find it in `scss/pages/startup.scss` . 

**Core files**

Core files are the heart of Bulkit's styles. Their main purpose is to centralize all styles. Every time you make a change in a partial file, it impacts the outputed `core.css` file resulting from the compilation process. Core files start with imports of other partial SCSS files. Here is an example import statement:

```scss
/*! core.scss | Bulkit | CSS Ninja */

/* ==========================================================================
Main theme core 
========================================================================== */

@import 'colors';
@import 'mixins';
@import 'themes/main';
@import 'layout/navbar';
@import 'layout/animations';
@import 'layout/navigation';
@import 'layout/sections';
@import 'layout/hero';
@import 'layout/footer';
@import 'layout/pageloader';
@import 'components/buttons';
@import 'components/cards';
@import 'components/boxes';
@import 'components/tabs';
@import 'components/testimonials';
@import 'components/dialogs';
@import 'components/forms';
@import 'components/tables';
@import 'components/lists';
@import 'components/labels';
@import 'components/dropdowns';
@import 'components/messages';
@import 'components/pricing';
@import 'extensions/checkboxes';
@import 'pages/details';
@import 'pages/auth';
@import 'pages/startup';
@import 'pages/landing';
@import 'layout/helpers';
@import 'layout/responsive';
```

!> Notice how partials are imported. Whereas the actual partial file name starts with an underscore and ends with a .scss extension, when you write imports inside your `core.scss` file, you have to remove the undescore and the `.scss` extension.

### Imports

Let's break a bit the list of imports we saw above, so we can understand how the global stylesheet is structured and how it impacts the final outputed style.

1. The first line imports scss/_colors.scss. Importing this file is mandatory since it contains all core color variables. Without it, nothing will work and your page will be broken. The second line imports `scss/_mixins.scss` . At the moment it contains one mixin, since Bulma natively provides plenty of them. However, if you need to add yours, this is the right place to do so. Notice that you will have to reimport this file in partials that use your mixins.
2. The third line is also part of mandatory imports. It imports the selected theme from scss/themes/main. There are 5 themes available by default : `_main.scss`, `_deep-blue.scss`, `_lemonade.scss`, `_flashy.scss` and `_dashboard.scss` . Each one of these themes is used by one specific demo kit, except _main.scss, wich is used by both the Startup kit and the Landing kit 1. Each theme can be linked to one or several core files. For more consistency, we linked each theme to a single core file (beside the exception that we mentionned above). You can learn more about themes in the [Theming section](#).
3. The following lines import layout partials from `scss/layout/*`. All of these imports are mandatory for the theme to work, as they handle all animations, navbars, sections, footer and even the preloader.
4.The components imports are up to you. However some of them like `scss/components/_forms.scss` should normally be imported by everyone because... everybody needs forms on a website. But it is still up to you to decide wich components you will need or not in your project. The component imports are followed by extensions imports, if you need to use some special features.
5. Before closing the imports, it's time to get your page specific partials. In the above example, we can see that the core imports `scss/pages/_landing.scss`, wich holds the landing kit 1 specific styles `scss/pages/_auth.scss`, wich handles some login and sign up pages styles, and `scss/pages/_details.scss`, wich handles some miscelaneous styles.
6. At the very end, import the `scss/layout/_helpers.scss` and the `scss/layout/_responsive.scss`. Even if these partials belong to the layout group, they are imported at the end because they are meant to override previously defined styles. See the list of Helpers classes available for more details. The file `_responsive.scss` holds the global media queries that are common to all demos and applied at the theme scope.

### Link the core
Once you finished writing your imports, and adding the basic css rules you want in your core file, you are ready to setup a new page. As we stated before, as soon as Sass is watching for changes, your core file is immediatly outputed into a compiled css file. The css chunks from partials are appended one after another following the order defined in the imports. Open your html page, let's call it `example.html` for the sake of the example. To import the core, just add a link to the compiled css inside your `head` tags:

```html
<link rel="stylesheet" type="text/css" href="assets/css/core.css">

```

You are now ready to start developing. Every change you make to the core file and to the imported partials wil be automatically compiled inside the css stylesheet you just linked to your page (as far as Sass is running on your machine). For a more detailed exaplanation about setting up your project, please head to the [Theming section](#).

## Javascript files
As stated before, Bulkit's is based on a css only framework, Bulma.io. CSS only means there is no javascript shipped with it, unlike Bootstrap. Bulkit has its own javascript implementation of Bulma components using jQuery. You are free to use the existing implementations or to write your own if you want to. You could also use Bulkit in a Vue js project by using only the css and inspiring from jQuery to write Vue js methods. The choice is up to you. Bulkit has 3 main categories of javascript files :

* Core libraries
* Plugins
* Theme javascript

### Core
Bulkit relies on 2 core libraries : **jQuery** and **Modernizr**. No modernizr code is shipped with bulkit, as every project has its specific needs. If you need it, you'll need to write your own.

### Plugins
Bulkit ships with many interesting javascript plugins that increase the frontend experience. If you want more details about plugin usage and initialization, please head to the [js reference section](#). Here is a list of the plugins used by Bulkit.

* **Innostudio file uploader**

A premium jQuery plugin developed by Innostudio. Bulkit grants you a license to use this plugin in one of your projects. It lets you setup a beautiful file uploader for your projects. Read the plugin [documentation](https://innostudio.de/fileuploader/documentation/) for more details about usage.

* **Billboard js **

A javascript library that lets you display nice looking charts based on datasets. Read the plugin [documentation](https://naver.github.io/billboard.js/) for more details about usage.. Billboard js depends on [D3js](https://d3js.org/).

* **Chart js**

Another javascript library that lets you display nice looking charts based on datasets. Read the plugin [documentation](http://www.chartjs.org/) for more details about usage.

* **Chosen js**

A plugin that transforms native html select boxes into beautiful and customizable select boxes with additional features. Read the plugin [documentation](https://harvesthq.github.io/chosen/) for more details about usage.

* **Counterup**

A plugin that makes easy to create animated counters. Notice that it relies on [Waypoints](http://imakewebthings.com/waypoints/), another javascript plugin that triggers events based on scroll position. Read the plugin [documentation](https://github.com/bfintal/Counter-Up) for more details about usage.

* **Covervid**

Bulkit uses this plugin to display full height background videos. Read the plugin [documentation](https://github.com/stefanerickson/covervid) for more details about usage.

* **D3js**

D3 handles svg paths rendering. It is a dependency often used by charting libraries. Billboard js relies on D3. D3 official homepage can be found [here](https://d3js.org/).

* **Datedropper**

Datedropper is a jQuery timepicker plugin. It stands out by it's awesome design and features. Read the plugin [documentation](http://felicegattuso.com/projects/datedropper/) for more details about usage.

* **Datepicker **

jQuery Datepicker is a jQuery timepicker plugin. It has basic features and is a good choice if you are looking for a simple datepicker for your website. Read the plugin [documentation](https://fengyuanchen.github.io/datepicker/) for more details about usage.

* **easyAutocomplete  **

A jQuery plugin that lets you easily setup an autocomplete input. You can also create custom templates for your autocomplete fields. Read the plugin [documentation](http://easyautocomplete.com/) for more details about usage.

* **Datepicker **

jQuery Datepicker is a jQuery timepicker plugin. It has basic features and is a good choice if you are looking for a simple datepicker for your website. Read the plugin [documentation](https://fengyuanchen.github.io/datepicker/) for more details about usage.

* **Embed**

Embed is a small jQuery plugin that lets you embed a Youtube or a Vimeo video inside your page. Nothing to configure, you just have to add the video url.

* **GGtooltip **

A small plugin that helps you to display simple tooltips. Documentation can be found [here](http://www.gigagit.com/item/ggtooltip-js-a-jquery-tooltip-plugin).

* **GGpopover   **

A small plugin that helps you to display nice popovers with many configuration options. Read the plugin [documentation](http://demo.gigagit.com/ggpopover/) for more details about usage.

* **gmapjs   **

A small plugin that lets you display a google map on your web page. Documentation can be found [here](https://hpneo.github.io/gmaps/)..

* **iziToast   **

A nice jQuery plugin to display styled toast notifications on your website. It has many configuration options. Read the plugin [documentation](http://izitoast.marcelodolce.com/) for more details about usage.

* **jqdropdown   **

A flexible and easy to use dropdown jQuery plugin. Read the plugin [documentation](https://labs.abeautifulsite.net/jquery-dropdown/) for more details about usage.

* **jqvmap**

A plugin to display interactive svg maps with less complexity than some others. Read the plugin [documentation](https://jqvmap.com/) for more details about usage.

* **Peity**

A very small plugin that let's you display mini charts in a breeze. Read the plugin [documentation](http://benpickles.github.io/peity/) for more details about usage.

* **scrollreveal**

A must have plugin if you want elements to animate on when visible on scroll. Read the plugin [documentation](https://scrollrevealjs.org/) for more details about usage. 

* **scrollspy**

Everybody knows Scrollspy from Bootstrap. This plugin has the same behaviour. Documentation can be found [here](https://github.com/r3plica/Scrollspy). 

* **slick carousel**

A powerful and highly customizable carousel with a very rich documentation. Read more about it [here](http://kenwheeler.github.io/slick/). 

* **tagsinput**

A simple component to transform a text input into a styled tags input.  Read more about it [here](https://github.com/xoxco/jQuery-Tags-Input). 

* **timedropper**

An original timepicker that can be customized. Read the plugin [documentation](http://felicegattuso.com/projects/timedropper/) for more details about usage. 

* **Vivusjs**

Vivus is a svg animation library. It makes animating svg paths really easy. Read the plugin [documentation](https://maxwellito.github.io/vivus/) for more details about usage. 

* **Waypoints**

Waypoints is a famous jQuery and vanilla js library that let's you setup events that trigger at  certain scroll position. The sticky plugin is also really useful to fix elements on scroll.  Read the plugin [documentation](http://imakewebthings.com/waypoints/) for more details about usage.

* **Wallop slider**

Wallop slider is an original and powerful slider. Beside being lightweight, it is highly customizable. Read more about it [here](https://github.com/peduarte/wallop). 

* **Wickedpicker**

A lightweight library that offers a nice timepicker to replace the boring html native one. Read more about it [here](https://ericjgagnon.github.io/wickedpicker/). 

### Theme javascript
Bulkit comes with it's own javascript files. Let's see the js file structure (without the plugins).

```
js
|-- pages
|     |-- agency.js
|     |-- auth.js
|     |-- components-accordion.js
|     |-- components-fileinput.js
|     |-- components-inputs.js
|     |-- components-modals.js
|     |-- components-quickview.js
|     |-- components-range.js
|     |-- components-toasts.js
|     |-- contact.js
|     |-- dashboard.js
|     |-- demo.js
|     |-- landing.js
|     |-- landingv1.js
|     |-- landingv2.js
|     |-- landingv3.js
|     |-- startup.js
|
|-- main.js    
|
|-- common.js 
 
```

#### Global js
`main.js` and `common.js` are bulkit's main javascript files. They are used by almost every page that Bulkit features (however, the dashboard kit uses its own js file instead of `main.js`). `main.js` holds all plugin initialization but also custom component implementation. However, you should review it carefully before using it in production. Delete the parts that you don't need and customize it to fit your needs. `common.js` holds the code that controls the pageloader. It is used by every Bulkit page. 

#### Page js
The js files in the `/pages` directory are specific to certain pages or elements. 

* `agency.js` : Agency kit specific js file
* `startup.js` : Startup kit specific js file
* `landing.js` : Landing kit 1 specific js file
* `landingv1.js` : Landing kit 2 specific js file
* `landingv2.js` : Landing kit 3 specific js file
* `landingv3.js` : Landing kit 4 specific js file
* `dashboard.js` : Dashboard kit main js file
* `auth.js` : Holds hide and show functions used in login pages
* `contact.js` : Holds code for google maps used in contact pages
* `demo.js` : Holds code used in demo pages (component pages and index, do not use in production)
* `components-accordion.js` : Accordion components implementation
* `components-fileinput.js` : File input components implementation
* `components-inputs.js` : Input components implementation (autocomplete, tagsinput, timepickers, datepickers)
* `components-modals.js` : Modal components implementation
* `components-quickview.js` : Quickview component implementation
* `components-range.js` : Custom range input component implementation
* `components-toasts.js` : Izitoast plugin examples

!> Some components require a js file to work (like accordions, modals, quickview, file inputs ...). Be sure to always import the right files in your projects.

# Theming
Bulkit is built in a css modular approach. We've made it easy for you to customize theme colors. In this section, we are going to setup a project from scratch to help you get started.

## Creating a project
Create a root folder for your Project (my-project) with the following folder and file structure. We will use one of the provided starter kits.

```
my-project
|
|-- assets
|     |-- css
|     |-- fonts
|     |-- images
|     |-- js
|          |-- core
|          |-- pages
|     |-- scss
|          |-- components
|          |-- extensions
|          |-- layout
|          |-- pages
|          |-- themes
|
|-- index.html        
 
```

## Using the Agency kit
Let's copy the Agency kit files in our new project. This way, you'll learn how to use all the available kits.

### Html files
Copy 

* agency.html
* agency-about.html
* agency-portfolio.html
* agency-contact.html
* agency-blog.html
* agency-post-sidebar.html
* agency-post-nosidebar.html

from `/bulkit` root folder to the `/my-project` root folder.

### Css files
Copy 

* bulma.css
* core_flashy.css (Agency kit uses a theme file named `_flashy.scss`)
* icons.min.css 

from `/bulkit/assets/css` folder to the `/my-project/assets/css` folder.

### Fonts
Copy all the files inside  `/bulkit/assets/fonts` to `/my-project/assets/fonts`

### Js files
Start by copying the core libraries

Copy

* jquery.min.js
* modernizr.min.js

from `/bulkit/assets/js/core` folder to the `/my-project/assets/js/core` folder.

Then copy the plugin folders. To know wich plugins are used by the Agency kit, just look at the imported stylesheets and js files in the html pages.

Copy the folders

* /slick-carousel
* /ggpopover
* /wallop
* /waypoints
* /counterup
* /scrollreveal

from `/bulkit/assets/js` folder to the `/my-project/assets/js` folder.

Then, finish by copying the Bulkit js files

Copy

* main.js
* common.js

from `/bulkit/assets/js` folder to the `/my-project/assets/js` folder.

Copy

* agency.js
* contact.js

from `/bulkit/assets/js/pages` folder to the `/my-project/assets/js/pages` folder.

### Scss files
Scss files are the heart of your project. They are vital for you to start customizing styles. Let's start by copying the global scss files.

Copy

* core_flashy.scss
* _colors.scss
* _mixins.scss

from `/bulkit/assets/scss` folder to the `/my-project/assets/scss` folder.

We need to import the theme (e.g the color scheme used by the agency kit)

Copy

* _flashy.scss

from `/bulkit/assets/scss/themes` folder to the `/my-project/assets/scss/themes` folder.

We then need to copy our layout scss files

Copy

* _navbar.scss
* _sections.scss
* _hero.scss
* _footer.scss
* _animations.scss
* _navigation.scss
* _pageloader.scss

from `/bulkit/assets/scss/layout` folder to the `/my-project/assets/scss/layout` folder.

We also need the components scss files

Copy

* _buttons.scss
* _cards.scss
* _boxes.scss
* _tabs.scss
* _testimonials.scss
* _dialogs.scss
* _forms.scss
* _tables.scss
* _lists.scss
* _labels.scss
* _messages.scss
* _pricing.scss
* _dropdowns.scss

If you are using any of the available extensions, you need to copy the relevant files

Copy 

* _checkboxes.scss

from `/bulkit/assets/scss/extensions` folder to the `/my-project/assets/scss/extensions` folder.

We then need to add some page level stylesheets

Copy

* _details.scss
* _auth.scss
* _agency.scss

from `/bulkit/assets/scss/pages` folder to the `/my-project/assets/scss/pages` folder.

Finally we need two critical files, one that holds all the helper classes and another that handles the global media queries.

Copy

* _helpers.scss
* _responsive.scss

from `/bulkit/assets/scss/layout` folder to the `/my-project/assets/scss/layout` folder.

### Double check
You are almost ready to launch and to start cutomizing. Don't forget to copy the `/bulkit/assets/images` folder contents inside the `/my-project/assets/images` folder. Now that all assets are in place you are ready to start customizing. Open your favorite terminal application and change directory to the root of your project.

`cd my-project`

Then go a level deeper, in the assets folder

`cd assets`

Now, enter the command to launch the sass watcher

`sass --watch scss:css --style compressed`

Your teminal window will inform you that sass is watching for changes. From now on, every change you make in any scss file will trigger a recompilation of the core css file (e.g `core_flashy.scss` in the example above). You then just have to open your browser at the right url to see the agency kit homepage. Everything should work fine now.

## Creating a Theme
Let's start from the same example that we buil above. Let's say that the **flashy theme** that the Agency kit uses doesn't fit your needs and that you want to customize it. Let's start from scratch to make you understand how you can do theming with bulkit.

### Add a new Theme

!> If your sass watcher is still running in your terminal, we recommend you to stop it (`Ctrl + C`) before creating a new theme.

Create a new file in `my-project/assets/scss/themes`. For the sake of the example, we will name this file `_example.scss` . Notice the underscore at the start of the file name. Don't forget it or your project will break. 

### Theme colors
Each Bulkit theme uses the same color variables that you can customize to control colors accross the template. There are 3 main variables :

* Primary color
* Secondary color
* accent color

Our new example theme will use primary red (`#f95c64`), secondary blue (`#325bff`) and accent purple (`#dc2dff`) as its main colors (these colors are just an example, do not use in production and pick your own colors instead). Lets create those new variables. Add this to your `scss/themes/_example.scss` file :

```scss
/*! themes/_example.scss | My project | My name */

/* ==========================================================================
Example theme variables and styles 
========================================================================== */

//Theme color variables
$primary: #f95c64;
$secondary: #325bff;
$accent: #dc2dff;
```

Every Bulkit component and layout element rely on these variables. Changing them will immediatly impact all colors on your project. 

### Theme gradient
Every theme comes with a linear gradient based on primary and secondary colors (you can change that if you want, but defining the gradient is mandatory).  Add this to your `scss/themes/_example.scss` file :

```scss
//Hero gradient
$webkit-hero-gradient: -webkit-linear-gradient(to right, $accent, $secondary); 
$hero-gradient: linear-gradient(to right, $accent, $secondary); 
```

### Theme shadows
Bulkit plays alot with colored box shadows. Box shadows inherit their colors from the 3 main variables. Before defining the theme's box shadows, we need to convert our main hex variables to the rgba format. There are many tools to do that quickly and for free, just search on Google. Here are our converted values:


| Variable        | Hex           | Rgb               |
| -------------   |:-------------:| :----------------:|
| $primary        | #f95c64       | rgb(249, 92, 100) |
| $secondary      | #325bff       | rgb(50, 91, 255)  |
| $accent         | #dc2dff       | rgb(220, 45, 255) |

Now that we have our converted values, we can setup box shadows using the rgba format, wich adds the alpha channel for transparency :

```scss
//Primary box shadow
$primary-shadow-from: rgba(249, 92, 100, 0.42);
$primary-shadow-to: rgba(249, 92, 100, 0.2);
$primary-box-shadow:  0 14px 26px -12px $primary-shadow-from, 0 4px 23px 0px $base-shadow, 0 8px 10px -5px $primary-shadow-to !important;

//Secondary box shadow
$secondary-shadow-from: rgba(50, 91, 255, 0.42);
$secondary-shadow-to: rgba(50, 91, 255, 0.2);
$secondary-box-shadow:  0 14px 26px -12px $secondary-shadow-from, 0 4px 23px 0px $base-shadow, 0 8px 10px -5px $secondary-shadow-to !important;

//Accent box shadow
$accent-shadow-from: rgba(220, 45, 255, 0.42);
$accent-shadow-to: rgba(220, 45, 255, 0.2);
$accent-box-shadow:  0 14px 26px -12px $accent-shadow-from, 0 4px 23px 0px $base-shadow, 0 8px 10px -5px $accent-shadow-to !important; 
```

### Theme pageloader
Every theme customizes the default backgound color for the pageloader but it's not mandatory. You are free to do so only if you want to.

```scss
//Pageloader background color 
.pageloader {
    background: $primary !important;
} 
```

## Activating a Theme
You're almost ready to start using your new theme but first, we need to wire it to the core scss file. You can create a new core file or edit the exitsing one. in this example, we wil first edit the existing `core_flashy.scss` file that lives in the `my-project/assets/scss` folder.

Start by renaming the file from `core_flashy.scss` to `core_example.scss` to match our example theme.

!> you could just rename the file `core.scss` without any theme indication. It doesn't make any difference so it is up to you.

Open  `core_example.scss` with your favorite text editor and edit the theme import original statement

```scss
@import 'themes/flashy';
```

Change it to 

```scss
@import 'themes/example';
```

if you start the sass watcher now and try to start working with the theme, you will soon notice that the flashy theme is still active (so don't start the sass watcher yet). This is because you need to edit the links to the core stylesheet in every html page. Let's do it together. Open `my-project/agency.html` file in your editor and change the link to the stylesheet

```html
<link rel="stylesheet" type="text/css" href="assets/css/core_flashy.css">
```

to

```html
<link rel="stylesheet" type="text/css" href="assets/css/core_example.css">
```

Now start the Sass watcher from the assets folder

`sass --watch scss:css --style compressed`

Congratulations, your demo is setup with a brand new theme you just created. You are now ready to start customizing the template. Now that you have a global understanding of how Bulkit works, you can use the Css and Js reference sections of this documentation to get a grasp on Bulkit classes, classes modifiers and javascript options.

# Css reference
This is the css reference section. You will find here the most important element classes and their related modifiers.

## Layout

### Grid system

#### Columns

| Main class | Modifier       | Effects                                                                                 |
|------------|----------------|-----------------------------------------------------------------------------------------|
| `.columns` | `is-vcentered` | Centers nested `column` elements verticaly using flexbox                                |
|            | `is-multiline` | Makes the nested columns wrap into a new row when the end of the current row is reached |
|            | `is-mobile`    | Prevents columns from stacking on mobile devices                                        |
|            | `is-gapless`   | Removes padding from children columns                                                   |

#### Column

| Main class | Modifier         | Effects                                                                                         |
|------------|------------------|-------------------------------------------------------------------------------------------------|
| `.column`  | `is-half`        | Makes the column take half of the available space                                               |
|            | `is-one-third`   | Makes the column take 1/3 of the available space                                                |
|            | `is-two-thirds`  | Makes the column take 2/3 of the available space                                                |
|            | `is-one-quarter` | Makes the column take 1/4 of the available space                                                |
|            | `is-*1-12`       | Makes the column take a ammount of space corresponding to the specified number between 1 and 12 |

### Responsive helpers

#### Display helpers

| Main class | Modifier                  | Effects                                                                                    |
|------------|---------------------------|--------------------------------------------------------------------------------------------|
| `.*`       | `is-flex-mobile`          | Sets display to flex for the target element when device width is < 768px                   |
|            | `is-flex-tablet-only`     | Sets display to flex for the target element when device width is between 769px and 1023px  |
|            | `is-flex-desktop-only`    | Sets display to flex for the target element when device width is between 1024px and 1215px |
|            | `is-flex-widescreen-only` | Sets display to flex for the target element when device width is between 1216px and 1407px |
|            | `is-flex-touch`           | Sets display to flex for the target element when device width is > 1408px                  |
|            | `is-flex-tablet`          | Sets display to flex for the target element when device width is > 768px                   |
|            | `is-flex-desktop`         | Sets display to flex for the target element when device width is > 1024px                  |
|            | `is-flex-widescreen`      | Sets display to flex for the target element when device width is > 1216px                  |
|            | `is-flex-fullhd`          | Sets display to flex for the target element when device width is > 1216px                  |

You can replace the keyword `flex` with the following parameters

* `block`
* `inline`
* `inline-block`
* `inline-flex`

#### Hide helpers

| Main class | Modifier                    | Effects                                                                 |
|------------|-----------------------------|-------------------------------------------------------------------------|
| `.*`       | `is-hidden-mobile`          | Hides the target element when device width is < 768px                   |
|            | `is-hidden-tablet-only`     | Hides the target element when device width is between 769px and 1023px  |
|            | `is-hidden-desktop-only`    | Hides the target element when device width is between 1024px and 1215px |
|            | `is-hidden-widescreen-only` | Hides the target element when device width is between 1216px and 1407px |
|            | `is-hidden-touch`           | Hides the target element when device width is > 1408px                  |
|            | `is-hidden-tablet`          | Hides the target element when device width is > 768px                   |
|            | `is-hidden-desktop`         | Hides the target element when device width is > 1024px                  |
|            | `is-hidden-widescreen`      | Hides the target element when device width is > 1216px                  |
|            | `is-hidden-fullhd`          | Hides the target element when device width is > 1216px                  |

### General helpers

#### Heading helpers

| Main class  | Modifier  | Effects                                     |
|-------------|-----------|---------------------------------------------|
| `.title`    | `is-*1-6` | Sets the title size on a scale of 1 to 6    |
| `.subtitle` | `is-*1-6` | Sets the subtitle size on a scale of 1 to 6 |

#### Text helpers

| Main class | Modifier               | Effects                                        |
|------------|------------------------|------------------------------------------------|
| `*`        | `is-size-*1-6`         | Sets the target text size on a scale of 1 to 6 |
|            | `primary-text`         | Sets the target text color to $primary         |
|            | `secondary-text`       | Sets the target text color to $secondary       |
|            | `accent-text`          | Sets the target text color to $accent          |
|            | `info-text`            | Sets the target text color to $blue            |
|            | `success-text`         | Sets the target text color to $green           |
|            | `warning-text`         | Sets the target text color to $orange          |
|            | `danger-text`          | Sets the target text color to $red             |
|            | `dark-text`            | Sets the target text color to $blue-grey       |
|            | `light-text`           | Sets the target text color to $white           |
|            | `font-w-400`           | Sets the target text font weight to 400        |
|            | `font-w-500`           | Sets the target text font weight to 500        |
|            | `font-w-600`           | Sets the target text font weight to 600        |
|            | `text-bolder`          | Sets the target text font weight to 700        |
|            | `text-decoration-none` | Sets the `text-decoration` property to none    |

#### Padding helpers

| Main class | Modifier            | Effects                                                        |
|------------|---------------------|----------------------------------------------------------------|
| `*`        | `no-padding`        | Sets the target element padding to 0                           |
|            | `no-padding-left`   | Sets the target element left padding to 0                      |
|            | `no-padding-right`  | Sets the target element right padding to 0                     |
|            | `no-padding-top`    | Sets the target element top padding to 0                       |
|            | `no-padding-bottom` | Sets the target element bottom padding to 0                    |
|            | `padding*10-100`    | Sets the target element padding to the specified number        |
|            | `pl*10-80`          | Sets the target element left padding to the specified number   |
|            | `pr*10-80`          | Sets the target element right padding to the specified number  |
|            | `pt*10-80`          | Sets the target element top padding to the specified number    |
|            | `pb*10-80`          | Sets the target element bottom padding to the specified number |
|            | `huge-pt`           | Sets the target element top padding to 100px                   |
|            | `huge-pb`           | Sets the target element bottom padding to 100px                |
|            | `giant-pb`          | Sets the target element bottom padding to 150px                |

#### Margin helpers

| Main class | Modifier           | Effects                                                       |
|------------|--------------------|---------------------------------------------------------------|
| `*`        | `no-margin`        | Sets the target element margin to 0                           |
|            | `no-margin-left`   | Sets the target element left  margin to 0                     |
|            | `no-margin-right`  | Sets the target element right margi nto 0                     |
|            | `no-margin-top`    | Sets the target element top margin to 0                       |
|            | `no-margin-bottom` | Sets the target element bottom margin to 0                    |
|            | `margin-x-auto`    | Sets the target element margin to 0 auto                      |
|            | `ml-auto`          | Sets the target element left margin to auto                   |
|            | `mr-auto`          | Sets the target element right margin to auto                  |
|            | `margin-*10-100`   | Sets the target element margin to the number value            |
|            | `ml*10-80`         | Sets the target element left margin to the specified number   |
|            | `mr*10-80`         | Sets the target element right margin to the specified number  |
|            | `mt*10-80`         | Sets the target element top margin to the specified number    |
|            | `mb*10-80`         | Sets the target element bottom margin to the specified number |

#### States helpers

| Main class | Modifier      | Effects                                        |
|------------|---------------|------------------------------------------------|
| `*`        | `pull-right`  | Adds `float: right` to target element          |
|            | `pull-left`   | Adds `float: left` to target element           |
|            | `is-hidden`   | Sets the target element to`display: none`      |
|            | `is-vhidden`  | Sets the target element to`visibility: hidden` |
|            | `is-disabled` | Disabled click events on target element        |

### Navbar

| Main class        | Modifier                          | Effects                                                                               |
|-------------------|-----------------------------------|---------------------------------------------------------------------------------------|
| `.navbar-wrapper` | `navbar-minimal`                  | Makes the navbar transparent and static (dark version)                                |
|                   | `navbar-minimal` + `navbar-light` | Makes the navbar transparent and static (light version)                               |
|                   | `navbar-fade`                     | Makes the navbar fixed on scroll (dark version)                                       |
|                   | `navbar-fade` + `navbar-light`    | Makes the navbar fixed on scroll (light version)                                      |
|                   | `nav-reverse`                     | Gives access to navbar color classes (must be used with one of the following classes) |
|                   | `nav-reverse` + `nav-primary`     | Makes the navbar background primary                                                   |
|                   | `nav-reverse` + `nav-secondary`   | Makes the navbar background secondary                                                 |
|                   | `nav-reverse` + `nav-dark`        | Makes the navbar background dark                                                      |
|                   | `nav-reverse` + `nav-blue`        | Makes the navbar background blue                                                      |
|                   | `nav-reverse` + `nav-green`       | Makes the navbar background green                                                     |
|                   | `nav-reverse` + `nav-orange`      | Makes the navbar background orange                                                    |
|                   | `nav-reverse` + `nav-red`         | Makes the navbar background red                                                       |

### Hero

| Main class | Modifier             | Effects                                             |
|------------|----------------------|-----------------------------------------------------|
| `.hero`    | `is-medium`          | Sets the hero header to medium size                 |
|            | `is-large`           | Sets the hero header to large size                  |
|            | `is-fullheight`      | Sets the hero header to fullheight size             |
|            | `is-relative`        | Sets the hero position to relative                  |
|            | `is-cover`           | Sets the hero `background-size` property to `cover` |
|            | `is-theme-primary`   |  Sets the hero background color to `$primary`       |
|            | `is-theme-secondary` | Sets the hero background color to `$secondary`      |
|            | `is-theme-accent`    | Sets the hero background color to `$accent`         |
|            | `is-theme-info`      | Sets the hero background color to `$info`           |
|            | `is-theme-success`   | Sets the hero background color to `$success`        |
|            | `is-theme-warning`   | Sets the hero background color to `$warning`        |
|            | `is-theme-danger`    | Sets the hero background color to `$danger`         |
|            | `is-feature-grey`    | Sets the hero background color to `$section-grey`   |
|            | `is-light-grey`      | Sets the hero background color to `$light-grey`     |
|            | `is-coal`            | Sets the hero background color to `$coal`           |

### Sections

| Main class | Modifier                      | Effects                                                     |
|------------|-------------------------------|-------------------------------------------------------------|
| `.section` | `is-medium`                   | Changes the section size to medium                          |
|            | `is-large`                    | Changes the section size to large                           |
|            | `is-relative`                 | Sets the element position to relative                       |
|            | `is-cover`                    | Sets the hero `background-size` property to `cover`         |
|            | `has-border-top`              | Gives the element a top border                              |
|            | `has-bottom-top`              | Gives the element a bottom border                           |
|            | `section-light-grey`          | Sets the element background color to `$light-grey`          |
|            | `section-feature-grey`        | Sets the element background color to `$section-grey`        |
|            | `section-header-grey`         | Sets the element background color to `$header-grey`         |
|            | `section-feature-grey-accent` | Sets the element background color to `$section-grey-accent` |
|            | `section-primary`             | Sets the element background color to `$primary`             |
|            | `section-secondary`           | Sets the element background color to `$secondary`           |

### Footer

| Main class | Modifier               | Effects                                     |
|------------|------------------------|---------------------------------------------|
| `.footer`  | `footer-dark`          | Changes the footer to use dark colors       |
|            | `footer-light`         | Changes the footer to use light colors      |
|            | `footer-dark-left`     | Changes left footer to use dark styles      |
|            | `footer-light-left`    | Changes left footer to use light styles     |
|            | `footer-centered-dark` | Changes centered footer to use dark styles  |
|            | `footer-centered`      | Changes centered footer to use light styles |

## Components

### Simple accordion

| Main class                  | Modifier       | Effects                                            |
|-----------------------------|----------------|----------------------------------------------------|
| `.simple-accordion-wrapper` | `is-primary`   | Sets the element header background to `$primary`   |
|                             | `is-secondary` | Sets the element header background to `$secondary` |
|                             | `is-accent`    | Sets the element header background to `$accent`    |
|                             | `is-info`      | Sets the element header background to `$blue`      |
|                             | `is-success`   | Sets the element header background to `$green`     |

### Boxes

#### Icon box

| Main class  | Modifier    | Effects                                  |
|-------------|-------------|------------------------------------------|
| `.icon-box` | `primary`   | Sets the icon box colors to `$primary`   |
|             | `secondary` | Sets the icon box colors to `$secondary` |
|             | `accent`    | Sets the icon box colors to `$accent`    |
|             | `info`      | Sets the icon box colors to `$info`      |
|             | `success`   | Sets the icon box colors to `$success`   |
|             | `warning`   | Sets the icon box colors to `$warning`   |
|             | `danger`    | Sets the icon box colors to `$danger`    |

#### Diamond box

| Main class     | Modifier    | Effects                                  |
|----------------|-------------|------------------------------------------|
| `.diamond-box` | `primary`   | Sets the icon box colors to `$primary`   |
|                | `secondary` | Sets the icon box colors to `$secondary` |
|                | `accent`    | Sets the icon box colors to `$accent`    |
|                | `info`      | Sets the icon box colors to `$info`      |
|                | `success`   | Sets the icon box colors to `$success`   |
|                | `warning`   | Sets the icon box colors to `$warning`   |
|                | `danger`    | Sets the icon box colors to `$danger`    |

#### Square icon box

| Main class         | Modifier    | Effects                                                    |
|--------------------|-------------|------------------------------------------------------------|
| `.square-icon-box` | `primary`   | Sets the icon box colors to `$primary`                     |
|                    | `secondary` | Sets the icon box colors to `$secondary`                   |
|                    | `accent`    | Sets the icon box colors to `$accent`                      |
|                    | `info`      | Sets the icon box colors to `$info`                        |
|                    | `success`   | Sets the icon box colors to `$success`                     |
|                    | `warning`   | Sets the icon box colors to `$warning`                     |
|                    | `danger`    | Sets the icon box colors to `$danger`                      |
|                    | `rounded`   | Makes the icon rounded instead of the default square shape |

#### Shadow icon box

| Main class         | Modifier       | Effects                                                    |
|--------------------|----------------|------------------------------------------------------------|
| `.shadow-icon-box` | `is-primary`   | Sets the icon box colors to `$primary`                     |
|                    | `is-secondary` | Sets the icon box colors to `$secondary`                   |
|                    | `is-accent`    | Sets the icon box colors to `$accent`                      |
|                    | `is-info`      | Sets the icon box colors to `$info`                        |
|                    | `is-success`   | Sets the icon box colors to `$success`                     |
|                    | `is-warning`   | Sets the icon box colors to `$warning`                     |
|                    | `is-danger`    | Sets the icon box colors to `$danger`                      |
|                    | `rounded`      | Makes the icon rounded instead of the default square shape |

### Buttons

| Main class | Modifier                                  | Effects                                                                       |
|------------|-------------------------------------------|-------------------------------------------------------------------------------|
| `.button`  | `is-small`                                | Small button size                                                             |
|            | `is-medium`                               | Medium button size                                                            |
|            | `is-large`                                | Large button size                                                             |
|            | `button-cta`                              | Transforms a simple button into a big cta button                              |
|            | `button-cta` + `btn-outlined`             | Transforms a simple button into a big outlined cta button                     |
|            | `button-cta` + `btn-outlined` + `is-bold` | Transforms a simple button into a big outlined cta button with a thick border |
|            | `btn-align`                               | Ajusts standard buttons padding                                               |
|            | `btn-align-md`                            | Ajusts medium buttons padding                                                 |
|            | `btn-align-lg`                            | Ajusts large buttons padding                                                  |
|            | `btn-upper`                               | Changes a button `text-transform` property to `uppercase`                     |
|            | `rounded`                                 | Makes a button edges rounded                                                  |
|            | `raised`                                  | Adds a box shadow to a button when hovered                                    |
|            | `is-raised`                               | Permanently adds a box shadow to a button                                     |
|            | `btn-fade`                                | Reduces a button opacity when hovered                                         |
|            | `btn-outlined`                            | Creates an outlined button that gets filled when hovered                      |
|            | `is-link`                                 | Creates a link style button                                                   |
|            | `btn-square`                              | Creates a square shaped button                                                |
|            | `primary-btn`                             | Makes a button background color `$primary`                                    |
|            | `secondary-btn`                           | Makes a button background color `$secondary`                                  |
|            | `accent-btn`                              | Makes a button background color `$accent`                                     |
|            | `info-btn`                                | Makes a button background color `$blue`                                       |
|            | `success-btn`                             | Makes a button background color `$green`                                      |
|            | `warning-btn`                             | Makes a button background color `$orange`                                     |
|            | `danger-btn`                              | Makes a button background color `$danger`                                     |

### Cards

#### Feature card

| Main class      | Modifier         | Effects                                                                     |
|-----------------|------------------|-----------------------------------------------------------------------------|
| `.feature-card` | `card-md`        | Sets the card height to 350px                                               |
|                 | `card-lg`        | Sets the card height to 400px                                               |
|                 | `light-bordered` | Gives a light border to the card element target                             |
|                 | `card-shadow`    | Gives a predefined box shadow to the target card element                    |
|                 | `hover-inset`    | Gives a predefined inset box shadow to the target card element when hovered |

#### Flex card

| Main class   | Modifier         | Effects                                                           |
|--------------|------------------|-------------------------------------------------------------------|
| `.flex-card` | `primary-card`   | Sets the card background color to `primary`                       |
|              | `secondary-card` | Sets the card background color to `secondary`                     |
|              | `accent-card`    | Sets the card background color to `accent`                        |
|              | `card-overflow`  | Sets the target flex card `overflow` property to `visible`        |
|              | `light-bordered` | Gives a light border to the target flex card element              |
|              | `simple-shadow`  | Adds an extra light box shadow to the target flex card element    |
|              | `light-raised`   | Adds a light box shadow to the target flex card element           |
|              | `raised`         | Adds a heavy box shadow to the target flex card element           |
|              | `hover-raised`   | Adds an heavy box shadow on hover to the target flex card element |
|              | `hover-inset`    | Adds an inset box shadow on hover to the target flex card element |

### Dialogs

| Main class | Modifier        | Effects                                                                             |
|------------|-----------------|-------------------------------------------------------------------------------------|
| `.modal`   | `modal-sm`      | change the size of the modal dialog to small                                        |
|            | `modal-hero`    | changes the modal overlay background color to the current theme predefined gradient |
|            | `modal-success` | changes the modal overlay background color to `$green`                              |
|            | `modal-info`    | changes the modal overlay background color to `$blue`                               |
|            | `modal-warning` | changes the modal overlay background color to `$orange`                             |
|            | `modal-error`   | changes the modal overlay background color to `$red`                                |

### Dropdowns

| Main class | Modifier       | Effects                                                                   |
|------------|----------------|---------------------------------------------------------------------------|
| `.dropOut` | `is-primary`   | sets the dropdown menu item background color to `$primary` when hovered   |
|            | `is-secondary` | sets the dropdown menu item background color to `$secondary` when hovered |
|            | `is-accent`    | sets the dropdown menu item background color to `$accent` when hovered    |

### Forms

#### Inputs

| Main class | Modifier             | Effects                                                                  |
|------------|----------------------|--------------------------------------------------------------------------|
| `.input`   | `is-small`           | sets the target input element size to small                              |
|            | `is-medium`          | sets the target input element size to medium                             |
|            | `is-large`           | sets the target input element size to large                              |
|            | `rounded`            | makes the edges of the target input element rounded                      |
|            | `is-primary-focus`   | sets the target input element border color to `$primary` when focused    |
|            | `is-secondary-focus` | sets the target input element border color to `$secondary` when focused  |
|            | `is-accent-focus`    | sets the target input element border color to `$accent` when focused     |
|            | `is-grey-focus`      | sets the target input element border color to `$title-grey` when focused |

#### Textareas

| Main class  | Modifier             | Effects                                                                     |
|-------------|----------------------|-----------------------------------------------------------------------------|
| `.textarea` | `is-grow`            | transforms a basic textarea into an animated textarea on focus              |
|             | `is-default-focus`   | sets the target input element border color to `$default-input` when focused |
|             | `is-primary-focus`   | sets the target input element border color to `$primary` when focused       |
|             | `is-secondary-focus` | sets the target input element border color to `$secondary` when focused     |
|             | `is-accent-focus`    | sets the target input element border color to `$accent` when focused        |
|             | `is-grey-focus`      | sets the target input element border color to `$title-grey` when focused    |

#### Material inputs

| Main class          | Modifier       | Effects                                                                        |
|---------------------|----------------|--------------------------------------------------------------------------------|
| `.control-material` | `is-primary`   | sets the target material input element label and border colors to `$primary`   |
|                     | `is-secondary` | sets the target material input element label and border colors to `$secondary` |
|                     | `is-accent`    | sets the target material input element label and border colors to `$accent`    |
|                     | `is-light`     | sets the target material input element label and border colors to `$white`     |

#### Radio group

| Main class    | Modifier       | Effects                                                      |
|---------------|----------------|--------------------------------------------------------------|
| `.radio-wrap` | `is-small`     | sets the size of the target radio group to small             |
|               | `is-medium`    | sets the size of the target radio group to medium            |
|               | `is-primary`   | sets the dot color of the target radio group to `$primary`   |
|               | `is-secondary` | sets the dot color of the target radio group to `$secondary` |
|               | `is-accent`    | sets the dot color of the target radio group to `$accent`    |

### Labels

#### Badge

| Main class | Modifier         | Effects                                             |
|------------|------------------|-----------------------------------------------------|
| `.b-badge` | `rounded`        | makes the target badge element rounded              |
|            | `badge-outlined` | makes the target badge element outlined             |
|            | `is-primary`     | sets the target badge element color to `$primary`   |
|            | `is-secondary`   | sets the target badge element color to `$secondary` |
|            | `is-accent`      | sets the target badge element color to `$accent`    |
|            | `is-info`        | sets the target badge element color to `$blue`      |
|            | `is-success`     | sets the target badge element color to `$green`     |
|            | `is-warning`     | sets the target badge element color to `$orange`    |
|            | `is-danger`      | sets the target badge element color to `$red`       |

#### Tags

| Main class | Modifier       | Effects                                            |
|------------|----------------|----------------------------------------------------|
| `.tag`     | `squared`      | makes the target tag element edges squared         |
|            | `is-outlined`  | makes the target tag element outlined              |
|            | `is-medium`    | sets the target tag element size to medium         |
|            | `is-large`     | sets the target tag element size to large          |
|            | `is-primary`   | sets the target tag element colors to `$primary`   |
|            | `is-secondary` | sets the target tag element colors to `$secondary` |
|            | `is-accent`    | sets the target tag element colors to `$accent`    |
|            | `is-info`      | sets the target tag element colors to `$blue`      |
|            | `is-success`   | sets the target tag element colors to `$green`     |
|            | `is-warning`   | sets the target tag element colors to `$orange`    |
|            | `is-danger`    | sets the target tag element colors to `$red`       |

### List block

| Main class    | Modifier   | Effects                                                        |
|---------------|------------|----------------------------------------------------------------|
| `.list-block` | `bordered` | gives borders to a list block element                          |
|               | `minimal`  | removes borders and gives a box shadow to a list block element |

### Messages

| Main class | Modifier        | Effects                                                |
|------------|-----------------|--------------------------------------------------------|
| `.message` | `msg-primary`   | sets the target message element colors to `$primary`   |
|            | `msg-secondary` | sets the target message element colors to `$secondary` |
|            | `msg-accent`    | sets the target message element colors to `$accent`    |
|            | `msg-info`      | sets the target message element colors to `$blue`      |
|            | `msg-success`   | sets the target message element colors to `$green`     |
|            | `msg-warning`   | sets the target message element colors to `$orange`    |
|            | `msg-danger`    | sets the target message element colors to `$red`       |

### Navigation tabs

| Main class         | Modifier          | Effects                                                                                                                                                              |
|--------------------|-------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------
| `.navigation-tabs` | `animated-tabs`   | animates tab content transition with a fade in animation                                                                                                             
|                    | `translated-tabs` | animates tab content transition with a translate animation                                                                                                           
|                    | `simple-tabs`     | creates simple underlined tabs                                                                                                                                       
|                    | `boxed-tabs`      | creates boxed style tabs                                                                                                                                             
|                    | `outlined-pills`  | creates outlined pills style tabs, you can also add the class `rounded` to make the edges rounded                                                                    
|                    | `full-pills`      | creates pills style tabs, you can also add the class `rounded` to make the edges rounded, also supports `primary`, `secondary` and `accent` classes for pills colors 
|                    | `square-pills`    | creates squared pills style tabs, you can also add the class `circle-pills` to make the target elements circled                                                      

## Extensions

### Badge

| Main class | Modifier               | Effects                                                                |
|------------|------------------------|------------------------------------------------------------------------|
| `.badge`   | `is-badge-left`        | positions the target badge element on the left of its container        |
|            | `is-badge-bottom`      | positions the target badge element at the bottom of its container      |
|            | `is-badge-bottom-left` | positions the target badge element at the bottom left of its container |
|            | `is-badge-small`       | sets the target badge element size to small                            |
|            | `is-badge-medium`      | sets the target badge element size to medium                           |
|            | `is-badge-large`       | sets the target badge element size to large                            |
|            | `is-badge-outlined`    | makes the target badge element outlined                                |
|            | `badge-primary`        | sets the target badge element colors to `$primary`                     |
|            | `badge-secondary`      | sets the target badge element colors to `$secondary`                   |
|            | `badge-accent`         | sets the target badge element colors to `$accent`                      |
|            | `badge-info`           | sets the target badge element colors to `$blue`                        |
|            | `badge-success`        | sets the target badge element colors to `$green`                       |
|            | `badge-warning`        | sets the target badge element colors to `$orange`                      |
|            | `badge-danger`         | sets the target badge element colors to `$red`                         |

### Checkboxes

| Main class    | Modifier       | Effects                                                           |
|---------------|----------------|-------------------------------------------------------------------|
| `.b-checkbox` | `is-circular`  | makes the target b-checkbox element circular                      |
|               | `is-inline`    | sets the target b-checkbox element `display` property to `inline` |
|               | `is-primary`   |  sets the target b-checkbox element colors to `$primary`          |
|               | `is-secondary` | sets the target b-checkbox element colors to `$secondary`         |
|               | `is-accent`    | sets the target b-checkbox element colors to `$accent`            |
|               | `is-info`      | sets the target b-checkbox element colors to `$blue`              |
|               | `is-success`   | sets the target b-checkbox element colors to `$green`             |
|               | `is-warning`   | sets the target b-checkbox element colors to `$orange`            |
|               | `is-danger`    | sets the target b-checkbox element colors to `$red`               |

### Range inputs

| Main class          | Modifier       | Effects                                                           |
|---------------------|----------------|-------------------------------------------------------------------|
| `input[type=range]` | `is-small`     | sets the target range input element size to small                 |
|                     | `is-medium`    | sets the target range input element size to medium                |
|                     | `is-large`     | sets the target range input element size to large                 |
|                     | `is-primary`   |  sets the target range input element colors to `$primary`         |
|                     | `is-secondary` | sets the target range input element colors to `$secondary`        |
|                     | `is-accent`    | sets the target range input element colors to `$accent`           |
|                     | `is-info`      | sets the target range input element colors to `$blue`             |
|                     | `is-success`   | sets the target range input element colors to `$green`            |
|                     | `is-warning`   | sets the target range input element colors to `$orange`           |
|                     | `is-danger`    | sets the target range input element colors to `$red`              |

### Switch

| Main class                 | Modifier       | Effects                                               |
|----------------------------|----------------|-------------------------------------------------------|
| `.switch[type="checkbox"]` | `is-outlined`  | makes the target switch element outlined              |
|                            | `is-thin`      | applies the thin style to the target switch element   |
|                            | `is-small`     | sets the target switch element size to small          |
|                            | `is-medium`    | sets the target switch element size to medium         |
|                            | `is-large`     | sets the target switch element size to large          |
|                            | `is-primary`   | sets the target switch element colors to `$primary`   |
|                            | `is-secondary` | sets the target switch element colors to `$secondary` |
|                            | `is-accent`    | sets the target switch element colors to `$accent`    |
|                            | `is-info`      | sets the target switch element colors to `$blue`      |
|                            | `is-success`   | sets the target switch element colors to `$green`     |
|                            | `is-warning`   | sets the target switch element colors to `$orange`    |
|                            | `is-danger`    | sets the target switch element colors to `$red`       |

# Js reference
This is the javascript reference section. You will find here what you need to know to get started with the theme's js.

## Pageloader
If you wish to change the behaviour of the pageloader component, you'll want to edit the snippet in `bulkit/assets/js/common.js` file. Here is the snippet that controls the pageloader :

```js
$(document).ready(function(){

    //Page loader
    if ($('.pageloader').length) {

        $('.pageloader').toggleClass('is-active');

        $(window).on('load', function() {
        var pageloaderTimeout = setTimeout( function() {
            $('.pageloader').toggleClass('is-active');
            $('.infraloader').toggleClass('is-active')
            clearTimeout( pageloaderTimeout );
        }, 700 );
        })
    }
});
```

## Navbar

### Responsive toggle

If you want to change the way the responsive menu toggle behaves, you need to edit this code, that you can find in  `bulkit/assets/js/main.js` :

```js
//Mobile menu toggle
if ($('.nav-toggle').length) {
    $('.nav-toggle').click(function(){
        $(this).toggleClass('is-active');
        if ($('.nav-menu').hasClass('is-active')) {
            $('.nav-menu').removeClass('is-active');
        } else {
            $('.nav-menu').addClass('is-active');
        }
        if ($('.navbar-wrapper').hasClass('navbar-fade', 'navbar-light')) {
            $('.navbar-wrapper').toggleClass('mobile-menu-dark');
        }
    });
}
```

### Navbar fade

You can turn the static top navigation to a navbar that fades in and out when you scroll the window. You just need to add the `navbar-fade` class to the `navbar-wrapper` element. You will find the javascript code that controls that behaviour in `bulkit/assets/js/main.js` :

```js
//Sticky scroll navbar
if ($('.navbar-wrapper.navbar-fade').length) {
    $(".navbar-wrapper.navbar-fade").wrap('<div class="navbar-placeholder"></div>');
    $(".navbar-placeholder").height(jQuery(".navbar-wrapper.navbar-fade").outerHeight());
    $(window).scroll(function() {    // this will work when your window scrolled.
        var height = $(window).scrollTop();  //getting the scrolling height of window
        if(height  > 65) {
            $(".navbar-wrapper.navbar-fade").removeClass('navbar-fade').addClass('translateDown navbar-sticky');
        } else{
            $(".navbar-wrapper.navbar-sticky").removeClass('translateDown navbar-sticky').addClass('navbar-fade');
        }
    });
}
```
!> Notice that it will be enough if you use the standard sticky navbar (e.g with normal logo and dark text colors). But if you choose to add the `navbar-light` class to the `.navbar-wrapper.navbar-fade` element, your navbar will turn to light colors (you will need it for colored hero sections). You will then need another snippet to control the color transitions and the logo replacement when the window is scrolled and the solid navbar comes in. You can find this snippet in the js files related to prebuilt kits as each kit needs to have its own logo color. Also, don't forget to add the `light-logo` class to the `navbar-light` logo, so the logo transition can be executed on scroll.

```html
<!-- Setting up the light fade navbar -->
<div class="navbar-wrapper navbar-fade navbar-light"></div>

<!-- identifying the logo as the light logo -->
<a class="nav-item" href="landing.html">
    <img class="light-logo" src="assets/images/logos/bulkit-w.png" alt="">
</a>
```

Here is an example with the standard bulkit logo:

```js
//Toggle between light and dark logo when solid navbar comes in
$(window).scroll(function() {    // this will work when your window scrolled.
    var height = $(window).scrollTop();  //getting the scrolling height of window
    if(height  > 80) {
        $("img.light-logo").attr("src","assets/images/logos/bulkit-logo.png");
    } else{
        $("img.light-logo").attr("src","assets/images/logos/bulkit-w.png");
    }
});

//This toggles the Sign up button color from white to primary when the window is scrolled
if ($('.navbar-light').length) {
    $(window).scroll(function() {    // this will work when your window scrolled.
        var height = $(window).scrollTop();  //getting the scrolling height of window
        if(height  > 80) {
            $('.button-signup').removeClass('light-btn').addClass('primary-btn');
        } else{
            $('.button-signup').removeClass('primary-btn').addClass('light-btn');
        }
    }); 
}
```

## Sidebar

The sidebar menu is easy to control, this is how it is triggered. you can find the code in  `bulkit/assets/js/main.js` .

```js
//trigger sidebar
$('#navigation-trigger, .navigation-trigger, .navigation-close').click(function(){
    $('.side-navigation-menu').toggleClass('is-active');
})
```

When you click on the category buttons of the sidebar (represented with icons on the left), the sidebar menu content changes. This is controlled with data attributes. If you want to add a new sidebar menu, add some markup (see the structure below) to the sidebar and give it a unique ID :

```html
<!-- Navigation menu -->
<div id="my-menu" class="navigation-menu-wrapper animated preFadeInRight fadeInRight is-hidden">
    <!-- Navigation Header -->
    <div class="navigation-menu-header">
        <span>Components</span>
        <a class="ml-auto hamburger-btn navigation-close" href="javascript:void(0);">
            <span class="menu-toggle">	
                <span class="icon-box-toggle"> 	
                    <span class="rotate">
                        <i class="icon-line-top"></i>
                        <i class="icon-line-center"></i>
                        <i class="icon-line-bottom"></i> 
                    </span>
                </span>
            </span>
        </a>
    </div>
    <!-- Navigation body -->
    <ul class="navigation-menu">
        <li class="has-children"><a class="parent-link" href="#"><span class="material-icons">view_quilt</span>Layout</a>
            <ul>
                <li><a class="is-submenu" href="some_page.html">A menu item</a></li>
                <li><a class="is-submenu" href="some_page.html">Another item</a></li>
                <li><a class="is-submenu" href="some_page.html">A third item</a></li>
            </ul>
        </li>
    </ul>
</div
```

Then, create a new category button :

```html
<ul class="categories">
    <li class="category-link" data-navigation-menu="my-menu"><i class="icon some-icon"></i></li>
</ul>
```

Notice how the `data-navigation-menu` attribute is pointing to the newly created menu ID. This is how you link them.

Here is the code that controls that `data-attribute` :

```js
//Data navigation menu setup
$('.category-link').click(function(){
    var category_id = $(this).attr('data-navigation-menu');
    $('.navigation-menu-wrapper').addClass('is-hidden');
    $("#" + category_id).removeClass('is-hidden');
})
```

## Parallax

Bulkit comes with built-in parallax hero and section. You can quickly setup a parallax header or section by adding the `parallax` class to a `.hero` or `.section` element. You will also need to add the `is-relative` class to the target element so the parallax overlay can be positioned correctly. You can also add the `is-cover` class wich is shortcut to `background-size: cover` .

You can also use data-attributes to pass some additional options like a background image, the overlay color and the overlay opacity. Here is an example of a Parallax hero markup

```html
<!-- Fullheight Parallax Hero -->
<div class="hero parallax is-cover is-relative is-fullheight" 
    data-background="assets/images/bg/good-morning.jpeg" 
    data-color="#7F00FF" 
    data-color-opacity="0.8">
```
!> The `data-color` attribute only accepts hex values

## Background images

Bulkit has built-in support for background images via data attributes. To add a background image to any element, use the `data-background="path/to/my/image.jpg"` attribute with a valid image url. Notice that you will still have to style your element's background properties with css.

## Plugins

### Tooltips

This is how you initialize tooltips :

```js
$('[data-toggle="tooltip"]').ggtooltip();
```

### Popovers

This is how you initialize popovers :

```js
$('[data-toggle="popover"]').ggpopover();
```

### Datedropper

This is how you initialize Datedropper js :

```js
$('#my-element').dateDropper();
```

### Datepicker

This is how you initialize jQuery datepicker :

```js
$('[data-toggle="datepicker"]').datepicker();
```

### Timedropper

This is how you initialize Timedropper js :

```js
$('#my-element').timeDropper({
    primaryColor: '#4FC1EA',
    borderColor:"#4FC1EA",
    backgroundColor:"#FFF",
    init_animation: 'fadeIn',
});
```

### Wickedpicker

Wickedpicker is simple timepicker plugin. it only has a few options. Here are two examples :

**12 hours :** 

```js
$('.my-element').wickedpicker();
```

**24 hours :** 

```js
$('.my-element').wickedpicker({
    twentyFour: true,
    timeSeparator: ':'
});
```

### Slick carousel

This how to initialize a basic a basic slick carousel, visit the plugin website to see all available options :

```js
$('.my-element').slick({
    dots: true,
    infinite: true,
    speed: 500,
    cssEase: 'cubic-bezier(0.645, 0.045, 0.355, 1.000)',
    autoplay: true,
});
```
### Tags input

This is how to initialize the tagsinput plugin :

```js
$('.my-element').jQueryInputTags({
    maxTotalSize: 255,
    maxTagSize: 10,
    minTagSize: 3,
    chars: /[,:]/,
    keycode: /(^9$|^13$|^32)/, // Tab, Enter, Space
    separator: ',',
    sensitive: false,
    clearSpaces: true

});
```

### Embed

To initialize the embed video instance, use this code :

```js
//Video embed init
if ($('#my-element').length) {
    Video('#my-element');
}
```

### Counterup

This is how to initialize counterup (don't forget that it depends on waypoints) :

```js
$('.my-element').counterUp({
    delay: 10,
    time: 1000
});
```

### Chosen

This is how to initialize your chosen selects. See the plugin's documentation for all available options.

```js
$(".my-element").chosen({
    disable_search_threshold: 6,
    width: '100%'
});
```

### Wallop Slider

Wallop slider is very flexible. Look at the plugin's documentation for more details about available options. Below an example of how to initialize a fullscreen slider (you will also need css to build your slider layout) :

```js
if ($('.Wallop').length) {
    var wallopEl = document.querySelector('.Wallop');
    var wallop = new Wallop(wallopEl);

    var paginationDots = Array.prototype.slice.call(document.querySelectorAll('.Wallop-dot'));

    //Attach click listener on the dots

    paginationDots.forEach(function (dotEl, index) {
        dotEl.addEventListener('click', function() {
            wallop.goTo(index);
        });
    });

    // Listen to wallop change and update classes

    wallop.on('change', function(event) {
        removeClass(document.querySelector('.Wallop-dot--current'), 'Wallop-dot--current');
        addClass(paginationDots[event.detail.currentItemIndex], 'Wallop-dot--current');
    });



    // Helpers
    function addClass(element, className) {
        if (!element) { return; }
        element.className = element.className.replace(/\s+$/gi, '') + ' ' + className;
    }

    function removeClass(element, className) {
        if (!element) { return; }
        element.className = element.className.replace(className, '');
    }

    // To start Autoplay, just call the function below
    // and pass in the number of seconds as interval
    // if you want to start autoplay after a while
    // you can wrap this in a setTimeout(); function
    autoplay(5000);

    // This a a helper function to build a simple
    // auto-play functionality. 
    function autoplay(interval) {
        var lastTime = 0;  

        function frame(timestamp) {
            var update = timestamp - lastTime >= interval;

            if (update) {
                wallop.next();
                lastTime = timestamp;
            }

            requestAnimationFrame(frame);
        }

        requestAnimationFrame(frame);
    };
}
```

### Scrollreveal

Scrollreveal lets you define on scroll animations for your page elements. check the plugin documentation for all available options. Here is an example :

```js
// Declaring defaults
window.sr = ScrollReveal();

// Simple reveal
sr.reveal('.is-title-reveal', { 
    origin: 'bottom',
    distance: '20px',
    duration: 600,
    delay: 100,
    rotate: { x: 0, y: 0, z: 0 },
    opacity: 0,
    scale: 1,
    easing: 'cubic-bezier(0.215, 0.61, 0.355, 1)',
    container: window.document.documentElement,
    mobile: true,
    reset: false,
    useDelay: 'always',
    viewFactor: 0.2,
});
```

### easyAutocomplete

This plugin let's you create simple and more complex autocompletes. We will see 2 examples here, a basic one and an advanced one with a cutom template.

Basic example: 

```js
//Basic autocomplete
if ($('#basic-autocpl').length) {
    var options = {
        url: "assets/js/easyAutocomplete/data/persons.json",
        getValue: function(element) {
            return element.name;
        },
        highlightPhrase: false,
        list: {
            maxNumberOfElements: 5,
            showAnimation: {
                type: "fade", //normal|slide|fade
                time: 400,
                callback: function() {}
            },
            match: {
                enabled: true
            }
        },
    };

    $("#basic-autocpl").easyAutocomplete(options);
}
```

Custom example using a custom template: 

```js
//Users autocomplete
if ($('#users-autocpl').length) {
    var usersOptions = {
        url: "assets/js/easyAutocomplete/data/persons.json",
        getValue: "name",
        template: {
            type: "custom",
            method: function(value, item) {
                return "<div class=" + 'template-wrapper' + "><img class=" + 'autocpl-avatar' + " src='" + item.pic + "' /><div class=" + 'entry-text' + ">" + value + "<br><span>" + item.email + "</span></div></div> ";
            }
        },
        highlightPhrase: false,
        list: {
            maxNumberOfElements: 3,
            showAnimation: {
                type: "fade", //normal|slide|fade
                time: 400,
                callback: function() {}
            },
            match: {
                enabled: true
            }
        },
    };

    $("#users-autocpl").easyAutocomplete(usersOptions);
}
```

!> Notice that esayAutocomplete gets its data from a `json` formatted file. Be sure to provide a validated json file and the right path to access it.

### iziToast

This how you initialize a simple toast message. Check the `bulkit/assets/js/pages/components-toats.js` for more examples :

```js
$('#top-left-toast').click(function(){
    iziToast.show({
        title: 'Hello,',
        message: 'Iam a very simple Toast !',
        position: 'topLeft',
    });
})
```

### gmapjs

Initialize a google map element :

```
if ($('#my-map').length) {
    $('#my-map').gMap({
        latitude: 40.7143528,
        longitude: -74.0059731,
        maptype: 'ROADMAP',
        zoom: 13,
        markers: [
            {
                latitude: 40.71771,
                longitude:  -74.003245,
                html: '<div style="width: 300px;"><h4 style="margin-bottom: 8px;"></h4><div style="align-items:center!important;" class="content content-flex"><div><img style="height:60px;border-radius:100px;" src="assets/images/logos/cssninja.svg"></div><div style="margin-left:20px;"> Iam very happy if you like this template. If you need any support, please feel free to contact us at <strong>hello@cssninja.io</strong></div></div></div>',
                icon: {
                    image: "assets/images/markers/marker-purple.png",
                    iconsize: [56, 82],
                    iconanchor: [32,39]
                }
            }
        ],
        doubleclickzoom: true,
        controls: {
            panControl: true,
            zoomControl: true,
            mapTypeControl: true,
            scaleControl: false,
            streetViewControl: false,
            overviewMapControl: false
        }
    });
}
```

### vmap

initialize an svg map. Check the plugin's riche documentation for more details about usage and available options.

```js
$('#vmap').vectorMap({
    map: 'usa_en',
    backgroundColor: null,
    colors: {
        mo: '#00D1B2',
        fl: '#7f00ff',
    },
    hoverOpacity: 0.7,
    selectedColor: '#666666',
    enableZoom: true,
    borderColor: '#999',
    showTooltip: true,
    //values: sample_data,
    //scaleColors: ['#00D1B2', '#7F00FF'],
    normalizeFunction: 'polynomial',
});
```

### Charts

Dashkit uses 3 charting libraries. Here are some examples to get you started. Reading these libraries documentation is however highly recommended.

#### Chart js

```js
//Chartjs Bar chart
if ($('#barChart').length) {
    new Chart(document.getElementById("barChart"), {
        type: 'bar',
        data: {
            labels: ["France", "Germany", "UK", "spain", "Belgium"],
            datasets: [
                {
                    label: "Last month Sales ($)",
                    backgroundColor: ["#00D1B2", "#7F00FF","#536dfe","#039BE5","#999"],
                    data: [12478,15267,11734,19784,12433]
                }
            ]
        },
        options: {
            maintainAspectRatio: false,
            legend: { display: false },
            title: {
                display: false,
                text: ''
            },
            scales: {
                xAxes: [{
                    display: true,
                    //stacked: true,
                    gridLines: {
                        color: "rgba(0, 0, 0, 0)",
                    } ,
                    scaleLabel: {
                        display: false,
                    },
                }],
                yAxes: [{
                    display: true,
                    //stacked: true,
                    gridLines: {
                        color: "rgba(0, 0, 0, 0)",
                    },
                    ticks: {
                        fontSize: 9,
                        fontColor: '#999',
                        autoSkip: true,
                        maxTicksLimit: 6,
                        callback: function(value) {
                            var ranges = [
                                { divider: 1e6, suffix: 'M' },
                                { divider: 1e3, suffix: 'k' }
                            ];
                            function formatNumber(n) {
                                for (var i = 0; i < ranges.length; i++) {
                                    if (n >= ranges[i].divider) {
                                        return (n / ranges[i].divider).toString() + ranges[i].suffix;
                                    }
                                }
                                return n;
                            }
                            return '$' + formatNumber(value);
                        }
                    }
                }],
            },
            tooltips: {
                backgroundColor: "rgba(68, 79, 96,0.7)",
                xPadding: 10,
                yPadding: 15,
                cornerRadius: 4,
                borderColor: "rgba(68, 79, 96,0.7)",
                caretSize: 4,
            },
        }
    });
}
```

#### Billboard js

```js
//Billboardjs line chart
if ($('#lineChart').length) {
    var chart = bb.generate({
        "data": {
            "columns": [
                ["Paid", 120, 149, 98, 131, 152, 139],
                ["Canceled", 50, 20, 10, 40, 15, 25],
                ['Pending', 75, 87, 56, 68, 62, 41]
            ],
            "colors": {
                "Paid": "#00D1B2",
                "Canceled": "#7F00FF",
                "Pending": "#536dfe"
            },
        },
        "size": {
            "height": 260,
        },
        "bindto": "#lineChart"
    });
}
```

#### Peity js

```js
//Small bar chart 
$(".small-bars").peity("bar", {
    fill: ["#fff"],
    height: 30,
    width: '50%'
})
```
# Customer support
Please remember you have purchased a very affordable theme and you did not pay for a full-time web design agency. We will help with your issues, but these requests will be put on a relevant priority, regarding their nature. Support is provided for your comfort and for a best possible experience, so please be patient, polite and respectful, as we are towards you.

## Support includes 

* Responding to questions or problems regarding the item and its features
* Fixing bugs and reported issues
* Providing updates 

## Support doesn't include

* Customization and installation services
* Support for third party software and plug-ins

## Before Support

* Make sure your question is a valid Theme Issue and not a customization request
* Make sure you have read through the documentation and any ressources before asking support on how to accomplish a task
* Make sure to double check the theme FAQs.
* If you have customized your theme and now have an issue, back-track to make sure you didn't make a mistake. If you have made changes and can't find the issue, please provide us with your changelog.
* Almost 80% of the time we find that the solution to people's issues can be solved with a simple "Google Search". You might want to try that before seeking support. You might be able to fix the issue yourself much quicker than we can respond to your request.
* Make sure to state the name of the theme you are having issues with when requesting support.

# Changelog
You can find the version history (changelog.txt) file on bulkit-theme.zip folder or you can check the changelog on the theme sale page.

Once again, thank you so much for purchasing this theme. As I said at the beginning, we'd be glad to help you if you have any questions relating to this theme. No guarantees, but we'll do our best to assist and support you. If you have a more general question relating to Bulkit, you might consider visiting our support forums and asking your question in the "Bulkit support" section.

```
-----------------------------------------------------------------------------------------
Version 1.0.0 - Jan 10, 2018
-----------------------------------------------------------------------------------------
 
- no changes for the moment

```