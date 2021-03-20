[Home](./index.md)

# HTML

Plain HTML, CSS, and JavaScript can be used anywhere, since markdown gets converted to HTML anyway. `.html` files can be used instead of `.md` if desired, but there is no real benefit to doing this. You may also have separate style sheets and script files just as you would with a regular website, but for these examples everything will be inline. 

## Colored Text

<p style="color:green;">This text is green.</p>

<p>Only <span style="color:purple;">some</span> of this text is <span style="color:purple;">purple.</span>

<p style="background:green;">This text's background is green.</p>

<p style="background:black;color:white;">This text's background is black and it's text color is white.</p>

## Specify Font

<p style="font-family:times new roman;">This text is using Times New Roman font.</p>

<p style="font-family:serif;color:red">This text is using Serif font and is colored red.</p>

## Specify Font Size

<p style="font-size:80px;">Hello!</p>

## Image Size

Octocat image `octocat.png` located in the `assets/images` folder.
The first image is at 20% its original size.
The second is at 50% its original size.
The third is explicitly set to be 80 pixels wide.
The fourth is explicitly set to be 80 pixels wide and 40 pixels tall.

<img src="./assets/images/octocat.png" alt="Octocat" width="20%">

<img src="./assets/images/octocat.png" alt="Octocat" width="50%">

<img src="./assets/images/octocat.png" alt="Octocat" width="80px">

<img src="./assets/images/octocat.png" alt="Octocat" width="80px" height="40px">

<br>

An image's width and height will automatically scale together unless both are set.

## Button

<button>I'm a button</button>

<button style="color:pink;background:purple" >I'm a pink button</button>

<input type="button" onclick="location.href='https://google.com';" value="Go to Google" />

## Styled Links

<a href="./index.md" style="color:brown;">Click here to go to the index page</a>

## Programming Logic

This is where JavaScript comes in!

<p id="increasing-number">0</p>
<button onclick="increaseByOne" style="color:white;background:black">Increase number by 1</button>

<script>
function increaseByOne() {
    const increasingNumberTag = document.getElementById("increasing-number");
    const number = parseInt(increasingNumberTag.innerHTML, 10);
    number.innerHTML = number++;
}
</script>