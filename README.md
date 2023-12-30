# Image Placement in HTML and CSS

This project demonstrates how to position an image at all four corners and the center of a div block using HTML and CSS. The div block is styled with a border, and the images are strategically placed for a visually appealing layout.

## Project Structure

- **index.html:** The main HTML file that defines the structure of the webpage.
- **style.css:** The stylesheet containing the CSS code for styling and positioning the image.

## Usage

1. Clone the repository to your local machine:

    ```bash
    git clone https://github.com/your-username/image-placement.git
    ```

2. Open the project in your preferred code editor.

3. Customize the image source in the `index.html` file by replacing "Image.jpeg" with your desired image filename.

4. Experiment with the CSS styles in the `style.css` file to further customize the appearance and positioning of the image.

5. Open the `index.html` file in a web browser to view the results.

## HTML Structure

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image Placement</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <div id="wrapper">

        <img src="Image.jpeg" alt="Corner 1" class="corner-image" id="top-left-image">
        <img src="Image.jpeg" alt="Corner 2" class="corner-image" id="top-right-image">
        <img src="Image.jpeg" alt="Corner 3" class="corner-image" id="bottom-left-image">
        <img src="Image.jpeg" alt="Corner 4" class="corner-image" id="bottom-right-image">
        <img src="Image.jpeg" alt="Center" id="centre-image">

    </div>

</body>
</html>
```

## CSS Styles

```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    background-color: black;
}

#wrapper {
    border: 5px solid white;
    width: 100vw;
    height: 100vh;
    position: relative;
}

img {
    border: 5px solid red;
    position: absolute;
    height: 20vh;
    width: 20vw;
}

.corner-image {
    position: absolute;
}

#top-left-image {
    top: 5px;
    left: 5px;
}

#top-right-image {
    top: 5px;
    right: 5px;
}

#bottom-left-image {
    bottom: 5px;
    left: 5px;
}

#bottom-right-image {
    bottom: 5px;
    right: 5px;
}

#centre-image {
    left: 40vw;
    top: 38vh;
}
