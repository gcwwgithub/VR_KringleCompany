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

### GUI Controls?
```
createText(scene: Scene) {
  const helloPlane = MeshBuilder.CreatePlane("hello plane", { width: 2.5, height: 1 }, scene);
  helloPlane.position.y = 0;
  helloPlane.position.z = 5;
  
  const helloTexture = AdvancedDynamicTexture.CreateForMesh(helloPlane, 250, 100, false);
  helloTexture.background = "white";

  const helloText = new TextBlock("hello");
  helloText.text = "Hello XR";
  helloText.color = "purple";
  helloText.fontSize = 50;

  helloTexture.addControl(helloText);
}
```
The function provided is a basic example of how to create simple GUI (Graphical User Interface) controls in a Babylon.js 3D scene. Here's how it aligns with GUI creation:

AdvancedDynamicTexture: This is a special kind of texture that allows you to overlay GUI elements on top of a 3D scene or attach them to a specific mesh, like the plane in this case. This texture acts as a canvas for GUI controls.

TextBlock: This is a GUI control for displaying text. It's a fundamental element in any GUI system and can be used for labels, buttons, or any interactive text element.

Adding the TextBlock to the Texture: The helloTexture.addControl(helloText); line adds the TextBlock to the AdvancedDynamicTexture, which means the text will appear on the plane in the 3D world.

This setup is indeed a simple example of GUI in a 3D application. Babylon.js also supports more complex GUI elements, such as buttons, sliders, input fields, etc., which can be layered together to create a rich user interface. The GUI in Babylon.js is particularly useful for VR or AR scenarios where traditional HTML-based interfaces may not be suitable.

The code is the same above with slight differences. In essence, the main functional difference is the size of the plane and the specified dimensions for the AdvancedDynamicTexture in the second snippet, which are not provided in the first. The explicit background color set for the texture in the second snippet is also a notable difference, as it changes the visual appearance of the text's backdrop.

### GUI Interactions
```
helloText.onPointerUpObservable.add(eventData => {
  alert('Hello Text at:\n X: ' + eventData.x + '\n Y: ' + eventData.y);
});

helloText.onPointerDownObservable.add(() => {
  this.sound.play();
});
```
The first one adds an event listener to the onPointerUpObservable of the helloText TextBlock. When the pointer (usually a mouse or touch input) is released over the text block, the provided callback function is executed. The callback function shows a browser alert with the x and y position of the pointer when the event was triggered.

The second one adds an event listener to the onPointerDownObservable of the helloText. When the pointer is pressed down over the text block, the provided callback function is executed. In this callback, this.sound.play(); is called, which implies that there is a sound property on the same context (this) where the function is defined, and its play method is invoked. Assuming this.sound refers to an audio object, this would start playing the sound.

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

### Animations
```
createAnimation(scene: Scene, model: AbstractMesh) {
  const animation = new Animation(
    'rotationAnim',
    'rotation',
    30,
    Animation.ANIMATIONTYPE_VECTOR3,
    Animation.ANIMATIONLOOPMODE_CYCLE
  );

  const keyframes = [
    { frame: 0, value: new Vector3(0, 0, 0) },
    { frame: 30, value: new Vector3(0, 2 * Math.PI, 0) }
  ];

  animation.setKeys(keyframes);

  model.animations = [];
  model.animations.push(animation);

  scene.beginAnimation(model, 0, 30, true);
}
```
createAnimation is a function that takes a Scene and an AbstractMesh object as arguments. This function is likely part of a Babylon.js application, where Scene represents the 3D environment and AbstractMesh represents a mesh within that scene.

An Animation object is instantiated with the name 'rotationAnim'. It is configured to animate the 'rotation' property of the mesh. The 30 specifies the frame rate, indicating how many frames per second the animation will run.

Animation.ANIMATIONTYPE_VECTOR3 indicates that the property being animated, rotation in this case, is a Vector3 type, which is a three-dimensional vector representing Euler angles for rotation.

Animation.ANIMATIONLOOPMODE_CYCLE sets the animation to loop continuously.

The keyframes array defines the keyframes for the animation:

The first keyframe at frame: 0 sets the initial rotation value to (0, 0, 0).
The second keyframe at frame: 30 sets the rotation value to (0, 2 * Math.PI, 0), which represents a full 360-degree rotation around the Y-axis.
animation.setKeys(keyframes); assigns the keyframes to the animation, which tells the animation object when and how to interpolate the mesh's rotation.

model.animations = []; initializes the animations array property of the model to an empty array. This ensures that any previous animations are removed and the mesh is ready for new animations.

model.animations.push(animation); adds the newly created animation to the model's animations array.

scene.beginAnimation(model, 0, 30, true); starts the animation on the model. It specifies that the animation should start at frame 0, end at frame 30, and the true argument indicates that the animation should loop.

The outcome of this code is that the mesh provided as model will rotate around the Y-axis one full turn (360 degrees) in a loop. The duration of this rotation is implicitly defined by the frame rate and the frame numbers given; since there are 30 frames and the frame rate is 30, this implies a one-second duration for the full rotation cycle.

Then in load model you add this
```
loadModel(scene: Scene) {
  SceneLoader.ImportMeshAsync('', 'assets/models/', 'H2O.glb', scene).then(result => {
    const root = result.meshes[0];
    root.id = 'h2oRoot';
    root.name = 'h2oRoot';
    root.position = someVariable; // 'someVariable' is not defined in this snippet. This likely should be a Vector3 object.
    root.rotation = new Vector3(0, 0, Math.PI);
    root.scaling.setAll(1.5);
    this.createAnimation(scene,root)
  });
}
```
### Particle System
```
createParticles(scene: Scene) {
  const particleSystem = new ParticleSystem('particles', 5000, scene);
  particleSystem.particleTexture = new Texture('assets/textures/flare.png', scene);

  particleSystem.emitter = new Vector3(0, 0, 0);
  particleSystem.minEmitBox = new Vector3(0, 0, 0);
  particleSystem.maxEmitBox = new Vector3(0, 0, 0);

  particleSystem.color1 = new Color4(0.7, 0.8, 1.0, 1.0);
  particleSystem.color2 = new Color4(0.3, 0.5, 1.0, 1.0);
  particleSystem.blendMode = ParticleSystem.BLENDMODE_ONEONE;

  particleSystem.minSize = 0.01;
  particleSystem.maxSize = 0.05;
  
  particleSystem.minLifeTime = 0.3;
  particleSystem.maxLifeTime = 1.5;
  
  particleSystem.emitRate = 1500;
  
  particleSystem.direction1 = new Vector3(-1, 8, -1);
  particleSystem.direction2 = new Vector3(1, 8, -1);
  
  particleSystem.minEmitPower = 0.2;
  particleSystem.maxEmitPower = 0.8;
  particleSystem.updateSpeed = 0.01;
  
  particleSystem.gravity = new Vector3(0, -9.8, 0);
  particleSystem.start();
}
```
Defines a function createParticles that takes a Babylon.js Scene object as a parameter.

Creates a new ParticleSystem within the provided scene. The system is named 'particles', and it's configured to use a maximum of 5000 particles.

Sets the particle texture to a flare image, 'assets/textures/flare.png', which will be used for each particle in the system.

Sets the emitter of the particle system to the origin point (0, 0, 0). This is the point in space where particles will be emitted.

The minEmitBox and maxEmitBox are set to (0, 0, 0), which means that particles will be emitted from a single point. If these vectors were different, particles would be emitted from random positions within the defined box area.

Defines two colors for the particles. color1 is a pale blue with full alpha (opaque), and color2 is a darker blue, also fully opaque. These colors will likely be interpolated between over the lifetime of the particles.

Sets the blendMode to BLENDMODE_ONEONE, which defines how particles blend with the background and each other. This particular mode is additive blending, where the colors of the particles are added to the colors of the background, creating a glowing effect.

minSize and maxSize set the minimum and maximum size of each particle. Particles will be randomly sized between these values when they are created.

minLifeTime and maxLifeTime set the minimum and maximum lifetime of each particle in seconds. Each particle will last for a random time between these values before it's recycled.

emitRate is the number of particles to emit per second.

direction1 and direction2 define the initial direction vectors for particle emission. Particles will be emitted with a random direction between these two vectors. This creates a spread of particles that can simulate effects like explosions or fountains.

minEmitPower and maxEmitPower define the range of speeds at which particles are emitted from the emitter.

updateSpeed is the time step used to update the particle system, effectively controlling the simulation's precision and smoothness.

gravity is a vector that represents the gravity applied to the particles. In this case, it's set to the Earth's gravity, pulling the particles downward along the Y-axis.

start is the method that starts the particle system, causing it to begin emitting particles.

### Sound
```
addSounds(scene: Scene) {
  const music = new Sound("music", "assets/sounds/hello-xr.mp3", scene, null, { loop: true, autoplay: false });
  const sound = new Sound("sound", "assets/sounds/button.mp3", scene, null);
}
```
This function, addSounds, is designed to add audio to a Babylon.js scene. The function is defined to take one parameter, scene, which is a Babylon.js Scene object where the sounds will be added.

Within the function:

A new Sound object named "music" is created with a source file located at "assets/sounds/hello-xr.mp3". The sound is added to the scene. The fourth parameter is set to null, which means no callback is used for when the sound is ready to play. The final parameter is an options object where loop: true means the sound will play in a loop, and autoplay: false means the sound will not play automatically when created.

Another Sound object named "sound" is created with a source file located at "assets/sounds/button.mp3" and added to the scene. The fourth parameter is null, and since no options object is provided, this sound will use the default settings (it will not loop and will not autoplay, assuming these are the defaults).

In summary, this function initializes two sounds for the scene: one for background music that loops (but does not autoplay), and another for a button press effect (with default playback settings). These sounds can be controlled programmatically to play, stop, pause, etc., within the application.

### Constructor
You can split up huge classes into components so something like this
```
export class TextPlane {
    constructor(
        name: string,
        width: number,
        height: number,
        x: number,
        y: number,
        z: number,
        text: string,
        backgroundColor: string,
        textColor: string,
        fontSize: number
    ) {
        // Create the plane mesh
        const textPlaneMesh = BABYLON.MeshBuilder.CreatePlane(name, { width, height }, scene);

        // Position the plane
        textPlaneMesh.position.set(x, y, z);

        // Create a dynamic texture for the plane
        const planeTexture = new BABYLON.AdvancedDynamicTexture.CreateForMesh(
            textPlaneMesh,
            width,
            height,
            false
        );

        // Set the background color of the texture
        planeTexture.background = backgroundColor;

        // Create a text block to display the text on the plane
        const planeText = new BABYLON.TextBlock(name + " text", planeTexture);
        planeText.text = text;
        planeText.fontSize = fontSize;
        planeText.color = new BABYLON.Color4(1, 1, 1, 1); // White text color

        // Rotate the text block to face the camera
        planeText.rotation.y = -Math.PI / 2;
    }
}

```
You are recommended to create a file for this in the same folder as all your classes then in the code write this
```
export * from './text-plane'
export * from './rigidbody'
```
Then in the main code just do
'''
import {} from './components/meshes'
'''

### Interfaces?
export interface HelloMesh {
    scene : Scene;
    mesh : Mesh;
    label : TextPlane;
}    

export class HelloSphere extends AbstractMesh implements HelloMesh {
    scene : Scene;
    mesh : Mesh;
    label : TextPlane;

constructor(name: string, options : {diameter : number}, scene : Scene)
{
  super(name,scene);
  this.scene = scene;
  this.mesh = MeshBuilder.CreateSphere("Hi". options, scene);
  this.mesh.material = new StandardMaterial("Mat", scene);
  this.label = new TextPlane(....... some parameters here)
  this.addChild(this.label.mesh);
}

  
}

### Create Ground
```
// ground
const groundMaterial = new StandardMaterial("ground material", scene);

//back will not be rendererd
groundMaterial.backFaceCulling = true;
groundMaterial.diffuseTexture = new Texture('assets/textures/grass.png',

scene);
const ground = MeshBuilder.CreateGround("ground", {width: 12, height: 12}, scene);

ground.material = groundMaterial;
ground.position.set(0, -1, 8);
```

### Behaviours to create interaction
```
const pointerDragBehavior = new PointerDragBehavior({
               dragPlaneNormal: new BABYLON.Vector3(0, 1, 0), // Makes the drag plane parallel to the y-axis

});
pointerDragBehavior.onDragStartObservable.add(evtData => {
                              console.log("drag start: pointer id " + evtData.pointerId);
                              console.log(evtData);

});
sphere.addBehavior(pointerDragBehavior);
```
Pointer Drag Behavior: A pointer drag behavior is created using the PointerDragBehavior class. This class allows you to drag meshes around the scene using a mouse or pointer. In this code, the dragPlaneNormal property is set to new BABYLON.Vector3(0, 1, 0), which makes the drag plane parallel to the y-axis. This means that the mesh can only be dragged up and down.

onDragStartObservable: This observable is used to listen for drag events. In this code, an event handler is added to the onDragStartObservable using the add method. The event handler logs the pointer ID and event data to the console when the dragging starts.

Adding the behavior to the sphere: The pointerDragBehavior is then added to the sphere mesh using the addBehavior method. This enables the drag functionality for the sphere.
### Actions
```
private initActions() {
const actionManager = (this.actionManager = new ActionManager(this.scene));

actionManager.isRecursive = true;

const light = this.scene.getLightById("default light");
actionManager
 .registerAction(new InterpolateValueAction(
        ActionManager.OnPickTrigger,
        light,
        "diffuse",
        Color3.Black(),
        1000
        )
       )
      .then(
          new InterpolateValueAction(
              ActionManager.OnPickTrigger,
              light,
              "diffuse",
              Color3.White(),
              1000
             )
         };

actionManager.registerAction(
    new InterpolateValueAction(
        ActionManager.OnPickDownTrigger,
        this,
        "scaling",
        new Vector3(2, 2, 2),
        1000,
        new PredicateCondition(actionManager, () => {
            return light.diffuse.equals(Color3.Black());
        })
    )
);

const otherMesh = this.scene.getMeshById("sphere");
actionManager.registerAction(
    new SetValueAction(
        {
            trigger: ActionManager.OnIntersectionEnterTrigger,
            parameter: {
                mesh: otherMesh,
                usePreciseIntersection: true,
            },
        },
        this.mesh.material,
        "wireframe",
        true
    )
);

}
```
To use this function, just call it in the constructor 
Here is the explanation of the code
Light Color Change on Pick:
Action 1: Fades the light (identified as "default light") to black (Color3.Black()) over 1000 milliseconds when it is picked/clicked.
Action 2: Fades the same light back to white (Color3.White()) over 1000 milliseconds when it is picked/clicked again.

Scaling on Pick with Condition:
Action: Scales the this object (likely referring to a mesh in the scene) to double its size (Vector3(2, 2, 2)) over 1000 milliseconds when it is picked/clicked.
Condition: This action has a PredicateCondition. It will only execute if the light object's 'diffuse' color is currently black.

Wireframe Toggle on Intersection:
Action: Sets the 'wireframe' property of another mesh's material to 'true' when this.mesh intersects with a mesh identified as "sphere". The usePreciseIntersection: true parameter ensures accurate intersection detection.

### Keyboard Actions
Assuming we continue from the previous code
```
this.scene.actionManager.registerAction(
    new ExecuteCodeAction(
        {
            trigger: ActionManager.OnKeyUpTrigger,
            parameter: "r",
        },
        () => {
            this.scaling.setAll(1);
            this.mesh.material.wireframe = false;
            console.log("r was pressed: reset " + this.name);
        }
    )
);
```
Presumably, this code provides a reset mechanism. Pressing the "r" key likely triggers other actions that might scale or change the wireframe mode of a mesh. Releasing the "r" key executes this snippet to restore the mesh to its default state.

### Observables
```
const onIntersectObservable = new Observable<boolean>();
scene.registerBeforeRender(function () {
  const isIntersecting = sphere.intersectsMesh(helloSphere, true, true);
  onIntersectObservable.notifyObservers(isIntersecting);
});

helloSphere.onIntersectObservable = onIntersectObservable;

const redColor = Color3.Red();
const whiteColor = Color3.White();

helloSphere.onIntersectObservable.add((isIntersecting) => {
  const material = helloSphere.mesh.material as StandardMaterial;
  const isRed = material.diffuseColor === redColor;
  if (isIntersecting && !isRed) {
    material.diffuseColor = redColor;
  } else if (!isIntersecting && isRed) {
    material.diffuseColor = whiteColor;
  }
});
```
In the sphere code,
```
    scene : Scene;
    mesh : Mesh;
    label : TextPlane;
    onIntersectObservable : Observable<boolean>
}    

export class HelloSphere extends AbstractMesh implements HelloMesh {
    scene : Scene;
    mesh : Mesh;
    label : TextPlane;
 onIntersectObservable : Observable<boolean>

//code continues
```
Observable for Intersection:
onIntersectObservable: An Observable is created. Observables are used in Babylon.js to notify subscribers when specific events occur. In this case, this observable will be used to signal when intersections happen.

Intersection Check Loop (scene.registerBeforeRender):

scene.registerBeforeRender: Registers a function to be executed before each frame is rendered in the scene. This ensures the intersection check happens continuously.
sphere.intersectsMesh(helloSphere, true, true): This line checks if the sphere mesh intersects with the helloSphere mesh. The true parameters ensure precise intersection calculations.
onIntersectObservable.notifyObservers(isIntersecting): Notifies all subscribers of the onIntersectObservable whether an intersection is currently happening (isIntersecting will be either true or false).

Handling the Observable (helloSphere.onIntersectObservable.add):
helloSphere.onIntersectObservable: This references the onIntersectObservable created earlier and attaches a subscriber to it.
Subscriber Function: The provided function will be executed whenever the onIntersectObservable is notified.
It receives an isIntersecting boolean indicating the current intersection status.
It changes the diffuseColor property of the helloSphere's material:
To red (Color3.Red()) if the meshes are intersecting and the color isn't already red.
Back to white (Color3.White()) if they are not intersecting and the color is currently red.

```
// 2. create an observable for checking distance
const onDistanceChangeObservable = new Observable<number>();
let previousState: number = null;
scene.onBeforeRenderObservable.add(() => {
  const currentState = Vector3.Distance(
    sphere.position,
    helloSphere.position
  );
  if (currentState !== previousState) {
    console.log("distance updated!");
    previousState = currentState;
    onDistanceChangeObservable.notifyObservers(currentState);
  }
});

helloSphere.onDistanceChangeObservable = onDistanceChangeObservable;

const blueColor = Color3.Blue();
helloSphere.onDistanceChangeObservable.add((distance) => {
  const isCloseEnough = distance < 1.2;
  const material = helloSphere.mesh.material as StandardMaterial;
  const isBlue = material.diffuseColor === blueColor;
  const isRed = material.diffuseColor === redColor;
  if (isCloseEnough && !isBlue && !isRed) {
    material.diffuseColor = blueColor;
  } else if (!isCloseEnough && isBlue) {
    material.diffuseColor = whiteColor;
  }
});
```
1. Distance Observable:
onDistanceChangeObservable: An Observable is created to track changes in distance between the meshes.
previousState: A variable to store the previous distance value, used for comparison.

2. Distance Calculation Loop (scene.onBeforeRenderObservable.add):
scene.onBeforeRenderObservable.add: Registers a function to be executed before each frame renders.
Vector3.Distance(sphere.position, helloSphere.position): Calculates the distance between the centers of the sphere and helloSphere meshes.
Change Detection:
If the current distance is different from the previous distance:
Log a message indicating the distance has changed.
Update previousState with the current distance.
Notify observers of the onDistanceChangeObservable with the new distance value.

3. Handling Distance Changes (helloSphere.onDistanceChangeObservable.add):
helloSphere.onDistanceChangeObservable: Attaches an observer that will execute code whenever the distance observable is notified.
Subscriber Function:
Receives the updated distance between the meshes.
isCloseEnough: Calculates if the meshes are within a specified threshold (1.2 units in this case).
Updates the helloSphere's material diffuseColor based on these conditions:
Blue: If the meshes are close enough, and the material isn't already blue or red, set the color to blue.
White: If the meshes are not close enough and the color is currently blue, set the color back to white.

### Create Custom Observer
```
const observer = new Observer<number>((distance) => {
  helloSphere.label.textBlock.text = "d: " + distance.toFixed(2);
}, -1);
onDistanceChangeObservable.observers.push(observer);

```

### Coroutines
```
const addObserverCoroutine = function* () {
  console.log("frame " + scene.getFrameId() + ": do nothing");
  yield;
  console.log("frame " + scene.getFrameId() + ": add observer");
  onDistanceChangeObservable.observers.push(observer);
  yield;
  console.log("frame " + scene.getFrameId() + ": do nothing");
};
scene.onBeforeRenderObservable.runCoroutineAsync(addObserverCoroutine());
```


Purpose of the Function
The primary purpose of this function is to delay the addition of an observer to the onDistanceChangeObservable until a later frame. Here's how it works:

Coroutine Definition:
addObserverCoroutine: This function is defined as a generator function (notice the function* syntax). Generator functions are special in JavaScript, allowing them to pause and resume execution using the yield keyword.
Coroutines in Babylon.js are a way to execute code over multiple frames, often to introduce delays or create sequences of actions.

Steps:
Log a message: Logs the current frame with the message "frame [frame number] : do nothing".
yield: Pauses the execution of the coroutine and resumes it in the next frame.
Log a message: Logs the current frame with the message "frame [frame number] : add observer".
Add the observer: Pushes an observer (which is assumed to be defined elsewhere in your code) onto the list of observers for the onDistanceChangeObservable.
yield: Pauses the execution again.
Log a message: Logs the current frame with the message "frame [frame number] : do nothing".

Executing the Coroutine
scene.onBeforeRenderObservable.runCoroutineAsync(addObserverCoroutine()): This line starts the execution of the addObserverCoroutine.
runCoroutineAsync ensures that the code within the coroutine will be spread out over multiple frames (because of the yield statements).

Overall Effect
By using a coroutine, this code:
Delays Adding Observer: The observer won't be added to the onDistanceChangeObservable immediately. Instead, it will be added in the frame after the coroutine begins executing.
Spreads Execution over Frames: The logging statements combined with the yield help visualize how the coroutine will run its code split across multiple frames of rendering

```
const coroutine = function* () {
  (async function () {
    await Tools.DelayAsync(2000);
    console.log("frame " + scene.getFrameId() + ": fn 1");
  })();
  yield;
  (async function () {
    await Tools.DelayAsync(2000);
    console.log("frame " + scene.getFrameId() + ": fn 2");
  })();
  yield;
  (async function () {
    console.log("frame " + scene.getFrameId() + ": fn 3");
  })();
  yield Tools.DelayAsync(1000);
  (async function () {
    console.log("frame " + scene.getFrameId() + ": fn 4");
  })();
};
scene.onBeforeRenderObservable.runCoroutineAsync(coroutine());
```
This code performs the following actions:

Starts an anonymous async function that waits for 2000ms (2 seconds), then logs the current frame ID along with the string ": fn 1".
Yields control back to the scene rendering loop, effectively pausing the coroutine until the next frame.
Starts another anonymous async function that also waits for 2000ms, then logs the current frame ID along with the string ": fn 2".
Yields control back to the scene rendering loop again.
Starts yet another anonymous function immediately, without a delay, which logs the current frame ID along with the string ": fn 3".
Yields control, but this time waits for 1000ms (1 second) before the next function in the coroutine is eligible to run.
Starts the last anonymous async function that logs the current frame ID along with the string ": fn 4".
The last line scene.onBeforeRenderObservable.runCoroutineAsync(coroutine()); schedules the coroutine to run within the scene's onBeforeRenderObservable, which will execute its steps asynchronously according to the yields and delays, aligning with the scene's render frames.

### Locomotion
```
initLocomotion(
  movement: MovementMode,
  xr: WebXRDefaultExperience,
  featureManager: WebXRFeaturesManager,
  ground: Mesh
) {
  switch (movement) {
    case MovementMode.Teleportation:
      console.log("movement mode: teleportation");
      const teleportation = featureManager.enableFeature(
        WebXRFeatureName.TELEPORTATION,
        "stable",
        {
          xrInput: xr.input,
          floorMeshes: [ground],
          timeToTeleport: 2000,
          useMainComponentOnly: true,
          defaultTargetMeshOptions: {
            teleportationFillColor: "#55FF99",
            teleportationBorderColor: "blue",
            torusArrowMaterial: ground.material,
          },
        },
        true,
        true
      ) as WebXRMotionControllerTeleportation;
      teleportation.parabolicRayEnabled = true;
      teleportation.parabolicCheckRadius = 2;
      break;

    case MovementMode.Controller:
      console.log("movement mode: controller");
      featureManager.disableFeature(WebXRFeatureName.TELEPORTATION);
      featureManager.enableFeature(WebXRFeatureName.MOVEMENT, "latest", {
        xrInput: xr.input,
      });
      break;

    case MovementMode.Walk:
      console.log("movement mode: walk");
      featureManager.disableFeature(WebXRFeatureName.TELEPORTATION);
      const xrRoot = new TransformNode("xr root", scene);
      xr.baseExperience.camera.parent = xrRoot;
      featureManager.enableFeature(
        WebXRFeatureName.WALKING_LOCOMOTION,
        "stable",
        {
          locomotionTarget: xrRoot,
        }
      );
      break;
  }
}
```
This is how to activate
```
const xr = await scene.createDefaultXRExperienceAsync({
  uiOptions: {
    sessionMode: "immersive-vr",
    // sessionMode: 'immersive-ar'
  },
  optionalFeatures: true,
});
// only for debugging
(window as any).xr = xr;

const featureManager = xr.baseExperience.featuresManager;
console.log(WebXRFeaturesManager.GetAvailableFeatures());

// locomotion
const movement = MovementMode.Walk;
this.initLocomotion(movement, xr, featureManager, ground, scene);
```

### Hand Track
```
// hand tracking
try {
  featureManager.enableFeature(WebXRFeatureName.HAND_TRACKING, "latest", {
    xrInput: xr.input,
    jointMeshes: {
      disableDefaultHandMesh: false,
    },
  });
} catch (error) {
  console.log(error);
}

// enabled features
console.log(featureManager.getEnabledFeatures());
```

### Bimanual Interaction
```
// multiple pointer scale
const multiPointerScaleBehavior = new MultiPointerScaleBehavior();
helloSphere.addBehavior(multiPointerScaleBehavior);
```

### Gizmos
```
// more behaviors
// default gizmo
const gizmoManager = new GizmoManager(scene);
// gizmoManager.positionGizmoEnabled = true;
// gizmoManager.rotationGizmoEnabled = true;
// gizmoManager.scaleGizmoEnabled = true;
gizmoManager.boundingBoxGizmoEnabled = true;
```
### Natural Grabbing
```
// hand/controller drag
let mesh: AbstractMesh;
xr.input.onControllerAddedObservable.add((controller) => {
  controller.onMotionControllerInitObservable.add((motionController) => {
    // const ids = motionController.getComponentIds();
    // const trigger = motionController.getComponent(ids[0]);
    const trigger = motionController.getComponentOfType("trigger");
    trigger.onButtonStateChangedObservable.add(() => {
      if (trigger.changes.pressed) {
        if (trigger.pressed) {
          if (mesh == xr.pointerSelection.getMeshUnderPointer()) {
            controller.uniqueId
            console.log("mesh under controller pointer: " + mesh.name);
            if (mesh.name != "ground") {
              const distance = Vector3.Distance(
                motionController.rootMesh.getAbsolutePosition(),
                mesh.getAbsolutePosition()
              );
              console.log("distance: " + distance);
              if (distance < 1) {
                mesh.setParent(motionController.rootMesh);
                console.log("grab mesh: " + mesh.name);
              }
            } else {
              console.log("no mesh under pointer");
            }
          }
        } else {
          if (mesh && mesh.parent) {
            mesh.setParent(null);
            console.log("release mesh: " + mesh.name);
          }
        }
      }
    });
  });
});

```
