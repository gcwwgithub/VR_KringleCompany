# VR_KringleCompany
Great Asset, Great Great Asset

## Possible Choices for why you choose a paraticular framework
1. Documentation
2. Code Management / Collab
3. Asset creation
4. Dev Tools

### Unity

### Unreal
Chosen For intensive and high quality graphics

### AFrame
According to Chatgpt
A-Frame is an open-source web framework for building virtual reality (VR) experiences. It is primarily used for creating VR scenes, applications, and experiences that run in a web browser. A-Frame is built on top of HTML, making it accessible to web developers who are already familiar with HTML, CSS, and JavaScript. With A-Frame, developers can create 3D, VR-enabled content using a simple HTML-like syntax, making it easier to design, iterate, and deploy VR applications without the need for complex WebGL APIs directly. It is created by Morzilla

A-Frame is based on the Entity-Component-System (ECS) architecture, which is a common pattern in game development. In **A-Frame, everything in the scene is an entity represented by HTML elements, and functionality is added to these entities through components that can modify their appearance, behavior, and functionality. This approach allows for high modularity, reusability, and simplicity in developing VR scenes.**

Developers can extend A-Frame's core functionality by creating custom components using JavaScript, enabling the integration of external libraries and APIs for more complex interactions, animations, and data visualization in 3D and VR. A-Frame supports WebVR and WebXR APIs, allowing it to work across various devices such as VR headsets (e.g., Oculus Rift, HTC Vive), mobile devices with cardboard viewers, and desktop/laptop browsers, providing a wide platform reach.

A-Frame is designed to be accessible for beginners while also powerful enough for advanced developers to build sophisticated VR experiences. It has fostered a growing community that contributes to its development, shares components, and provides resources, making it a popular choice for web-based VR projects.

According to Chek
Pros: designed to be a highly accessible tool for new VR developers with some programming Foundations at the same time it is highly extensible to allow experienced devs to create highly complex VR experiences. Note that applications developed by A-frame can only exist on the web which has the usual obvious pros and cons
1. Extremely Accessible
2. Conducive for learnimg
3. Conducive for Reseasrch
4. Well designed architecture and usable API

Cons: 
the biggest con is perhaps the level of immersion from A System's point of view that is limited by what web Technologies can provide and in many ways limited by the browser developers as well however that is slowly improving as we move from webgl to web GPU which without delving into the rapid hole of advanced rendering topics simply means that we get more and more direct access to Hardware right from your browser relatedly the number of differences between each of the popular browsers is. WebXR resolves that somewhat

Benefits of Web Based Tools
1. Accessible to users and developers

### Babylon JS
From chatgpt
Babylon.js is a powerful, open-source 3D engine that enables developers to create and render 3D graphics within web browsers. It leverages WebGL, WebXR, and other web standards to facilitate the development of interactive 3D applications, games, and immersive experiences directly on the web, without the need for plugins or additional software installations.

The core strengths of Babylon.js include its comprehensive feature set, ease of use, and strong performance. It is designed to be accessible to beginners, with a straightforward API and extensive documentation, while also offering the depth and flexibility required for complex projects by advanced users.

Key features of Babylon.js include:

Rich 3D Graphics Rendering: Supports advanced graphics features like shadows, lighting, textures, particle systems, and more, enabling the creation of realistic and visually appealing scenes.
Physics Engine Integration: Integrates with popular physics engines, allowing for realistic simulations of physical interactions within the 3D world.
Support for WebXR: Enables the creation of virtual reality (VR) and augmented reality (AR) experiences that are compatible with a wide range of devices, from smartphones to dedicated VR headsets.
Animation System: Comes with a sophisticated animation system that supports complex animations, blending, and transitions for 3D objects.
GUI Support: Provides a library for creating interactive 2D user interfaces within 3D scenes, facilitating the development of comprehensive user experiences.
Extensibility: Developers can extend Babylon.js with custom shaders, materials, and more, thanks to its modular architecture.
Community and Ecosystem: Benefits from a vibrant community and ecosystem, offering numerous examples, extensions, and plugins to help accelerate development.
Babylon.js is widely used for a variety of web-based 3D projects, including games, interactive visualizations, training simulations, and architectural walkthroughs. Its commitment to being cross-platform ensures that Babylon.js applications can run on any device with a web browser, making it a versatile choice for developers looking to leverage 3D graphics on the web.

From Chek
1. Scaled down Unity interfacd
2. Rendering and physics using state of the art techniques and "target performance"
3. Large and active community

### WebXR
From ChatGPT
WebXR, or Web Extended Reality, is a set of standards and technologies that enables immersive experiences, including virtual reality (VR) and augmented reality (AR), to be delivered through web browsers. It allows developers to create VR and AR applications that can be accessed and experienced directly through web browsers, without the need for users to install additional software or applications.

WebXR builds upon the capabilities of WebVR and WebAR, extending them to support a wider range of devices and experiences. It provides APIs (Application Programming Interfaces) that developers can use to access the features of VR and AR devices, such as headsets, controllers, and sensors, allowing them to create interactive and immersive content for the web.

One of the key advantages of WebXR is its accessibility. Users can access WebXR experiences across a variety of devices, including desktop computers, smartphones, and standalone VR headsets, simply by visiting a website. This democratizes access to VR and AR content, making it easier for developers to reach a broader audience without the need for specialized hardware or software.

Overall, WebXR represents a significant step forward in making immersive experiences more widely available and accessible on the web, opening up new possibilities for entertainment, education, training, and other applications.

From Chek
in general webxr refers to a set of open apis that aim to standardize the way XR apps are created on the web it originally started with the web XR device API but has since worked on a number of other open apis including the web XR Gamepad API and the WebEx are AR API a greater adoption of common standards will go a long way in moving the industry forward

### JavaScript vs TypeScript 
JavaScript and TypeScript are both programming languages used for web development, but they have some key differences. JavaScript is a dynamically typed language, while TypeScript is a statically typed superset of JavaScript that adds optional static typing and other features. Here's a code example to illustrate some of the differences:

```
// JavaScript code
function greet(name) {
    return "Hello, " + name + "!";
}

console.log(greet("John")); // Output: Hello, John!
console.log(greet(123));     // Output: Hello, 123!

// TypeScript code
function greet(name: string): string {
    return "Hello, " + name + "!";
}

console.log(greet("John")); // Output: Hello, John!
console.log(greet(123));     // Error: Argument of type 'number' is not assignable to parameter of type 'string'.
```

### Order? I dont know if its correct, its in the video
Open XR


Bablyon JS
A-Frame
Unity
Unreal



Cospaces

### OpenXR C++ SDK
From ChatGPT
OpenXR is an open, royalty-free standard for virtual reality (VR) and augmented reality (AR) applications and devices. It was developed by the Khronos Group, a consortium of companies working on creating open standards for multimedia and parallel computing. OpenXR aims to address the fragmentation and compatibility issues that arise in the VR and AR ecosystem by providing a common API (Application Programming Interface) for developers to target multiple VR and AR platforms.

OpenXR is an open, royalty-free standard for virtual reality (VR) and augmented reality (AR) applications and devices. It was developed by the Khronos Group, a consortium of companies working on creating open standards for multimedia and parallel computing. OpenXR aims to address the fragmentation and compatibility issues that arise in the VR and AR ecosystem by providing a common API (Application Programming Interface) for developers to target multiple VR and AR platforms.

Key features and goals of OpenXR include:

Cross-Platform Compatibility: OpenXR is designed to work across various VR and AR platforms, including different hardware devices and software ecosystems. This allows developers to write applications once and deploy them across multiple platforms without significant modifications.

Hardware Abstraction: OpenXR abstracts the differences between VR and AR hardware devices, such as headsets, controllers, and sensors, allowing developers to write code that interacts with these devices in a unified manner.

Optimization and Performance: OpenXR provides mechanisms for optimizing performance and reducing latency in VR and AR applications, ensuring a smoother and more immersive user experience.

Vendor Neutrality: OpenXR is an open standard that is not tied to any specific hardware manufacturer or software platform, promoting vendor neutrality and fostering innovation within the VR and AR industry.

Community Collaboration: OpenXR is developed collaboratively by industry stakeholders through the Khronos Group, allowing for input and contributions from a wide range of companies and developers.

Overall, OpenXR aims to simplify the development process for VR and AR applications, improve interoperability between different hardware and software platforms, and accelerate the growth of the VR and AR ecosystem by providing a common foundation for developers to build upon.

From Chek
Only go this route if you need  to implement some unique novel features that require Ultra custom code close to the metal on the targeted platform

### Cospaces
CoSpaces is a platform that allows users to create, share, and explore virtual reality (VR) and augmented reality (AR) experiences without the need for coding skills. It provides an intuitive and user-friendly interface for building immersive 3D environments, interactive scenes, and games.

Key features of CoSpaces include:

Visual Programming: CoSpaces offers a drag-and-drop interface for creating interactive elements and programming behaviors without writing code. Users can easily add and manipulate objects, characters, animations, and logic to design their VR and AR experiences.

Asset Library: CoSpaces provides a library of pre-made 3D models, textures, sounds, and animations that users can use to quickly populate their scenes and enhance their creations.

Collaboration: CoSpaces supports collaborative editing, allowing multiple users to work on the same project simultaneously. This feature is particularly useful for classrooms, workshops, and team projects where collaboration is essential.

Cross-Platform Compatibility: CoSpaces experiences can be viewed and interacted with on various devices, including desktop computers, smartphones, tablets, and VR headsets. This enables users to access and share their creations across different platforms and devices.

Educational Use: CoSpaces is widely used in educational settings to create immersive learning experiences, virtual field trips, simulations, and presentations. It provides educators with a powerful tool for engaging students and enhancing learning outcomes through experiential and interactive content.

Overall, CoSpaces empowers users to unleash their creativity and imagination to build immersive VR and AR experiences without the need for advanced technical skills, making it accessible to a wide range of users, including educators, students, hobbyists, and professionals.

### Key Considerations
1. Requirements of specific project - this will forgo the personal inclinations (like if you like Unity but need to use BabylonJS)
2. Cost
3. Stability (like does the API got bugs)
4. Customisability
5. Community + Support
6. Learning Opportunites

### Why our course use BablyonJS
1. Facilitate Learning in the best way possible
2. Accessbility for users
3. Large Dev Community Support
4. Supports the latest web GPU API
5. Provides Longevity to the prototypes built - could allow you to transfer knowledge to other webxr applications
6. Appreciate the nuanced technicalities - you will need to consider the technical details and knowledge when making the apps
7. Contribute to XRAuthor which is a research project - yes the school is trying to slave us.



## Mentimeter Questions
![Image Description](Pictures/Week4_Slide1.JPG)
![Image Description](Pictures/Week4_Slide2.JPG)
![Image Description](Pictures/Week4_Slide3.JPG)
![Image Description](Pictures/Week4_Slide4.JPG)
The answer is package.json
package.json is a file used in Node.js projects to manage project dependencies, scripts, metadata, and other configuration settings. It is a standard file in Node.js projects and is typically located in the root directory of the project. Here's what you'll commonly find in a package.json file:

Project Metadata: Information about the project such as its name, version, description, author, license, etc. This metadata helps other developers understand the purpose and characteristics of the project.

Dependencies: Lists of packages or modules that the project depends on for its functionality. Dependencies can be categorized into two types: dependencies and devDependencies. Dependencies listed under dependencies are required for the application to run, while those under devDependencies are only needed for development purposes.

Scripts: Custom scripts that can be executed using the npm or yarn command line interface. These scripts can perform various tasks such as running tests, building the project, starting the development server, etc. Common script names include start, test, build, dev, etc.

Version Control: Information related to version control systems such as Git repositories, including URLs for remote repositories, branch information, etc.

Configuration Settings: Additional configuration settings specific to the project or its dependencies. These settings can include options for compilers, linters, bundlers, test frameworks, etc.

Here's an example of a simple package.json file:
```
{
  "name": "my-project",
  "version": "1.0.0",
  "description": "A sample Node.js project",
  "main": "index.js",
  "scripts": {
    "start": "node index.js", // Script to start the application
    "test": "jest",           // Script to run tests using Jest
    "build": "webpack --mode production", // Script to build the project for production
    "lint": "eslint ."       // Script to run ESLint for code linting
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

![Image Description](Pictures/Week4_Slide5.JPG)
The answer is packagelock.json

package-lock.json is a file generated by npm (Node Package Manager) when you run npm install to install dependencies for a Node.js project. It serves as a lockfile that records the exact versions of all packages and their dependencies that were installed. This ensures that subsequent installs of the project, whether by the same developer or by others, will use the exact same versions of dependencies, thus guaranteeing reproducibility and consistency across different environments.

Here's what package-lock.json typically contains:

Dependency Tree: The file contains a detailed dependency tree, listing all the packages that were installed, along with their versions. It records both direct dependencies (those listed in your package.json) and their transitive dependencies.

Exact Versions: For each package, package-lock.json specifies the exact version that was installed, including any sub-dependencies. This prevents npm from installing different versions of the same package in different environments, which could lead to compatibility issues.

Integrity Hashes: package-lock.json includes integrity hashes for each package, which are cryptographic hashes computed from the package's contents. These hashes ensure that the installed packages have not been tampered with or corrupted.

Metadata: Additional metadata such as URLs for package tarballs, version ranges, and other information necessary for installing and resolving dependencies.

The presence of package-lock.json is particularly important in collaborative projects or when deploying applications to production environments. It helps ensure that all developers working on the project are using the same versions of dependencies and reduces the likelihood of unexpected behavior due to version mismatches.

It's worth noting that package-lock.json should be committed to version control along with your other project files (package.json, source code, etc.) to ensure that everyone working on the project has access to the same dependency versions. However, it's generally recommended to exclude the node_modules directory from version control, as the dependencies themselves can be quite large and are better managed through npm or yarn.

So in particular
package-lock.json: This file is automatically generated by npm when dependencies are installed and contains detailed information about the exact versions of dependencies (including sub-dependencies) that were installed. By committing package-lock.json, you ensure that all team members install the exact same versions of dependencies, preventing version mismatches and ensuring consistency across different environments.

The code for the next line is this
```
const xr = await scene.createDefaultXRExperienceAsync({
            uiOptions: {
                    sessionMode: "immersive-vr",
                    },
});
```
![Image Description](Pictures/Week4_Slide6.JPG)
The createDefaultXRExperienceAsync method is an asynchronous function provided by Babylon.js to create a default XR experience in the scene.
The await keyword is used before calling createDefaultXRExperienceAsync, indicating that the execution of the code will pause and wait for the asynchronous operation (initialization of the XR experience) to complete before proceeding.
The 4th option is not correct cause that is a blocking call. The await is async so it is not waiting for everything 



![Image Description](Pictures/Week4_Slide7.JPG)

The question is 
You are engaged by a mining company to build a VR system for training their own miners to operate in a coal mine. They have funds to purchase any necessary hardware you propose that is suitable and within budget and they want the working system delivered in 8 months time.
![Image Description](Pictures/Week4_Slide8.JPG)
Chek logic is because its supposed to be realistic and you have decently long time. So something with good support and realism is Unity. If Unreal was here, it will be hard to choose


The question is 
You are building your own metaverse application, an immersive social network that aims to allow as many users as possbile to particupate in, using different platform and devices. You have limited funds as an individual of course and aim to spend as little as possible on development
![Image Description](Pictures/Week4_Slide9.JPG)
Chek logic is Unity web support not good so choose the one gives better web support and that is Babylon JS. Sure whatever fuck u.

I cant read the bloody question for the next one but its something like that
The question sis something like You need to implement a cross platform native (i cant tell is it XR or VR) experience using a novel hand tracking application and you want to focus on implementing VR components with the same undelying code base access. Metas something HMDS, HTC Vive HMDs. Google Cardboard, something image is align it is an open standard so that here is a something developer ecosystem and that the underlyinh something will be constanttly improved

My guess is that standards are generally OpenXR 
![Image Description](Pictures/Week4_Slide10.JPG)
