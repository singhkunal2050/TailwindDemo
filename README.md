
# Learing Tailwind CSS with Building a Simple LAnding Page

## Steps 

- Inititialised npm
- Installed tailwind
- Created CSS Folder in root 
- Added tailwind directives in the style.css
- Added Tailwind Config File
- Added PosCSS-Cli and AutoPrefixer node modules for building css with tailwind
- Create Post CSS Config File
- Adding Build script in package.json

### Installation

    npm init -y
    npm install tailwindcss

### Add Tailwind directives in root css file 

    @tailwind base;
    @tailwind components;
    @tailwind utilities;

### Added Tailwind Config File
    PS O:\Practicals\JamstackProjects\TailwindDemo> npx tailwindcss init
    tailwindcss 1.9.6
    ✅ Created Tailwind config file: tailwind.config.js


### Adding two more dependencies
     npm install postcss-cli autoprefixer

### Create POST CSS Config file in root
    module.exports = {
        plugins :[
            require('tailwindcss'),
            require('autoprefixer'),
        ]
    }

### Adding Build script in package.json
    "scripts": {
        "build" : "postcss css/style.css -o build/style.css"
    },



