# Conference Speaker App

A React app that manages speakers for a code camp. It is the result of completing [Designing React Components](https://app.pluralsight.com/library/courses/react-components-designing) on Pluralsight.

Conference Speaker App concerns the following: designing better components; managing state in a component hierarchy; 
asynchronously updating state via custom hooks; using React Context and the useContext Hook for component data sharing;
building a local REST server supporting CRUD poerations with the NextJS API Routes; 
mastering performance monitoring, error reporting, and debugging of Components; and 
using higher order components and render props.

The course taught how to architect and build independent components in React that seamlessly work together to present a consistent view across the web app. It covered ensuring just the right components re-render as the data in the application changes, applying seperation of concerns to building React components, various primitive methods for sharing data and methods between components, using Context for shared information and using custom hooks for advanced state management, and leveraging re-usability.

## Getting Started
1. **Install [Node 18](https://nodejs.org)**
2. **Clone this repository** 
```
git clone https://github.com/g-esco101/conference-speaker-app.git
```
3. **Change to root directory**
```
cd conference-speaker-app
```
4. **Install Node Packages with Dependencies**
```
npm install
```
5. **Run the app**
```
npm run dev
```

## Building the app for production
```
npm run build
npm run start
```