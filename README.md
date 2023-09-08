# Svelte_project
Here you will find a simple application made using Svelte that has an interactive rectangular box that can be dragged across the window.
The coordinates of the box are also displayed at the top.

You will find two parts of the code in the source code.
<!-- Ordered List -->
1. JavaScript
   
This part has all the variable declarations and the event handlers.
The event handlers will detect a mouse click and the motion of the mouse. As the handlers are a child of the box class, they will only be called if a mouse button press is detected inside the box. The mouse movement handler will also assign the position of the cursor to the rectangular box's location.

2. HTML

This part has two objectives, one is to define the box class and its attributes and to display the coordinates. We also assign the mouse events to their respective handler here. 

## How to Run the Application on a Web Browser:

*Note: You will need to have [Node.js](https://nodejs.org) installed.*
<!-- Ordered List -->
1. Clone the repository and navigate to the folder 'Svelte_project'
2. On Windows: Press and hold Shift key and right-click inside the folder
3. Click on 'Open PowerShell window here'
4. Install the dependencies...

```bash
npm install
```
5. Then start [Rollup](https://rollupjs.org):

```bash
npm run dev
```
6. Navigate to [localhost:8080](http://localhost:8080). You should see the app running.
7. To create an optimized version of the app:

```bash
npm run build
```

