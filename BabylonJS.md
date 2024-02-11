# VR_KringleCompany
Great Asset, Great Great Asset

## BablyonJS
I dont know what the fuck notes to do here. Take note week 4 have some babylon js questions and notes there as well

### Node.js
Node.js is an open-source, cross-platform JavaScript runtime environment that allows developers to execute JavaScript code outside of a web browser. It uses the V8 JavaScript engine from Google Chrome to execute JavaScript code on the server-side, enabling the development of scalable and high-performance network applications.

Some key features of Node.js include:

Asynchronous and Event-Driven: Node.js uses an event-driven, non-blocking I/O model, which allows it to handle multiple connections concurrently without getting blocked by I/O operations. This makes it well-suited for building real-time applications like chat servers, streaming services, and APIs.

NPM (Node Package Manager): npm is the default package manager for Node.js and the largest software registry in the world. It allows developers to discover, share, and reuse packages of code, making it easy to integrate third-party libraries, frameworks, and tools into Node.js projects.

Server-Side Development: Node.js is commonly used for server-side development, including building web servers, RESTful APIs, microservices, and server-side rendering for web applications.

JavaScript Ecosystem: Node.js enables developers to use JavaScript for both client-side and server-side development, providing a unified language and ecosystem across the entire application stack.

### npm
npm (Node Package Manager) is a command-line tool used for managing Node.js packages and dependencies. It comes bundled with Node.js installation and provides a convenient way to install, update, and remove packages from a Node.js project. npm allows developers to specify dependencies in a package.json file and automatically installs them along with their dependencies, simplifying the process of managing project dependencies and ensuring consistent development environments across different machines.
Songjia just says its a way to get your packages into your projecct


As a Babylon.js user, understanding Node.js and npm is important for several reasons:

Development Workflow: Node.js and npm facilitate a streamlined development workflow for Babylon.js projects. You can use npm to manage dependencies, including Babylon.js itself and any additional libraries or tools you may need for your project.

Third-Party Libraries: Babylon.js is often used alongside other JavaScript libraries and frameworks to enhance functionality or simplify development tasks. npm provides access to a vast ecosystem of third-party libraries and packages that you can easily integrate into your Babylon.js projects.

Build Tools: Node.js and npm offer various build tools and utilities that can help optimize and automate your Babylon.js project's development process. For example, you can use npm scripts to automate tasks such as bundling, minification, testing, and deployment.

Server-Side Rendering: Node.js enables server-side rendering (SSR) of Babylon.js applications, allowing you to pre-render 3D scenes on the server and deliver them to clients for improved performance and SEO (Search Engine Optimization).

Community and Support: Node.js and npm have large and active communities of developers who contribute to open-source projects, share knowledge, and provide support. Being familiar with Node.js and npm allows you to tap into this community for assistance, resources, and collaboration.

Full-Stack Development: With Node.js, you can build full-stack applications that combine server-side logic written in JavaScript with client-side Babylon.js code. This allows for a unified development experience and easier integration between the frontend and backend components of your application.

Overall, understanding Node.js and npm enhances your capabilities as a Babylon.js user, enabling you to leverage a wider range of tools, libraries, and resources to build immersive 3D experiences more efficiently and effectively.

Commands
npm init - Creates a package.json
npm init --yes - Does the same above but answers every single questions that npm ask with yes
npm vite@latest - installs vite

### package.json
package.json is a file used in Node.js projects to manage project dependencies, scripts, metadata, and other configuration settings. It is a standard file in Node.js projects and is typically located in the root directory of the project. Here's what you'll commonly find in a package.json file:

Project Metadata: Information about the project such as its name, version, description, author, license, etc. This metadata helps other developers understand the purpose and characteristics of the project.

Dependencies: Lists of packages or modules that the project depends on for its functionality. Dependencies can be categorized into two types: dependencies and devDependencies. Dependencies listed under dependencies are required for the application to run, while those under devDependencies are only needed for development purposes.

Scripts: Custom scripts that can be executed using the npm or yarn command line interface. These scripts can perform various tasks such as running tests, building the project, starting the development server, etc. Common script names include start, test, build, dev, etc.

Version Control: Information related to version control systems such as Git repositories, including URLs for remote repositories, branch information, etc.

Configuration Settings: Additional configuration settings specific to the project or its dependencies. These settings can include options for compilers, linters, bundlers, test frameworks, etc.
```
{
  "name": "my-project",
  "version": "1.0.0",
  "description": "A sample Node.js project",
  "main": "index.js",
  "scripts": {
    "start": "node index.js",
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "keywords": [
    "node",
    "sample",
    "project"
  ],
  "author": "John Doe",
  "license": "MIT",
  "dependencies": {
    "express": "^4.17.1",
    "lodash": "^4.17.21"
  },
  "devDependencies": {
    "nodemon": "^2.0.15"
  }
}

```

### package lock.json
package-lock.json is a file generated by npm (Node Package Manager) when you run npm install to install dependencies for a Node.js project. It serves as a lockfile that records the exact versions of all packages and their dependencies that were installed. This ensures that subsequent installs of the project, whether by the same developer or by others, will use the exact same versions of dependencies, thus guaranteeing reproducibility and consistency across different environments.

Here's what package-lock.json typically contains:

Dependency Tree: The file contains a detailed dependency tree, listing all the packages that were installed, along with their versions. It records both direct dependencies (those listed in your package.json) and their transitive dependencies.

Exact Versions: For each package, package-lock.json specifies the exact version that was installed, including any sub-dependencies. This prevents npm from installing different versions of the same package in different environments, which could lead to compatibility issues.

Integrity Hashes: package-lock.json includes integrity hashes for each package, which are cryptographic hashes computed from the package's contents. These hashes ensure that the installed packages have not been tampered with or corrupted.

Metadata: Additional metadata such as URLs for package tarballs, version ranges, and other information necessary for installing and resolving dependencies.

The presence of package-lock.json is particularly important in collaborative projects or when deploying applications to production environments. It helps ensure that all developers working on the project are using the same versions of dependencies and reduces the likelihood of unexpected behavior due to version mismatches.

It's worth noting that package-lock.json should be committed to version control along with your other project files (package.json, source code, etc.) to ensure that everyone working on the project has access to the same dependency versions. However, it's generally recommended to exclude the node_modules directory from version control, as the dependencies themselves can be quite large and are better managed through npm or yarn.

### index.html

index.html is a commonly used filename for the main HTML file in a web application or website. It serves as the entry point for the web application and typically contains the structure and content of the initial page that users see when they visit the website.

The index.html file often includes the following components:

HTML Structure: The basic structure of an HTML document, including the <html>, <head>, and <body> tags.

Metadata: Metadata elements such as <meta> tags for specifying character encoding, viewport settings, authorship information, and other metadata that browsers and search engines use to interpret and display the page correctly.

Title: The <title> element, which specifies the title of the web page displayed in the browser's title bar or tab.

Content: The main content of the web page, including text, images, links, forms, and other HTML elements that make up the user interface of the website.

Script and Style References: References to external JavaScript files (<script> tags) and CSS stylesheets (<link> tags) used to add functionality and styling to the web page.

JavaScript Code: Inline JavaScript code or script blocks within the <script> tags for adding interactivity, event handling, and dynamic behavior to the web page.

The index.html file is often located in the root directory of a web project and is served by the web server as the default document when users access the website's domain or root URL (e.g., http://example.com).

In summary, index.html is the main HTML file of a web application or website, containing the structure and content of the initial page that users see when they visit the site. It plays a crucial role in defining the user interface and functionality of the web application.

For babylon js, since the application is hosted on the web, treat the html as how the app will look like. Its like making a website where you add elements to the html page and then you see ui elements appear

### tsconfig.json

A tsconfig.json file is a configuration file used in TypeScript projects to specify compiler options and settings for the TypeScript compiler (tsc). This file helps manage various aspects of the TypeScript project, such as compiler behavior, output directory, module resolution, and more.

Here are some common settings that can be configured in a tsconfig.json file:

Compiler Options: Compiler options control how TypeScript code is compiled into JavaScript. These options include settings such as target ECMAScript version, module system (e.g., CommonJS, AMD, ES6), strict type checking, source map generation, and more.

File Inclusion/Exclusion: Specify which files should be included or excluded from compilation. You can use the include and exclude properties to specify file paths or glob patterns to include or exclude files from compilation.

Output Options: Configure the output directory and file naming conventions for compiled JavaScript files. Options include setting the output directory (outDir), generating declaration files (declaration), emitting ECMAScript modules (esModuleInterop), and more.

Module Resolution: Configure how TypeScript resolves module imports. Options include specifying module resolution strategy (moduleResolution), root directories for module resolution (baseUrl), path mappings (paths), and more.

Type Checking Options: Control the strictness of type checking and error reporting. Options include enabling strict mode (strict), enforcing null checks (strictNullChecks), enabling strict property initialization (strictPropertyInitialization), and more.

Source Map Generation: Specify whether to generate source maps for compiled JavaScript files (sourceMap) and configure source map options.

Project References: Define references to other TypeScript projects or projects' outputs. This feature allows you to create multi-project setups and manage dependencies between projects.

A tsconfig.json file is typically located in the root directory of a TypeScript project, and TypeScript automatically detects and uses this file when compiling the project. Having a tsconfig.json file helps ensure consistent compilation settings across different environments and simplifies project setup and maintenance.

Here's a minimal example of a tsconfig.json file:
```
{
  "compilerOptions": {
    "target": "es5",
    "module": "commonjs",
    "strict": true
  },
  "include": [
    "src/**/*.ts"
  ],
  "exclude": [
    "node_modules"
  ]
}
```

### Vite
First install vite in your project
npm vite@latest - installs vite

Next install dependencies
npm i

This songjia cant really make any sense on why the dependencies was not already installed but oh well

To run project
run dev

Install babylon js
npm i babylonjs@core

### Bablylon JS Code Beginning
The beginning code is like this
```
// main.ts
import { Engine } from "@babylonjs/core";
import { App } from "./app";

const canvas = document.getElementById("renderCanvas") as HTMLCanvasElement;
const engine = new Engine(canvas, true);
const app = new App(engine);

const scenePromise = app.createScene();
scenePromise.then((scene) => {
  engine.runRenderLoop(() => {
    scene.render();
  });
});

// app.ts
import { Engine, Scene } from "@babylonjs/core";

export class App {
  private engine: Engine;

  constructor(engine: Engine) {
    this.engine = engine;
  }

  async createScene(): Promise<Scene> {
    const scene = new Scene(this.engine);
    scene.createDefaultCameraOrLight()l;
    return scene;
  }
}
```
There was a index.html file earlier right, in that file, sonjia added a canvas file to the html and in the main.ts, he gets the canvas. The result is when he loads the web host, you will see a black image representing the canvas. 

### Babylonjs Canvas
```
const canvas = document.getElementById('renderCanvas') as HTMLCanvasElement;

const ctx = canvas.getContext('2d');
ctx.font = '50px Arial';

ctx.fillText('Hello XR', 50, 50);
```
The getContext('2d') call retrieves the 2D rendering context for the specified canvas element (renderCanvas). The '2d' argument indicates that the rendering context being requested is for 2D drawing operations.

Once the rendering context (ctx) is obtained, it provides methods and properties that allow you to perform various drawing operations on the canvas, such as drawing shapes, text, images, and applying transformations.

### Create a Sphere
```
const scene = new Scene(this.engine);  

scene.createDefaultCameraOrLight();

const sphere = MeshBuilder.CreateSphere('sphere', { diameter: 1.3 }, scene); 

sphere.position.y = 1; 
sphere.position.z = 5; 
```

### Create Text
```
const helloPlane = MeshBuilder.CreatePlane('hello plane', { size: 15 });

helloPlane.position.y = 0;
helloPlane.position.z = 5;


const helloTexture = AdvancedDynamicTexture.CreateForMesh(helloPlane);

const helloText = new TextBlock('hello');
helloText.text = 'Hello XR';

helloText.color = 'purple';
helloText.fontSize = 50;


```
```MeshBuilder.CreatePlane('hello plane', { size: 15 });```
This line creates a plane mesh named 'hello plane' with a size of 15 units. This plane will serve as the background for displaying the text.

```const helloTexture = AdvancedDynamicTexture.CreateForMesh(helloPlane); ```
This line creates an advanced dynamic texture associated with the plane mesh. AdvancedDynamicTexture is a Babylon.js feature that allows for rendering 2D elements onto 3D objects.

```helloTexture.addControl(helloText);```
This adds the TextBlock element (containing the text 'Hello XR') to the advanced dynamic texture associated with the plane mesh. As a result, the text will be rendered onto the plane mesh in the 3D scene.
