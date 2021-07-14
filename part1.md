# Introduction to Semantic UI (less-based framework) in preparation for Junior Phase Final Project && -> https://semantic-ui.com/
## We are going to include the CDN, and create a 'cheat sheet' first. Then we will npm install for more customizability  (utilizing gulp as well).
> A CDN allows for the quick transfer of assets needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos.
<hr />

## Basic CDN Setup
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Semantic Sandbox</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/semantic-ui/2.4.1/semantic.min.css" integrity="sha512-8bHTC73gkZ7rZ7vpqUQThUDhqcNFyYi2xgDgPDHc+GXVGHXq+xPjynxIopALmOPqzo9JZj0k6OqqewdGO3EsrQ==" crossorigin="anonymous" referrerpolicy="no-referrer" />
</head>
<body>
    <h1>Hello</h1>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/semantic-ui/2.4.1/semantic.min.css"></script>
</body>
</html>
```
# Element: **Container**
## The container picks a width and wraps other UI elements so that they are contained in the container's max width and are responsive.
> Def: A container is an element designed to contain page elements to a reasonable maximum width based on the size of a user's screen.
```
<div class="ui container">
    Hello
</div>
```
## We can override styles with semantic ui. Notice how the headers are given classes that manipulate their normal size
```
<div class="ui container">
    <!-- HEADER -->
    <h1 class="ui small header">Heading 1</h1>
    <h2 class="ui tiny header">Heading 2</h2>
    <h3 class="ui medium header">Heading 3</h3>
    <h4 class="ui large header">Heading 4</h4>
    <h5 class="ui huge header">Heading 5</h5>
    <h6 class="ui small header">Heading 6</h6>
</div>
```
# Element: **Button**
## One thing to note about Semantic UI is that..well.. it's more semantic. Btn is button. More descriptive.
## Like bootstrap though, we do have context classes. Primary, secondary, positive, negative..
> Def: A standard button.
> fluid: will span the entire width of its container.
```
    <!-- BUTTONS -->
    <button class="ui button">Read More</button>
    <button class="ui primary button">Read More</button>
    <button class="ui secondary button">Read More</button>
    <button class="ui positive button">Read More</button>
    <button class="ui negative button">Read More</button>
    <br><br>
    <button class="ui red button">Read More</button>
    <button class="ui blue button">Read More</button>
    <button class="ui green button">Read More</button>
    <button class="ui purple button">Read More</button>
    <button class="ui yellow button">Read More</button>
    <button class="ui brown button">Read More</button>
    <button class="ui orange button">Read More</button>
    <button class="ui olive button">Read More</button>
    <button class="ui teal button">Read More</button>
    <button class="ui violet button">Read More</button>
    <button class="ui grey button">Read More</button>
    <br><br>
    <button class="ui disabled red button">Read More</button>
    <button class="ui loading blue button">Read More</button>
    <button class="ui massive button">Read More</button>
    <button class="ui big button">Read More</button>
    <button class="ui large button">Read More</button>
    <button class="ui medium button">Read More</button>
    <button class="ui small button">Read More</button>
    <button class="ui tiny button">Read More</button>
    <button class="ui mini button">Read More</button>
    <br><br>
    <button class="ui basic button">Read More</button>
    <button class="ui basic red button">Read More</button>
    <button class="ui basic green button">Read More</button>
    <button class="ui basic blue button">Read More</button>
    <button class="ui basic teal button">Read More</button>
    <button class="ui basic fluid button">Read More</button>
```
## We can use more advance ui classes to accomplish animations and other fancy things. (tabindex 0 allows this button to be reached by tab)
```
    <div class="ui animated fade button" tabindex="0">
        <div class="visible content">Visible</div>
        <div class="hidden content">Hidden</div>
    </div>
```

# Element: **Icon**
> An icon is a glyph used to represent something else.
```
    <button class="ui icon button">
        <i class="cloud icon"></i>
    </button>
    <i class="bell icon"></i>
    <i class="bell outline icon"></i>
    <i class="bell slash icon"></i>
    <i class="bell slash outline icon"></i>
    <i class="calendar icon"></i>
    <i class="calendar outline icon"></i>
    <i class="calendar alternate icon"></i>
    <i class="calendar alternate outline icon"></i>
    <i class="calendar check icon"></i>
    <i class="calendar check outline icon"></i>
    <i class="calendar minus icon"></i>
    <i class="calendar minus outline icon"></i>
    <i class="calendar plus icon"></i>
    <i class="calendar plus outline icon"></i>
    <i class="calendar times icon"></i>
    <i class="calendar times outline icon"></i>
    <i class="clock icon"></i>
    <i class="clock outline icon"></i>
    <i class="hourglass icon"></i>
    <i class="hourglass outline icon"></i>
    <i class="hourglass end icon"></i>
    <i class="hourglass half icon"></i>
    <i class="hourglass start icon"></i>
    <i class="stopwatch icon"></i>
```
# Element: **Label**
> A label displays content classification.
```
    <!-- LABELS -->
    <div class="ui label">
        <i class="mail icon"></i>23
    </div>

    <div class="inline field">
        <input type="text" name="" value="" />
        <div class="ui left pointing label">
            That username is taken
        </div>
    </div>
```

# Collection: **Breadcrump**
> A breadcrumb is used to show hierarchy between content .
```
    <div class="ui breadcrumb">
        <a class="section">Home</a>
        <div class="divider"> / </div>
        <a class="section">Store</a>
        <div class="divider"> / </div>
        <div class="active section">T-Shirt</div>
    </div>
```