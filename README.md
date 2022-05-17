# Conference Speaker App

A React app that manages speakers for a code camp. It is the result of completing the [Designing React Components](https://app.pluralsight.com/library/courses/react-components-designing) course on Pluralsight.

Conference Speaker App concerns the following: designing better components; managing state in a component hierarchy; 
asynchronously updating state via custom hooks; using React Context and the useContext Hook for component data sharing;
building a local REST server supporting CRUD operations with the NextJS API Routes; 
mastering performance monitoring, error reporting, and debugging of components; and 
using higher order components and render props.

The course taught how to architect and build independent components in React that seamlessly work together to present a consistent view across the web app. It covered ensuring just the right components re-render as the data in the application changes, applying seperation of concerns to building React components, various primitive methods for sharing data and methods between components, using Context for shared information and using custom hooks for advanced state management, and leveraging re-usability.

## Technology
- Node.js version 18
- React 
- Next.js  

## Getting Started
1. Install [Node 18](https://nodejs.org) (I recommend using nvm - node version manager - to switch between versions of node)
2. Clone this repository
```
git clone https://github.com/g-esco101/code-camp-speakers-app.git
```
3. Change to root directory
```
cd code-camp-speakers-app
```
4. Install node packages with dependencies
```
npm install
```
If this gives you an error regarding the dependencies, use the following command
```
npm install --force
```
5. Run the app
```
npm run dev
```

## Building the app for production
1. Build the app
```
npm run build
```
2. Run the app
```
npm run start
```


## Creating project from an empty directory
This section is intended for people taking the course and wish to create the project from an empty directory. It uses the latest versions of the tools/dependencies instead of using the versions in the course.

- Make a new directory to use as the main directory for the project (I named mine code-camp-speakers-app):
```
mkdir code-camp-speakers-app
```

- Move into this directory:
```
cd code-camp-speakers-app
```

- Initialize the project (this will create the package.json file):
```
npm init -y
```

- Install dependencies:
```
npm install react react-dom next
```

- Add these scripts to the package.json file using your IDE or text editor:
```
  "scripts": {
    "dev": "next",
    "build": "next build",
    "start": "next start"
  }
```

- Nextjs has file based routing built into it: Any js file that you put into your pages directory, will get executed when the user browses to the root of your website followed by the name of that js file. Create the pages directory and add a file named index.js file:
```
mkdir pages
```
index.js
```
const IndexPage = () => {
    return (
        <div> Bonjour la monde</div>
    );
}
export default IndexPage;
```

- At this point, you can run the app:
```
npm run dev
```

- In the project root directory (code-camp-speakers-app), add the public directory from the instructor's public. Webpack will serve your contents from this directory. It is essentially the root of the web project and contains these directories (static assets): css and images.

- Copy the _document.js file from the instructor's pages directory into your pages directory. This file acts like a template for all your React pages, such that what is mentioned in the Head section is pulled into all your site pages, e.g., bootstrap, fontawesome icons, fonts from google, and a custom css file. 

- Copy the instructor's SpeakerData.js file into the root of the project (code-camp-speakers-app). It contains data that we will display throughout the course. 

- Now you can begin coding the app! Run the app:
```
npm run dev
```

-- You can add place holders using the react-placeholder package:
```
npm install react-placeholder
```
