# ![Traffic Light Lab - Setup](./assets/hero.png)

## Setup

Open your Terminal application and navigate to your `~/code/ga/labs` directory:

```bash
cd ~/code/ga/labs
```

Make a new repository on [GitHub](https://github.com/) named traffic-light-lab.

Clone a copy of your remote repo locally by using the `git clone` command:

```bash
git clone https://github.com/<your-username>/traffic-light-lab.git
```

> 📚 Note: In the link above, where it says `<your-username>`, you should see the username from your GitHub account.

Next, `cd` into your new cloned directory, `traffic-light-lab`:

```bash
cd traffic-light-lab
```

Open the project's folder in your code editor:

```bash
code .
```

Next, create directories for your CSS and JS files: 

```bash
mkdir css js
```

Create your HTML, CSS, and JS files: 

```bash
touch css/style.css js/app.js index.html
```

Next, copy the following into your newly created `index.html` file: 

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" type="text/css" href="./css/style.css">
  <script defer src="./js/app.js"></script>
  <title>Traffic Light</title>
</head>
<body>
  <div id="controlPanel">
    <h1 id="stopButton" class="button">Stop</h1>
    <h1 id="slowButton" class="button">Slow</h1>
    <h1 id="goButton" class="button">Go</h1>
  </div>
  <div id="traffic-light">
    <div id="stopLight" class="bulb"></div>
    <div id="slowLight" class="bulb"></div>
    <div id="goLight" class="bulb"></div>
  </div>
</body>
</html>
```

Copy the following into `css/style.css`:

```css
body {
  font-family: sans-serif;
}

#controlPanel {
  float: left;
  padding-top: 30px;
}

.button {
  background-color: gray;
  color: white;
  border-radius: 10px;
  padding: 20px;
  text-align: center;
  margin: 90px 40px;
  cursor: pointer;
}

#traffic-light {
  height: 550px;
  width: 200px;
  float: left;
  background-color: #333;
  border-radius: 40px;
  margin: 30px 0;
  padding: 20px;
}

.bulb {
  height: 150px;
  width: 150px;
  background-color: #111;
  border-radius: 50%;
  margin: 25px auto;
  transition: background 500ms;
}
```

Finally, in `js/app.js`, enter the following: 

```js
console.log('hello world!');
```

Open `index.html` in the browser. You should see the following traffic light. If you open your browser console, you should see 'hello world!'

<img src="./assets/hello-world.png" alt="traffic light lab starting point">

The traffic light won't do anything yet when you click the buttons - that's where you come in! 

If either are not showing up correctly, go back and make sure your directory structure is correct, and that everything was copied over from the above codeblocks. 