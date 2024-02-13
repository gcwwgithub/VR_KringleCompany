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
```npm vite@latest``` - installs vite

Next install dependencies
```npm i```

This songjia cant really make any sense on why the dependencies was not already installed but oh well

To run project
```run dev```

Install babylon js
```npm i babylonjs@core```

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


### Create VR Experience and Async
```
const xr = scene.createDefaultXRExperienceAsync({
    uiOptions: {
        sessionMode: 'immersive-vr'
    }
})
```
The provided code is from Babylon.js and is used to create a default WebXR (Web Extended Reality) experience in a Babylon.js scene. Here's what each part of the code does:

scene.createDefaultXRExperienceAsync():
This method creates a default WebXR experience within the given scene. It enables support for WebXR in the browser and sets up the necessary components to allow users to experience the scene in virtual reality (VR) or augmented reality (AR) depending on their device and capabilities.

uiOptions: { sessionMode: 'immersive-vr' }:
This part of the code specifies options for the user interface (UI) of the XR experience. In this case, it sets the sessionMode option to 'immersive-vr', indicating that the XR session should be in immersive virtual reality (VR) mode. This means that the scene will be experienced in full VR mode, where users are fully immersed in the virtual environment.

xr variable:
The xr variable is assigned the result of the createDefaultXRExperienceAsync() method call. This variable likely represents the XR experience itself or contains information about the XR session, which can be used for further interaction or customization.

In summary, the code sets up a default WebXR experience in a Babylon.js scene, specifically configuring it to operate in immersive virtual reality (VR) mode. This allows users to interact with the scene using VR devices and experience it in a fully immersive virtual environment.

**Note: xr is a promise**
As part of async coding, other code below this will run without waiting for the xr to initalise. So if you do something with xr, u will crash or something. If you want to ensure it initialise properly u can add a await in front. BUt the function the code is called needs an async in front. Afterwards, you will be able to use xr as per normal.
So here is an example
```
// Create an async function to set up the Babylon.js scene
async function setupScene() {
    // Create a new Babylon.js engine
    const engine = new Engine(canvas, true);

    // Create a new Babylon.js scene
    const scene = new Scene(engine);

    // Create an XR experience asynchronously
    const xr = await scene.createDefaultXRExperienceAsync({
        uiOptions: {
            sessionMode: 'immersive-vr'
        }
    });
    // Run the render loop
    engine.runRenderLoop(() => {
        scene.render();
    });
}

// Call the async function to set up the scene when the window has finished loading
window.onload = async () => {
    await setupScene();
};
```
Just remember this, everytime you use async, it returns a Promise which means its a promise that a value will be eventually there so therefore you always need to ensure you declare await. Lets say you have a promise object, how do you get it to do stuff. Our code earlier has the answer
```
scenePromise.then((scene) => {
  engine.runRenderLoop(() => {
    scene.render();
  });
});
```
Then basically says, what should I do after the promise is fulfilled or in other words, what happens after the promise has been fulfilled and the object is initialised? It will call a callback which you see here is to runRenderLoop()

### Quick Debugging tip
The line ```(window as any).xr = xr;``` in TypeScript is a way to attach the xr variable to the global window object. By doing this, xr becomes accessible from anywhere in the web application, including the browser's console, which is particularly useful for debugging purposes.

Here's what this line of code does:

window: This is the global object in the context of the browser, representing the window in which the script is running.
as any: TypeScript is a statically typed superset of JavaScript. Using as any is a type assertion in TypeScript which tells the compiler to treat the window object as any type, effectively turning off type checking for this expression. This is done because window does not have a property xr by default, so you have to assert it to any to bypass the type checking system.
.xr = xr;: This assigns the xr variable (which presumably holds a reference to a WebXR experience created by scene.createDefaultXRExperienceAsync()) to a new property xr on the window object.
After running this line of code, you could open your browser's developer console and access the xr variable directly, which is useful for inspecting its properties and methods, debugging issues with your WebXR experience, or even manipulating the WebXR session in real-time. It effectively makes xr a global variable, which should generally be avoided in production code due to the potential for naming collisions and it being considered a bad practice, but for debugging, it's a useful shortcut.

### Morzilla Web XR Emulator
After you get on the web host, if you have the emulator, there will be an icon on the bottom right of the screen. You click on it and now you can see VR Mode. You can even move around a VR Headset on controllers as well

### AR Debugging
```
const xr = await scene.createDefaultXRExperienceAsync({
        uiOptions: {
            sessionMode: 'immersive-ar'
        }
    });
```
Then in the XR emulator, just change ur device into a phone

### Meta Quest Debugging
1. Create an organisation and then create a account
2. Enable USB Debugging but you must have an account with the developer mode enabled
3. Make sure you install adb so you can use ```adb devices``` in console to see the connected device
4. Use ```adb reverse``` to allow  the quest can access a local host website on the connected desktop through the cable

### Android Debugging
Same as above but connect the android phone instead

### IOS Debugging
Didnt watch hehe i swear to god if this chek test

Everything below is I didnt watch video to hear the explanation cause hehe
### Skybox
```
createSkybox(scene: Scene) {
  // Create a skybox mesh
  const skybox = MeshBuilder.CreateBox('skybox', { size: 1000 }, scene);

  // Create a skybox material
  const skyboxMaterial = new StandardMaterial('skybox-mat');

  // Disable backface culling for the skybox material
  skyboxMaterial.backFaceCulling = false;

  // Set the reflection texture of the skybox material to a cube texture
  skyboxMaterial.reflectionTexture = new CubeTexture('assets/textures/skybox', scene);
  skyboxMaterial.reflectionTexture.coordinatesMode = Texture.SKYBOX_MODE;

  // Set the diffuse and specular colors of the skybox material to black
  skyboxMaterial.diffuseColor = new Color3(0, 0, 0);
  skyboxMaterial.specularColor = new Color3(0, 0, 0);

  // Assign the skybox material to the skybox mesh
  skybox.material = skyboxMaterial;
}
```
In webpack, there is a setting in webpack.config.js where you need to set the static variable if its there to true to use static asssets.
Backface culling is a performance optimization that doesn't render the faces of a mesh that point away from the camera. Since the camera is inside the skybox, you want to disable backface culling to ensure all the inside faces of the cube are rendered.

The diffuse and specular colors of the skybox material are set to black. In the context of a skybox, these properties are typically set to black because the skybox usually doesn't need to reflect any light or have any shiny properties, as it represents distant objects like stars or clouds.

### Camera
```
createCamera(scene: Scene) {
  // const camera new ArcRotateCamera('arcCamera, Math.PI/5, Math.PI/2, 5, Vector3.Zero()),
  // scene):

  const camera = new UniversalCamera("uniCamera", new Vector3(0), scene);
  camera.attachControl(this.canvas, true);
}
```
This was the code they gave. There a commented out arc rotate camera there
The Universal Camera is a versatile camera that can be used for both touch and keyboard/mouse control schemes. The camera is given a name "uniCamera" and is initially positioned at the origin (0, 0, 0) in the 3D world.
The ArcRotateCamera automatically rotates around a target (in this case, Vector3.Zero() which is the origin of the scene) and is controlled by three parameters:

The key difference between UniversalCamera and ArcRotateCamera is their control scheme and behavior:

UniversalCamera: This is similar to a free camera or first-person shooter camera. It's controlled by WASD keys for movement and mouse for looking around.
ArcRotateCamera: This camera is automatically set to revolve around a target point and is typically controlled by dragging the mouse to rotate the camera around the target, and the mouse wheel to zoom in and out.
Depending on the type of interaction you want in your scene, you would choose the camera type that suits your needs. UniversalCamera is good for scenarios where you want the user to freely move around the scene, while ArcRotateCamera is excellent for scenarios where you want the user to orbit around a specific object or location.

### Lights
```
const hemisphericLight = new HemisphericLight('hemilight', new Vector3(-1, 1, 0), scene);
hemiLight.intensity = 0.5;
hemiLight.diffuse = new Color3(0, 0, 1);

const pointLight = new PointLight("pointLight", new Vector3(0, 1.5, 2), scene);
pointLight.intensity = 1;
pointLight.diffuse = new Color3(1, 0, 0);
```
Diffuse light is the light that is scattered in all directions off the surface it hits.

The HemisphericLight simulates light coming from above, much like the ambient light in the real world where the sky acts as a light source. This type of light has a direction but no specific source position. Gemini says Hemispheric lights simulate indirect lighting from the sky and ground.
The PointLight simulates a light bulb or a point source that emits light in all directions:

The Differences Between Hemispheric Light and Point Light:

Direction vs. Position: Hemispheric light is defined by a direction, meaning it does not have a specific point in space it originates from. It's assumed to be infinitely far away, similar to sunlight. Point light, on the other hand, is defined by its position in space, similar to a lamp.

Light Spread: Hemispheric light illuminates the scene uniformly and simulates a soft ambient effect that doesn't cast strong shadows. Point light emits light in all directions from its position and can cast shadows based on its relationship to objects in the scene.

Color: In this particular code, hemispheric light is given a blue diffuse color, which will tint the surfaces it illuminates with a blueish tone, while the point light is given a red diffuse color, which will tint illuminated surfaces red.

### Sky Dome 
```
createVideoSkyDome(scene: Scene) {
  const dome = new VideoDome(
    'videoDome',
    'assets/videos/bridge_360.mp4',
    {
      resolution: 32,
      size: 1000
    },
    scene
  );
}
```
Inside the function, it creates an instance of VideoDome, which is likely a class from Babylon.js or a custom class in the application. VideoDome is used to project a 360-degree video onto the inner surface of a dome that surrounds the entire scene, creating an immersive environment.

This one is Chatgpt say one ah
The object { resolution: 32, size: 1000 } sets the properties for the VideoDome:
resolution: 32 might refer to the number of segments used to render the dome, affecting the quality of the mesh onto which the video is projected.
size: 1000 likely sets the size of the dome in the scene's units.

### Inspector Shortcut
addInspectorKeyboardShortcut(scene: Scene) {
  window.addEventListener('keydown', e => {
    if (e.altKey && e.ctrlKey && e.key === 'I') {
      if (scene.debugLayer.isVisible()) {
        scene.debugLayer.hide();
      } else {
        scene.debugLayer.show();
      }
    }
  });
}
It defines an event listener that listens for keydown events on the window object.
When a key is pressed, it checks if the Alt key and Ctrl key are held down simultaneously, and the letter 'I' is the key that was pressed. This combination (Ctrl+Alt+I) acts as the shortcut to trigger the code block.
Inside the if-statement, it checks whether the debug layer of the scene is currently visible.
If the debug layer is visible, it will hide it by calling scene.debugLayer.hide().
If the debug layer is not visible, it will show it by calling scene.debugLayer.show().
Whats the debug layer?
In Babylon.js, the "scene debug layer", also commonly referred to as The Inspector, is a powerful visual debugging tool. It provides you with various functionalities to help you understand and troubleshoot your 3D scene. 

### Make the VE Responsive to Window Sizes
```
window.addEventListener('resize', () => {
  engine.resize();
});
```
This code snippet is adding an event listener to the window object, which listens for the resize event. This event is triggered whenever the browser window is resized.

How it's used:

The anonymous arrow function () => { engine.resize(); } is the event handler that gets called when the resize event occurs.
Inside the event handler, the resize method of the engine object is called. This method is typically provided by 3D engine libraries like Babylon.js or Three.js to handle the resizing of the rendering canvas. When the window is resized, the canvas needs to adjust its dimensions accordingly to ensure the 3D content is rendered correctly to the new window size.
When this event is called:

The resize event is called by the browser every time there is a change in the size of the viewport, which could happen for various reasons like changing the size of the browser window, rotating a mobile device, or when the browser window is maximized or minimized.
The purpose of calling engine.resize() is to make sure that the 3D scene's aspect ratio remains correct and that the scene does not get stretched or squished. It ensures that the rendering engine adjusts its internal projections to accommodate the new size of the canvas.

### Load Models
```
loadModel(scene: Scene) {
  SceneLoader.ImportMeshAsync('', 'assets/models/', 'H2O.glb', scene);
}
```
Here's what the function does:

SceneLoader is a static class in Babylon.js that provides functions to load scenes and meshes from various file formats.

ImportMeshAsync is a method that loads meshes, geometries, and materials defined in a .glb file format (which is the binary version of the GLTF format) into the provided scene.

The first argument is a blank string which means no specific mesh names are provided; thus, it will load all meshes from the file.

'assets/models/' is the directory path where the .glb file is located.

'H2O.glb' is the name of the 3D model file that will be loaded.

scene is the instance of the scene where the meshes will be added.

This function would be used to load a model named 'H2O.glb' from the 'assets/models/' directory into the provided Babylon.js scene. The loading is asynchronous, which means it won't block the rest of the code from running while the model is being loaded. This is typically desired behavior in web applications to maintain a responsive interface.

Once the promise returned by ImportMeshAsync is resolved, the loaded meshes will be present in the scene and can be manipulated or displayed according to the needs of the application.

**You need to add ts-loader in package.json and import bablyonjs-loaders in the ts files.**

### Tips on Async again?
```
loadModel(scene: Scene) {
  SceneLoader.ImportMeshAsync('', 'assets/models/', 'H2O.glb', scene).then(result => {
    const root = result.meshes[0];
    root.id = 'h2oRoot';
    root.name = 'h2oRoot';
    root.position = someVariable; // 'someVariable' is not defined in this snippet. This likely should be a Vector3 object.
    root.rotation = new Vector3(0, 0, Math.PI);
    root.scaling.setAll(1.5);
  });
}
```
This function loadModel is similar to the previous one in that it imports a 3D model into the given scene. However, this version of the function adds more steps after the model is loaded:

It uses .then on the promise returned by ImportMeshAsync to handle the result of the asynchronous operation. This part of the code will execute once the model has finished loading.
result.meshes[0] gets the first mesh from the loaded model. In the context of Babylon.js, a model can consist of one or several meshes. Here we assume that result.meshes[0] is the root mesh or the main mesh that other parts of the model are parented to.

The root mesh is given an ID and a name 'h2oRoot', which can be used to identify it within the scene.

root.position is being set to someVariable, which appears to be a placeholder for a Vector3 object representing the position where the mesh should be placed in the scene. Since someVariable isn't defined in the code snippet, it should be replaced with an actual Vector3 value or variable.

root.rotation is set to a new Vector3 object that represents the rotation of the mesh. In this case, it's rotated by Math.PI radians (180 degrees) around the Z-axis.

root.scaling.setAll(1.5) uniformly scales the mesh by a factor of 1.5 along all three axes.

The difference between this and the previous snippet is that after loading the model, this code snippet is also manipulating the root mesh by setting its ID, name, position, rotation, and scale. This allows for immediate customization of the model's properties once it has been loaded into the scene. The previous snippet didn't include these post-loading operations.



