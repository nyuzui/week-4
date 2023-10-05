## Link to my card on Vue: 
https://github.com/nyuzui/vue.git

## link to the hello world boiler plates;
1. sveltekit: https://github.com/nyuzui/sveltekit-boilerplate.git
2. angular: https://github.com/nyuzui/angular-boilerplate.git
3. react: https://github.com/nyuzui/create-react-app.git
4. vue: https://github.com/nyuzui/vite-vue.git


## 1.What are the similarities and what are the differences in repo structure? Find 5 similarities and 1 difference between each of the 4.
Similarities:
All have a source code directory for application code.
Use npm or Yarn for package management.
Involve a build/transpile process with configuration files.
Include routing capabilities.
Support CSS for styling.

Differences:
Angular uses TypeScript (.ts files).
React uses JSX (.jsx or .tsx files).
SvelteKit uses .svelte files for components.
Vue uses single-file components (.vue).

## 2.Look at the syntax of a js/template file from each. Identify something vanilla in each and something library specific in each (8 total items here)?
**React:**
```jsx
import logo from './logo.svg';
import './App.css';

function App() {
  // Something Vanilla (JavaScript): Importing a static image and using it in JSX.
  // The alt attribute in the <img> tag is also vanilla HTML.
  
  return (
    <div className="App">
      <header className="App-header">
        <img src={logo} className="App-logo" alt="logo" />
        
        // Something React-specific: JSX syntax and component structure.
        
        <p>
          Edit <code>src/App.js</code> and save to reload.
        </p>
        <a
          className="App-link"
          href="https://reactjs.org"
          target="_blank"
          rel="noopener noreferrer"
        >
          Learn React
        </a>
      </header>
    </div>
  );
}

export default App;
```

**Angular:**

```javascript
import { platformBrowserDynamic } from '@angular/platform-browser-dynamic';
import { AppModule } from './app/app.module';

platformBrowserDynamic().bootstrapModule(AppModule)
  .catch(err => console.error(err));

// Something Vanilla (JavaScript): Standard JavaScript imports and function calls.

// Something Angular-specific: Using Angular's module and platformBrowserDynamic to bootstrap the application.
```

**SvelteKit:**

```javascript
// Something Vanilla (JavaScript): Importing a module and defining an object.
const nextConfig = {}

module.exports = nextConfig;

// Something SvelteKit-specific: This code appears to be related to configuration, and SvelteKit uses its own setup and build process.
```

**Vue:**

```javascript
import { env } from '$env/dynamic/private';

// Something Vanilla (JavaScript): Importing a module using ES6 import syntax.

/** @type {import('./$types').LayoutServerLoad} */
export function load() {
	// Something Vue-specific: Vue's composition API and TypeScript annotations.
	return { analyticsId: env.VERCEL_ANALYTICS_ID };
}
```

In each of these examples:

**Vanilla (Generic JavaScript)** represents code that doesn't rely on the specific framework or library and can be used in any JavaScript project.

**Library/Framework-Specific** elements are those that rely on the particular syntax, conventions, or features of the respective framework or library. These elements are unique to their respective ecosystems.

## 3.Review package.json - What is common amongst them, what's different? What commands can we run? Try to run all the different commands in the repo for each project.
**Common Elements:**

1. All `package.json` files contain project name and version information.
2. They list dependencies and devDependencies.
3. They define scripts for various tasks.

**Differences:**

1. Framework-specific dependencies are unique to each framework.
2. Framework-specific scripts might differ.
3. Custom scripts tailored to the project can vary.

**Commands to Run (Examples):**

**Angular**:
- Start: `ng serve`
- Build: `ng build`
- Test: `ng test`

**React**:
- Start: `npm start` or `yarn start`
- Build: `npm run build` or `yarn build`
- Test: `npm test` or `yarn test`

**SvelteKit**:
- Start: `npm run dev` or `yarn dev`
- Build: `npm run build` or `yarn build`
- Testing may vary based on project setup.

**Vue**:
- Start: `npm run serve` or `yarn serve`
- Build: `npm run build` or `yarn build`
- Test: `npm run test` or `yarn test`

## 4.Rank order these for readability / ease of your understanding and give a brief justification as to why you thought 1 was the easiest and 4 was the hardest to understand (or that you didn't understand!)
i thought that vue was the simplest one to use because of the way it was laid out compared to the rest. the html/css/js was laid out clearly and it wasnt very difficult to figure out how to customize it compared to the rest. 
