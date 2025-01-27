# Appendix: Complete code for all projects

## Project 1. Does the photo contain a certain object? {#section_yj4_rny_tkb}

**Specifications:**

#|
||**Input:**|**Output:**||
||
```json
{
  "image": {
    "type": "url",
    "hidden": false,
    "required": true
  }
}
```
|
```json
{
  "result": {
    "type": "string",
    "hidden": false,
    "required": true
  }
}
```
||
|#

**HTML:**

{% if locale == "en-com" %}

```html
{{img src=image width="100%" height="400px"}} <div>Are there <b>shoes</b> in the picture?<div>
<div> {{field type="radio" name="result" value="OK" label="Yes" hotkey="1"}}
{{field type="radio" name="result" value="BAD" label="No" hotkey="2"}}
{{field type="radio" name="result" value="404" label="Loading error" hotkey="3"}}</div>
```

{% endif %}

**JavaScript:**

```javascript
exports.Task = extend(TolokaHandlebarsTask, function(options) {
    TolokaHandlebarsTask.call(this, options);
}, {
    onRender: function() {
        // DOM element for task is formed (available via #getDOMElement())
    },
    onDestroy: function() {
        // Task is completed. Global resources can be released (if used)
    }
});

function extend(ParentClass, constructorFunction, prototypeHash) {
    constructorFunction = constructorFunction || function() {};
    prototypeHash = prototypeHash || {};
    if (ParentClass) {
        constructorFunction.prototype = Object.create(ParentClass.prototype);
    }
    for (var i in prototypeHash) {
        constructorFunction.prototype[i] = prototypeHash[i];
    }
    return constructorFunction;
}
```

## Project 2. Find a similar item in an online store {#section_xnw_b4y_tkb}

**Specifications:**

#|
||**Input:**|**Output:**||
||
```json
{
  "image": {
    "type": "url",
    "hidden": false,
    "required": true
  }
}
```
|
```json
{
  "button": {
    "type": "boolean",
    "hidden": false,
    "required": true,
    "allowed_values": [
      true
    ]
  },
  "found_link": {
    "type": "string",
    "hidden": false,
    "pattern": "https://www.asos.com/.*",
    "required": true
  },
  "found_image": {
    "type": "file",
    "hidden": false,
    "required": true
  }
}
```
||
|#

**HTML:**

{% if locale == "en-com" %}

```html
{{img src=image width="50%" height="400px"}}
<div class='answers'>
 <p>Find similar <b>shoes</b> in the ASOS online store</p>
 {{field type="button-clicked" name="button" label="ASOS" href="https://www.asos.com" action=true}}
 <p>Shoes must be the same color, fabric, length, and style</p>
 <p>Paste the link here</p>
 {{field width="100%" type="input" name="found_link"}}
 <p>Upload the image here</p>
 <div>
 {{field width="100%" type="file-img" name="found_image" preview=true}}
 </div>
</div>
```

{% endif %}

**JavaScript:**

```javascript
exports.Task = extend(TolokaHandlebarsTask, function(options) {
    TolokaHandlebarsTask.call(this, options);
}, {
    validate: function(solution) {

        if (!solution.output_values.found_image) {

            return {
                task_id: this.getTask().id,
                errors: {
                    '__TASK__': {
                        message: 'Upload photo or mark that there is no photo'
                    }
                }
            };
        } else {
            return TolokaHandlebarsTask.prototype.validate.apply(this, arguments);
        }
    },
    onRender: function() {
        // DOM element for task is formed (available via #getDOMElement())
    },
    onDestroy: function() {
        // Task is completed. Global resources can be released (if used)
    }
});

function extend(ParentClass, constructorFunction, prototypeHash) {
    constructorFunction = constructorFunction || function() {};
    prototypeHash = prototypeHash || {};
    if (ParentClass) {
        constructorFunction.prototype = Object.create(ParentClass.prototype);
    }
    for (var i in prototypeHash) {
        constructorFunction.prototype[i] = prototypeHash[i];
    }
    return constructorFunction;
}
```

**CSS:**

```css
.task {
    display: block;
    height: 500px;
    width: 800px;
}

.img {
    float: left;
    width: 50%;
}

.answers {
    float: left;
    width: 40%;
    margin: 5%;
}
```

## Project 3. Does the item found look similar to the original? {#section_jyg_n4y_tkb}

**Specifications:**

#|
||**Input:**|**Output:**||
||
```json
{
  "image": {
    "type": "url",
    "hidden": false,
    "required": true
  },
  "found_link": {
    "type": "url",
    "hidden": false,
    "required": true
  },
  "assignment_id": {
    "type": "string",
    "hidden": true,
    "required": true
  }
}
```
|
```json
{
  "result": {
    "type": "string",
    "hidden": false,
    "required": true
  }
}
```
||
|#

**HTML:**

{% if locale == "en-com" %}

```html
{{img src=image height="400px"}} {{iframe src= found_link height="600px"}}
<p>Check that the uploaded image matches the product in the store.</p>
{{button label="Check the product" href=found_link action=true}}
<p>Are <b>these shoes</b> similar to each other?</p>
<p>Shoes must be the same color, fabric, length, and style.</p>
{{field type="radio" name="result" value="Yes" label="Yes"}}
{{field type="radio" name="result" value="No" label="No"}}
```

{% endif %}

**JavaScript:**

```javascript
exports.Task = extend(TolokaHandlebarsTask, function(options) {
    TolokaHandlebarsTask.call(this, options);
}, {
    onRender: function() {
        // DOM element for task is formed (available via #getDOMElement())
    },
    onDestroy: function() {
        // Task is completed. Global resources can be released (if used)
    }
});

function extend(ParentClass, constructorFunction, prototypeHash) {
    constructorFunction = constructorFunction || function() {};
    prototypeHash = prototypeHash || {};
    if (ParentClass) {
        constructorFunction.prototype = Object.create(ParentClass.prototype);
    }
    for (var i in prototypeHash) {
        constructorFunction.prototype[i] = prototypeHash[i];
    }
    return constructorFunction;
}
```

**CSS:**

```css
.task {
    display: block;
}

.img {
    float: left;
    width: 50%;
}

.iframe {
    float: left;
    width: 50%;
}
```

## Project 4. Which of the found items is most similar to the original? {#section_o3y_t4y_tkb}

**Specifications:**

#|
||**Input:**|**Output:**||
||
```json
{
  "image": {
    "type": "url",
    "hidden": false,
    "required": true
  },
  "left_link": {
    "type": "url",
    "hidden": false,
    "required": true
  },
  "right_link": {
    "type": "url",
    "hidden": false,
    "required": true
  }
}
```
|
```json
{
  "result": {
    "type": "url",
    "hidden": false,
    "required": true
  }
}
```
||
|#

**HTML:**

{% if locale == "en-com" %}

```html
<div class="header">
    <div class="left caption"> {{button label="Go to site" href=left_link size="L"}}
        <p class="url">not_var{{left_link}}</p>
    </div>
    <div class="right caption">
        <p class="url">not_var{{right_link}}</p>
        {{button label="Go to site" href=right_link size="L"}}
    </div>
</div> {{img src=image}}
<div class="content clearfix">
    <div class="left page">
        {{iframe src=uploaded_link_left width="100%" height="700px" real-size=true screenshot=true}}
    </div>
    <div class="right page">
        {{iframe src=uploaded_link_right width="100%" height="700px" real-size=true screenshot=true}}
    </div>
</div>
<div class="footer">
    {{field type="radio" name="result" label="Left image is better" value=result_left hotkey="1"}}
    {{field type="radio" name="result" label="Right image is better" value=result_right hotkey="2"}}
</div>
```

{% endif %}

**JavaScript:**

```javascript
exports.Task = extend(TolokaHandlebarsTask, function(options) {
    TolokaHandlebarsTask.call(this, options);
}, {
    getTemplateData: function() {
        var data = TolokaHandlebarsTask.prototype.getTemplateData.apply(this, arguments),
            input = this.getTask().input_values;
        var left_link = input.left_link;
        var right_link = input.right_link;
        var uploaded_link_left = '',
            uploaded_link_right = ''
        if (Math.floor(Math.random() * 2)) {
            uploaded_link_left = left_link
            uploaded_link_right = right_link
        } else {
            uploaded_link_left = right_link
            uploaded_link_right = left_link
        }
        data.uploaded_link_left = uploaded_link_left;
        data.uploaded_link_right = uploaded_link_right;
        data.result_left = uploaded_link_left;
        data.result_right = uploaded_link_right;

        return data;

    },

    onRender: function() {
        // DOM element for task is formed (available via #getDOMElement())
    },
    onDestroy: function() {
        // Task is completed. Global resources can be released (if used)
    }
});

function extend(ParentClass, constructorFunction, prototypeHash) {
    constructorFunction = constructorFunction || function() {};
    prototypeHash = prototypeHash || {};
    if (ParentClass) {
        constructorFunction.prototype = Object.create(ParentClass.prototype);
    }
    for (var i in prototypeHash) {
        constructorFunction.prototype[i] = prototypeHash[i];
    }
    return constructorFunction;
}
```

**CSS:**

```css
.task {
    display: block;
    text-align: center;
}

.header {
    overflow: hidden;
    background-color: #FFCC00;
}

.caption {
    width: 50%;
}

.url {
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;

    max-width: calc(100% - 182px);

    display: inline-block;
    vertical-align: bottom;
}

.button {
    margin: 10px;
    max-width: 182px;
}


.content {
    margin: 10px 0;
}

.page {
    display: inline-block;
    width: 50%;
}

.left {
    float: left;
    text-align: left;
}

.right {
    float: right;
    text-align: right;
}

.clearfix {
    overflow: hidden;
    width: 100%;
}


.image {
    display: inline-block;
    width: 50%;
}.task {
    display: block;
    text-align: center;
}

.header {
    overflow: hidden;
    background-color: #FFCC00;
}

.caption {
    width: 50%;
}

.url {
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;

    max-width: calc(100% - 182px);

    display: inline-block;
    vertical-align: bottom;
}

.button {
    margin: 10px;
    max-width: 182px;
}


.content {
    margin: 10px 0;
}

.page {
    display: inline-block;
    width: 50%;
}

.left {
    float: left;
    text-align: left;
}

.right {
    float: right;
    text-align: right;
}

.clearfix {
    overflow: hidden;
    width: 100%;
}

.image {
    display: inline-block;
    width: 50%;
}
```

{% include [contact-support](../_includes/contact-support.md) %}