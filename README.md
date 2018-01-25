# Meme-tastic sound board

In this project we will create a sound board full of memes and then upload it to a real website. Try to follow the class and ask questions! There will be many explanations you will miss if you try to get ahead.

# Step 1

Create a folder in your machine, it can be in your desktop.

# Step 2

Download all the sound files in the following link into the folder you created:

http://titanhack.com/lighthouse/

# Step 3 

Browse to that folder, click on it, and then click on "Open with Code." This will open visual studio code.

# Step 4

Create a new file called index.html. You can create this file by hitting Ctrl+n and then ctrl+s, or by right-clicking on an empty area of the left-side panel.

# Step 5

Let's get coding your first website:

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Document</title>
</head>
<body>
  <h1> Hello, World! </h1>  
</body>
</html>
```

H1 is a "header" tag. Html files are just a bunch of tags like that one, nested one inside the other.

# Step 6

Browse to your index.html file using the windows explorer and open it. It should automatically open in your web browser.

# Step 7

Problems? Ask questions!

# Step 8

Now let's add one of the sound files to the page. Include the following code after the closing h1 tag:

```
<audio src="airhorn.mp3" controls id="airhorn" />
```

# Step 9

Now let's write our first bit of real code! Insert the following code right before the ending body tag:

```
<script>
  document.onkeypress = function(e) {
    alert("You pressed a key!!");
  }
</script>
```

# Step 10

You just built and bound your first event listener! Now, if you replace the contents of the event handler function, you can make a key stroke do whatever you want! For instance, when they press the number 1, you can make it play the airhorn sound. In order to do this, modify the content of the event handler function as follows:

```
if (e.key == 1) {
  document.getElementById("airhorn").currentTime = 0;
  document.getElementById("airhorn").play();
} 
```

# Step 11

Test! Ask questions! Make sure it works.

# Step 12

Now remove the ```controls``` attribute from the ```<audio>``` tag so it's invisible. Also, add instructions to your web page, like for instance:

```
<p>1 = airhorn</p>
```

# Step 13

Repeat the process for all the other files. Now you have a soundboard!

