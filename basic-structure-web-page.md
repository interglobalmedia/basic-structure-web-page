<h1 class="capitalize">COMD2451</h1>
<h2 class=" capitalize center">Basic Structure of a Web Page</h2>

---

<section class="section">
    <h2 class="sentence">What makes up a basic web page?</h2>

A ***basic*** `web page` is ***made up*** of `HTML`(`5`), `CSS(3)`, and `JavaScript`. `HML5` ***provides*** the `page structure`, `CSS3`, the ***latest*** version of `CSS`, ***released*** in `1999`, ***provides*** the `presentation` (`styling`). `JavaScript` makes things ***happen*** `dynamically` on the `page`.

Since `HTML` was ***first*** [introduced](https://en.wikipedia.org/wiki/HTML) ***by*** `Tim Berners-Lee` in mid 1993 with the **publication** of his ***first*** proposal for an `HTML specification` by [The Internet Engineering Task Force](https://en.wikipedia.org/wiki/Internet_Engineering_Task_Force), an ***open standards*** organization, which ***develops*** and ***promotes*** `voluntary internet standards`, it has ***evolved*** as a `markup language` (`HTML5`) as well as into ***various*** `web technologies` (`HTML5`).

***Specifically***, however, we will ***first*** be `focusing` on the `HTML markup language` which ***provides*** `structure` to the `page`.

</section>

---

<section class="section">
    <h2 class="sentence">What exactly IS HTML?</h2>

`HTML` ***stands*** for `Hyper Text Markup Language`. It ***gives*** content `structure` and `meaning` to a ***page*** by ***defining*** the ***content*** as `headings`, `paragraphs`, `tables`, `lists`, or `images`, for ***example***.
</section>

---

<section class="section">
    <h2 class="sentence">HTML Elements</h2>

When ***learning*** `HTML`, the ***first*** `HTML` **term** one should ***tackle*** is the `HTML element`.

`HTML element`: is an ***individual*** component within an `HTML` document. It ***can*** represent `semantics`, or `meaning`, and it ***defines*** the **structure** and **content** of an `object` ***within*** a `web page`. For ***example***, the `title element` ***represents*** the `title` of the `document`.

`HTML tag`: ***most*** `HTML elements` ***usually*** consist of an `opening` and `closing` ***tag***. For ***example***, the `title` ***tag*** basically **looks** like the ***following***:

```html
<title>This is a title</title>
```

***However***, the `title element` is ***not*** visible on the `web page`. We will get back to that ***later***.

An element's `opening tag` (aka `start tag`) is ***identified*** by its **closure** with a `>` at the ***end*** of the **tag**. The element's `closing tag` (aka `end tag`) is ***identified*** by its **closure** with `</` at the ***beginning*** of the **tag**.

There are ***also*** `self-closing tags`. We will get to that ***later***.

An `HTML element` which is ***visible*** on the `web page` would ***look*** something like ***this***:

```html
<h1 class="main-heading" id="main-heading">Maria's Kitchen</h1>
```

`<h1 class="main-heading" id="main-heading">` is the `start` or `opening tag`, and it ***consists*** of the **following**:

+ A `class attribute` and/or an `id attribute`. ***Here***, the `class attribute` has the `value` of `"main-heading"` and the `id attribute` has the `value` of `"main-heading"` as well. 

`Maria's Kitchen` ***represents*** the **content** of the `h1 element`.

`</h1>` ***represents*** the element's `closing` or `end tag`.

---

<section class="section">
    <h2 class="sentence">Identifying HTML Elements</h2>

`HTML elements` are ***identified*** by the **use** of the `<` and `>` ***angle brackets***, which ***surround*** the `element name`. For ***example***, the `header element` looks like the ***following***:

```html
<header>
    <h1>
      This is a static template, there is no bundler or bundling involved!
    </h1>
    <h2>This is the sub-heading for the static template!</h2>
</header>
```

To **view** the ***live*** `example` of the **a*bove***, please ***visit*** the  [header element](https://codesandbox.io/s/crazy-sanne-3wblj) on [CodeSandbox](https://codesandbox.io/).

As ***indicated*** above, the `HTML element` ***usually*** consists of an `opening` and `closing tag`, and in ***between*** the **tags** is the `element content`.

</section>

---

<section class="section">
    <h2 class="sentence center">HTML Element Index</h2>
</section>

---

<section class="section">
    <h2 class="sentence">The HTML Elements</h2>

The ***following*** is the [list](https://html.spec.whatwg.org/#elements-3) of `HTML elements` as per **Web Hypertext Application Technology Working Group's** `HTML specification` in their `HTML Living Standard docs`:

+ **Document element**
  + `html` (***no*** category, **content model**: a `head` element ***followed*** by a `body` element)
  + can be ***used*** as a document's `document` element
  + can be ***used*** wherever a `sub-document fragment` is ***allowed*** in a **compound document**
+ **Document metadata**
  + `head` (***no*** category, **content model**: if the `document` is an `iframe srcdoc` document or if `title` information is ***available*** from a ***higher*** level **protocol**: zero or more elements of **metadata content**, of which ***no*** more than ***one*** is a `title` element and ***no*** more than ***one*** is a `base` element, ***otherwise***: one or ***more*** elements of **metadata content**, of which ***exactly*** one is a `title` element and ***no*** more than ***one*** is a `base` element)
    + ***used*** as the ***first*** element within an `html` element
  + `title` (metadata content, **content model**: text that is ***not*** inter-element whitespace)
    + ***used*** in a `head` element containing ***no*** other `title` elements
    + **text content model** that is ***not*** inter-element whitespace (which is ***ignored***)
  + `base` (metadata content, ***no*** content model)
    + contains ***no*** end tag
      + can be ***used*** in a `head` element containing ***no*** other `base` elements
        + accepts the `href` attribute, which ***provides*** the Document `base` URL
        + accepts the `target` attribute, which ***provides*** the ***default*** browsing context for **hyperlink** navigation and `form` submission
  + `link` (metadata content, if the element is ***allowed*** in the `body`: flow content, if the element is ***allowed*** in the `body`: phrasing content, ***no*** content model)
    + contains ***no*** end tag
      + can be ***used*** where ***metadata content** is ***expected***
      + can be ***used*** in a `noscript` element that is a ***child*** of a `head` element
      + can be ***used*** in the `body` if it is ***allowed***, where **phrasing content** is expected
        + accepts the `href` attribute, which ***provides*** the address of the hyperlink
        + accepts the `crossorigin` attribute, which ***indicates*** how the element ***handles*** crossorigin requests
        + accepts the `rel` attribute, which ***provides*** the ***relationship*** between the document ***containing*** the hyperlink and the ***destination*** resource
        + accepts the `media` attribute, which ***provides*** the applicable media
        + accepts the `integrity` attribute, which ***provides*** the integrity metadata ***used*** in Sub-resource integrity checks (`SRI`)
        + accepts the `hreflang` attribute, which ***provides*** the language of the ***linked*** resource
        + accepts the `type` attribute, which ***provides*** a hint for the type of the ***referenced*** resource
        + accepts the `referrerpolicy` attribute, which ***provides*** the referrer policy for fetches ***initiated*** by the element
        + accepts the `sizes` attribute, which ***provides*** the sizes of the icons (***for*** `rel="icon"`)
        + accepts the `imagesrcset` attribute, which ***provides*** the images to ***use*** in different situations, e.g., high-resolution displays, small monitors, etc. (***for*** `rel="preload"`)
        + accepts the `imagesizes` attribute, which ***provides*** the image sizes for ***different*** page layouts (***for*** `rel="preload"`)
        + accepts the `as` attribute, which provides the potential destination for a preload request (***for*** `rel="preload"` ***and*** `rel="modulepreload"`)
        + accepts the `color` attribute, which ***provides*** the color to ***use*** when ***customizing*** a site's icon (***for*** `rel="mask-icon"`)
        + accepts the `disabled` attribute, which ***indicates*** whether the link is ***disabled***
        + accepts the `title` attribute, which has a ***special*** semantics on `link`
  + `meta` (metadata content, if the `itemprop`attribute ***is*** present: ***flow content***, if the `itemprop` attribute ***is*** present: ***phrasing content***, ***no*** content model)
    + contains ***no*** end tag
      + can be ***used*** if the `charset` attribute is ***present***, ***or*** if the element's `http-equiv` attribute ***is*** in the Encoding declaration ***state***: in a `head` element
      + can be ***used*** if the `http-equiv` attribute is ***present*** but ***not*** in the Encoding declaration ***state***: in a `head` element
      + can be ***used*** if the `http-equiv` attribute is ***present*** but ***not*** in the Encoding declaration ***state***: in a `noscript` element that is a ***child*** of a `head` element
      + can be ***used*** if the `name` attribute ***is*** present: where **metadata content** is ***expected***
      + can be ***used*** if the `itemprop` attribute ***is*** present: where **metadata content** is ***expected***
      + can be ***used*** if the `itemprop` attribute ***is*** present: where **phrasing content** is ***expected***
      + accepts the `name` attribute, which ***provides*** the metadata ***name***
      + accepts the `content` attribute, which ***provides*** the value of the ***element***
      + accepts the `http-equiv` attribute, which ***provides*** the ***pragma directive***
      + accepts the `charset` attribute, which ***provides*** the character encoding ***declaration***
      + accepts the `itemprop` attribute
        + there must ***not*** be duplicate `meta tags` containing the same state at any given time
  + `style` (metadata content, **content model**: text that gives a ***conformant*** style sheet ***within*** the `style` element)
    + accepts the `media` attribute, which ***provides*** the applicable media
    + accepts the `title` attribute, which has ***special*** semantics on `style`: CSS style sheet ***sets*** the name
+ **Sections**
  + `body` (sectioning root, **content model**: flow content)
    + used as the ***second*** element in an `html` element (placed ***after*** the `head` element)
      + accepts the `onafterprint` attribute
      + accepts the `onbeforeprint` attribute
      + accepts the `onbeforeunload` attribute
      + accepts the `onhashchange` attribute
      + accepts the `onlanguagechange` attribute
      + accepts the `onmessageerror` attribute
      + accepts the `onoffline` attribute
      + accepts the `ononline` attribute
      + accepts the `onpagehide` attribute
      + accepts the `onpageshow` attribute
      + accepts the `onpopstate` attribute
      + accepts the `onrejectionhandled` attribute
      + accepts the `onstorage` attribute
      + accepts the `onunhandledrejection` attribute
      + accepts the `onunload` attribute
  + `article` (flow content, sectioning content, palpable content, **content model**: flow content)
    + can be ***used*** where sectioning content is ***expected***
  + `section` (flow content, sectioning content, palpable content, **content model**: flow content)
    + can be used where sectioning content is ***expected***
  + `nav` (flow content, sectioning content, palpable content, **content model**: flow content)
    + can be ***used*** where sectioning content is ***expected***
  + `aside` (flow content, sectioning content, palpable content, **content model**: flow content)
    + can be ***used*** where sectioning content is ***expected***
  + `h1`, `h2`, `h3`, `h4`, `h5`, `h6` (flow content, heading content, palpable content, **content model**: phrasing content)
    + can be ***used*** as a ***child*** of an `hgroup` element
    + can be ***used*** where heading content is ***expected***
  + `hgroup` (flow content, heading content, palpable content, **content model**: ***one*** or ***more*** `h1-h6` elements, ***optionally*** inter-mixed with ***script-supporting*** elements)
  + `header` (flow content, palpable content, **content model**: flow content, but with ***no*** `header` or `footer` element ***descendants***)
    + can be ***used*** where flow content is ***expected***
  + `footer` (flow content, palpable content, flow content model, but with no header or footer element descendants)
  + `address` (flow content, palpable content, **content model**: flow content, but with ***no*** heading content ***descendants***, ***no*** sectioning content ***descendants***, and ***no*** `header`, `footer`, or `address` element ***descendants***)
    + can be ***used*** where flow content is ***expected***
+ **Grouping content**
  + `p` (flow content, palpable content, **content model**: phrasing content)
    + can be ***used*** where flow content is ***expected***
  + `hr` (flow content, no content model)
    + can be ***used*** where flow content is ***expected***
      + contains ***no*** end tag
  + `pre` (flow content, palpable content, **content model**: phrasing content)
    + can be ***used*** where flow content is ***expected***
  + `blockquote` (flow content, sectioning root, palpable content, **content model**: flow content)
    + can be ***used*** where flow content is ***expected***
    + accepts the `cite` attribute, which links to the source of the **quotation** or ***more*** information about the ***edit***
  + `ol` (flow content, if the element's children ***include*** at ***least*** one `li` element: palpable content, **content model**: zero or ***more*** `li` and ***script-supporting*** elements)
    + can be ***used*** where flow content is ***expected***
      + accepts the `reversed` attribute, which ***numbers*** the list ***backwards*** 
      + accepts the `start` attribute, which ***provides*** the starting value of the ***list***
      + accepts the `type` attribute, which ***provides*** the kind of list marker
  + `ul` (flow content, content model: zero or more li and script-supporting elements)
  + `menu` (flow content, if the element's ***children*** include at ***least*** one `li` element: palpable content, **content model**: zero or ***more*** `li` and ***script-supporting*** elements)
    + can be ***used*** where flow content is ***expected***
  + `li` (***no*** category, **content model**: flow content)
    + can be ***used*** inside `ol`
    + can be ***used*** inside `ul`
    + can be ***used*** inside `menu`
      + accepts the `value` attribute, which ***must be*** a valid integer. 
      + it is ***used*** to ***determine*** the ***ordinal*** value of the list item, when the `li`'s list ***owner*** is an `ol` element
      + if the element is ***not*** a ***child*** of a `ul` or `menu` element: `value` is an ***ordinal*** value of the ***list item***
  + `dl` (flow content, if the element's children ***include*** at ***least*** one name-value ***group***: palpable content, **content model**: either zero or ***more*** groups, each ***consisting*** of one or ***more*** `dt` elements ***followed*** by one or ***more*** `dd` elements, ***optionally*** inter-mixed with ***script-supporting*** elements OR one or ***more*** `div` elements, ***optionally*** inter-mixed with ***script-supporting*** elements)
  + `dt` (***no*** category, **content model**: flow content, but with ***no*** `header`, `footer`, sectioning content, or heading content ***descendants***)
    + can be ***used*** before `dd` or `dt` elements ***inside*** `dl` elements
    + can be ***used*** before `dd` or `dt` elements ***inside*** `div` elements that are ***children*** of a `dl` element
  + `dd` (***no*** category, **content model**: flow content)
    + can be ***used*** after `dt` or `dd` and inside `dl` elements
    + can be ***used*** after `dt` or `dd` and ***inside*** `div` elements that are ***children*** of a `dl` element
  + `figure` (flow content, sectioning root, palpable content, **content model**: either ***one*** `figcaption` element ***followed*** by flow content OR flow content ***followed*** by ***one*** `figcaption` element OR flow content)
    + can be ***used*** where flow content is ***expected***
  + `figcaption` (***no*** category, **content model**: flow content)
    + can be ***used*** as the ***first*** or ***last*** child of a `figure` element
  + `main` (flow content, palpable content, **content model**: flow content)
    + can be ***used*** where flow content is ***expected***, but ***only*** if it is a hierarchically ***correct*** `main` element
  + `div` (flow content, palpable content, **content model**: if the element is a ***child*** of a `dl` element: ***one*** or ***more*** `dt` elements ***followed*** by ***one*** or ***more*** `dd` elements, ***optionally*** inter-mixed with ***script-supporting*** elements, if the element is ***not*** a ***child*** of a `dl` element: flow content)
    + can be ***used*** where flow content is ***expected***
    + can be ***used*** as a ***child*** of a `dl` element
+ **Text-level semantics**
  + `a` (flow content, phrasing content, if the element ***has*** an `href` attribute: interactive content, palpable content, **content model**: transparent, but there ***must*** be ***no*** interactive content ***descendant***, `a` element ***descendant***, or ***descendant*** with the `tabindex` attribute ***specified***)
    + can be ***used*** where phrasing content is ***expected***
      + accepts the `href` attribute, which ***provides*** the address of the hyperlink
      + accepts the `target` attribute, which ***provides*** the browsing context for hyperlink ***navigation***
      + accepts the `download` attribute, which ***indicates*** whether to ***download*** the resource ***instead*** of ***navigating*** to it, and its file name if ***so***
      + accepts the `ping` attribute, which ***provides*** the URLs to ***ping***
      + accepts the `rel` attribute, which ***provides*** the ***relationship*** between the ***location*** in the `document` ***containing*** the hyperlink and the ***destination*** resource
      + accepts the `hreflang` attribute, which ***provides*** the language of the ***linked*** resource
      + accepts the `type` attribute, which ***provides*** a hint for the type of the ***referenced*** resource
      + accepts the `referrerpolicy` attribute, which ***provides*** the referrer policy for fetches ***initiated*** by the element
  + `em` (flow content, phrasing content, palpable content, **content model**: phrasing content)
    + can be ***used*** where phrasing content is ***expected***
  + `strong` (flow content, phrasing content, palpable content, **content model**: phrasing content)
    + can be ***used*** where phrasing content is ***expected***
  + `small` (flow content, phrasing content, palpable content, content model: phrasing content)
    + can be ***used*** where phrasing content is ***expected***
  + `s` (flow content, phrasing content, palpable content, **content model**: phrasing content)
    + can be ***used*** where phrasing content is ***expected***
  + `cite` (flow content, phrasing content, palpable content, **content model**: phrasing content)
    + can be ***used*** where phrasing content is ***expected***
  + `q` (flow content, phrasing content, palpable content, **content model**: phrasing content)
    + can be ***used*** where phrasing content is ***expected***
      + accepts the `cite` attribute, which ***provides*** a link to the ***source*** of the quotation or ***more*** information about the ***edit***
  + `dfn` (flow content, phrasing content, palpable content, **content model**: phrasing content, but there ***must*** be ***no*** `dfn` element ***descendants***)
    + can be ***used*** where phrasing content is ***expected***
    + accepts the `title` attribute, which has ***special*** semantics on `dfn`: full term or expansion of abbreviation
  + `abbr` (flow content, phrasing content, palpable content, **content model**: phrasing content)
    + can be ***used*** where phrasing content is ***expected***
      + accepts the `title` attribute, which has ***special*** semantics on `abbr`: Full term or expansion of abbreviation.
  + `ruby` (flow content, phrasing content, palpable content, **content model**: see prose)
    + can be ***used*** where phrasing content is ***expected***
  + `rt` (***no*** category, **content model**: phrasing content)
    + can be ***used*** as a ***child***of a `ruby` element
  + `rp` (***no*** category, **content model**: text)
    + can be ***used*** as a ***child*** of a `ruby` element, either ***immediately*** before or ***immediately*** after an `rt` element
  + `data` (flow content, phrasing content, palpable content, **content model**: phrasing content)
    + can be ***used*** where phrasing content is ***expected***
      + accepts the `value` attribute with a ***machine-readable*** `value`
  + `time` (flow content, phrasing content, palpable content, **content model**: if the element ***has*** a `datetime` attribute: phrasing content, ***otherwise***: text, but must ***match*** the requirements ***described*** in prose below)
    + accepts the `datetime` attribute with a ***machine-readable*** `value`
  + `code` (flow content, phrasing content, palpable content, **content model**: phrasing content)
    + can be ***used*** where phrasing content is ***expected***
  + `var` (flow content, phrasing content, palpable content, **content model**: phrasing content)
    + can be ***used*** where phrasing content is ***expected***
  + `samp` (flow content, phrasing content, palpable content, **content model**: phrasing content)
    + can be ***used*** where phrasing content is ***expected***
  + `kbd` (flow content, phrasing content, palpable content, **content model**: phrasing content)
    + can be ***used*** where phrasing content is ***expected***
  + `sub`, `sup` (flow content, phrasing content, palpable content, **content model**: phrasing content)
    + can be ***used*** where phrasing content is ***expected***
  + `i` (flow content, phrasing content, palpable content, **content model**: phrasing content)
    + can be ***used*** where phrasing content is ***expected***
      + using `em` instead of `i` is encouraged
  + `b` (flow content, phrasing content, palpable content, **content model**: phrasing content)
    + can be ***used*** where phrasing content is ***expected***
      + using `h1 - h6` for ***headings***, `em` for ***stress emphasis***, and `strong` for ***importance*** instead of `b` are ***encouraged***
  + `u` (flow content, phrasing content, palpable content, **content model**: phrasing content)
    + can be ***used*** where phrasing content is ***expected***
    + in ***most*** cases, ***another*** element is likely to be ***more*** appropriate: for marking ***stress emphasis***, the `em` element ***should*** be used; for marking ***key words*** or ***phrases*** either the `b` element or the `mark` element ***should*** be used, ***depending*** on the context; for marking ***book titles***, the `cite` element ***should*** be used; for ***labeling*** text with ***explicit*** textual annotations, the `ruby` element should be used; for ***technical*** terms, ***taxonomic*** designation, ***transliteration***, a ***thought***, or for ***labeling*** ship names in Western texts, the `i` element ***should*** be used
  + `mark` (flow content, phrasing content, palpable content, **content model**: phrasing content)
    + can be ***used*** where phrasing content is ***expected***
  + `bdi` (flow content, phrasing content, palpable content, **content model**: phrasing content)
    + can be ***used*** where phrasing content is ***expected***
      + the `dir` ***global*** attribute has ***special*** semantics on `bdi`
  + `bdo` (flow content, phrasing content, palpable content, **content model**: phrasing content)
    + can be ***used*** where phrasing content is ***expected***
    + the `dir` ***global*** attribute, has ***special*** semantics on `bdo`
    + authors ***must*** specify the `dir` attribute, with ***either*** `ltr` or `rtl` values
  + `span` (flow content, phrasing content, palpable content, **content model**: phrasing content)
    + can be ***used*** where phrasing content is ***expected***
  + `br` (flow content, phrasing content, **content model**: none)
    + can be ***used*** where phrasing content is ***expected***
      + contains ***no*** end tag
  + `wbr` (flow content, phrasing content, **content model**: none)
    + can be ***used*** where phrasing content is ***expected***
    + contains ***no*** end tag
+ **Edits**
  + `ins` (flow content, phrasing content, palpable content, **content model**: transparent)
    + can be ***used*** where phrasing content is ***expected***
      + accepts the `cite` attribute, which ***links*** to the **source** of the quotation or ***more*** information about the **edit**
      + accepts the `datetime` attribute, which ***provides*** the **date** and (optionally) the **time** of the change/edit (the `datetime` value may be ***shown*** to the user, but it is ***primarily*** intended for ***private*** use)
        + `ins` elements should ***not*** cross ***implied*** paragraph boundaries (in other words, there should be ***one*** `ins` element ***per*** piece of text)
  + `del` (flow content, phrasing content, **content model**: transparent)
    + can be ***used*** where phrasing content is ***expected***
      + accepts the `cite` attribute, which ***links*** to the **source** of the quotation or ***more*** information about the **edit**
      + accepts the `datetime` attribute, which ***provides*** the **date** and (optionally) the **time** of the change/edit (the `datetime` value may be ***shown*** to the user, but it is ***primarily*** intended for ***private***å use)
        + `del` elements should ***not*** cross ***implied*** paragraph boundaries
+ **Embedded content**
  + `picture` (flow content, phrasing content, embedded content, **content model**: ***zero*** or ***more*** `source` elements, ***followed*** by ***one*** `img` element, ***optionally*** inter-mixed with ***script-supporting*** elements)
    + can be ***used*** where embedded content is ***expected***
  + `source` (***no*** category, ***no*** content model)
    + contains ***no*** end tag
      + accepts the `src` attribute, which is the ***address*** of the resource
      + accepts the `type` attribute, which is the ***type*** of the embedded resource
      + accepts the `srcset` attribute, which ***image*** to use in ***different*** situations, e.g., high-resolution displays, small monitors, etc
      + accepts the `sizes` attribute, which are ***different*** image sizes for ***different*** page layouts
      + accepts the `media` attribute, for ***applicable*** media
  + `img` (flow content, phrasing content, embedded content, form-associated element, if the element ***has*** a `usemap` attribute: interactive content, palpable content, **content model**: none)
    + can be ***used*** where embedded content is ***expected***
      + contains ***no*** end tag
        + accepts the `alt` attribute, which is ***replacement*** text for use when **images** are ***not*** available
        + accepts the `src` attribute, which is the ***address*** of the resource
        + accepts the `srcset` attribute, which ***images*** use in ***different*** situations, e.g., high-resolution displays, small monitors, etc
        + accepts the `sizes` attribute, which are ***different*** image sizes for ***different*** page layouts
        + accepts the `crossorigin` attribute, which is ***how*** the element ***handles*** crossorigin requests
        + accepts the `usemap` attribute, which is the ***name*** of the ***image map*** to use
        + accepts the `ismap` attribute, which ***indicates*** whether the image is a ***server-side*** image map
        + accepts the `width` attribute, which is the ***horizontal*** dimension of the image
        + accepts the `height` attribute, which is the ***vertical*** dimension of the image
        + accepts the `referrerpolicy` attribute, which is the referrer policy for fetches ***initiated*** by the element
        + accepts the `decoding` attribute, which is the decoding ***hint*** to use when ***processing*** the image for presentation
        + accepts the `loading` attribute, which is used when ***determining*** loading ***deferral***
  + `iframe` (flow content, phrasing content, embedded content, interactive content, palpable content, **content model**: none)
    + can be ***used*** where embedded content is ***expected***
      + accepts the `src` attribute, which ***provides*** the address of the resource
      + accepts the `srcdoc` attribute, which is a **document** to ***render*** in the `iframe`
      + accepts the `name` attribute, which is the name of the ***nested*** browsing context (name of/attributed to the ***embedded*** `iframe`)
      + accepts the `sandbox` attribute, which ***provides*** the security rules for nested content
      + accepts the `allow` attribute, which ***provides*** the permissions policy to be ***applied*** to the `iframe`'s contents
      + accepts the `allowfullscreen` attribute, which ***indicates*** whether to ***allow*** the `iframe`'s contents to ***use*** `requestFullscreen()` method
      + accepts the `width` attribute, which ***provides*** the element's ***horizontal*** direction
      + accepts the `height` attribute, which ***provides*** the element's ***vertical*** dimension
      + accepts the `referrerpolicy` attribute, which ***provides*** the referrer policy for fetches ***initiated*** by the element
      + accepts the `loading` attribute, which is ***used*** when ***determining*** loading ***deferral***
  + `embed` (flow content, phrasing content, embedded content, interactive content, palpable content, **content model**: none)
    + can be ***used*** where embedded content is ***expected***
      + contains ***no*** end tag
        + accepts the `src` attribute, which ***provides*** the address of the resource
        + accepts the `type` attribute, which ***provides*** the type of the ***embedded*** resource
        + accepts the `width` attribute, which ***provides*** the element's ***horizontal*** dimension
        + accepts the `height` attribute, which ***provides*** the element's ***vertical*** dimension
  + `object` (flow content, phrasing content, embedded content, if the element has a `usemap` attribute: interactive content, listed form-associated element, palpable content, **content model**: if zero or more `param` elements, then ***transparent***)
    + can be ***used*** where embedded content is ***expected***
    + accepts the `data` attribute, which ***provides*** the address of the resource
      + accepts the `type` attribute, which ***provides*** the type of ***embedded*** resource
      + accepts the `name` attribute, which ***provides*** the name of the ***nested*** browsing context (name of/attributed to the `object`)
      + accepts the `usemap` attribute, which ***provides*** the name of the image map to ***use***
      + accepts the `form` attribute, which ***associates*** the element with a `form` element
      + accepts the `width` attribute, which ***provides*** the element's ***horizontal*** dimension
      + accepts the `height` attribute, which ***provides*** the element's ***vertical*** dimension
  + `param` (***no*** category, ***no*** content model)
    + can be ***used*** as a ***child*** of an `object` element, ***before*** any flow content
      + contains ***no*** end tag
        + accepts the `name` attribute, which ***provides*** the name of the ***parameter***
        + accepts the `value` attribute, which ***provides*** the `value` of the ***parameter***
  + `video` (flow content, phrasing content, embedded content, if the element has a `controls` attribute: interactive content, palpable content, **content model**: if the element has a `src` attribute: ***zero*** or ***more*** `track` elements, then ***transparent***, but with ***no*** `media` element ***descendants***; if the element does ***not*** have a `src` attribute: ***zero*** or ***more*** `source` elements, then ***zero*** or ***more*** `track` elements, then ***transparent***, but with ***no*** `media` element ***descendants***)
    + can be ***used*** where embedded content is ***expected***
      + accepts the `src` attribute, which is the ***address*** of the resource
      + accepts the `crossorigin` attribute, which is ***how*** the element ***handles*** crossorigin requests
      + accepts the `poster` attribute, which is a ***poster frame*** to ***show*** prior `video` playback
      + accepts the `preload` attribute, which ***hints*** how much ***buffering*** the media resource will likely ***need***
      + accepts the `autoplay` attribute, which ***hints*** that the media resource can be ***started automatically*** when the page is ***loaded***
      + accepts the `playsinline` attribute, which ***encourages*** the user agent to ***display*** `video` content ***within*** the element's playback area
      + accepts the `loop` attribute, which ***indicates*** whether to ***loop*** the media resource
      + accepts the `muted` attribute, which ***indicates*** whether to ***mute*** the media resource by ***default***
      + accepts the `controls` attribute, which ***shows*** the user agent ***controls***
      + accepts the `width` attribute, which ***provides*** the element's ***horizontal*** dimension
      + accepts the `height` attribute, which ***provides*** the element's ***vertical*** dimension
  + `audio` (flow content, phrasing content, embedded content, if the element ***has*** a `controls` attribute: interactive content, if the element ***has*** a `controls` attribute: palpable content, **content model**: if the element ***has*** a `src` attribute: ***zero*** or ***more*** `track` elements, then ***transparent***, but with ***no*** `media` element ***descendants***; if the element does ***not*** have a `src` attribute: ***zero*** or ***more*** `source` elements, then ***zero*** or ***more*** `track` elements, then ***transparent***, but with ***no*** `media` element ***descendants***)
    + can be ***used*** where embedded content is ***expected***
      + accepts the `src` attribute, which ***provides*** the address of the resource
      + accepts the `crossorigin` attribute, which ***indicates*** how the element ***handles*** crossorigin requests
      + accepts the `preload` attribute, which ***hints*** how much ***buffering*** the media resource will likely ***need***
      + accepts the `autoplay` attribute, which ***hints*** that the media resource can be ***started automatically*** when the page is ***loaded***
      + accepts the `loop` attribute, which ***indicates*** whether to ***loop*** the media resource
      + accepts the `muted` attribute, which ***indicates*** whether to ***mute*** the media resource by ***default***
      + accepts the `controls` attribute, which ***shows*** the user agent ***controls***
  + `track` (***no*** category, ***no*** content model)
    + can be ***used*** as a ***child*** of a `media` element, ***before*** any flow content
      + contains ***no*** end tag
        + accepts the `kind` attribute, which ***indicates*** the type of text `track`
        + accepts the `src` attribute, which ***provides*** the address of the resource
        + accepts the `srclang` attribute, which ***provides*** the language of the text `track`
        + accepts the `label` attribute, which ***provides*** the user-visible ***label***
        + accepts the `default` attribute, which ***enables*** the `track` if ***no*** other text `track` is ***more*** suitable
  + `map` (flow content, phrasing content, palpable content, **content model**: transparent)
    + can be ***used*** where phrasing content is ***expected***
      + accepts the `name` attribute, which ***provides*** the name of the **image map** to ***reference*** from the `usemap` attribute
  + `area` (flow content, phrasing content, **content model**: none)
    + can be ***used*** where phrasing content is ***expected***
      + accepts the `alt` attribute, which is ***replacement*** text for **use** when images are ***not*** available
      + accepts the `coords` attribute, which ***provides*** the coordinates for the ***shape*** to be ***created*** in an **image map**
      + accepts the `href` attribute, which ***provides*** the address of the ***hyperlink***
      + accepts the `target` attribute, which ***provides*** the browsing context for ***hyperlink navigation***
      + accepts the `download` attribute, which ***indicates*** whether to ***download*** the resource ***instead*** of navigating to it, and its ***file name*** if so
      + accepts the `ping` attribute, which ***provides*** the URLs to ***ping***
      + accepts the `rel` attribute, which ***provides*** the ***relationship*** between the **location** in the document ***containing*** the hyperlink and the ***destination*** resource
      + accepts the `referrerpolicy` attribute, which ***provides*** the referrer policy for fetches ***initiated*** by the element
  + (MathML) `math` (embedded content, phrasing content, flow content, palpable content, ***when*** the MathML `annotation-xml` element ***contains*** elements from the `HTML` namespace, ***such*** elements must ***all*** be **flow content**; ***when*** the MathML `token` elements (`mi`, `mo`, `mn`, `ms`, and `mtext`) are ***descendants*** of `HTML` elements, they ***may*** contain **phrasing content** elements ***from*** the `HTML` namespace)
  + `SVG` (embedded content, phrasing content, flow content, palpable content, ***when*** the `SVG` `foreignObject` element ***contains*** elements ***from*** the `HTML` ***namespace***, ***such*** elements must ***all*** be **flow content**; the **content model** for the `SVG` `title` element ***inside*** `HTML documents` is **phrasing content**. (this ***further*** constrains the ***requirements*** given in `SVG 2`))
    + the ***semantics*** of `SVG` elements are ***defined*** by `SVG 2` and [other applicable specifications](https://html.spec.whatwg.org/#other-applicable-specifications)
+ **Tabular data**
  + `table` (flow content, palpable content, **content model**: in ***this*** order: ***optionally*** a `caption` element, ***followed*** by ***zero*** or ***more*** `colgroup` elements, followed ***optionally*** by a `thead` element, followed by ***either*** zero or more `tbody` elements ***or*** one or more `tr` elements, followed ***optionally*** by a `tfoot` element, ***optionally*** inter-mixed with one or more ***script-supporting*** elements)
    + can be ***used*** where flow content is ***expected***
  + `caption` (***no*** category, **content model**: flow content, but with ***no*** descendant `table` elements)
    + can be ***used*** as the ***first*** element child of a `table` element
  + `colgroup` (***no*** category, **content model**: if the `span` attribute ***is*** present: ***none***, if the `span` attribute is ***absent***: zero or more `col` and `template` elements)
    + can be ***used*** as a ***child*** of a `table` element, ***after*** any `caption` elements and ***before*** any `thead`, `tbody`, `tfoot`, and `tr` elements
      + accepts the `span` attribute, which ***provides*** the number of columns ***spanned*** by the element
  + `col` (***no*** category, ***no*** content model)
    + can be ***used*** as a ***child*** of a `colgroup` element that ***doesn't*** have a `span` attribute
      + contains ***no*** end tag
        + accepts the `span` attribute, which ***provides*** the number of columns ***spanned*** by the element
  + `tbody` (***no*** category, **content model**: ***zero*** or ***more*** `tr` and ***script-supporting*** elements)
    + can be ***used*** as a ***child*** of a `table` element, ***after*** any `caption`, `colgroup`, and `thead` elements, but ***only*** if there are ***no*** `tr` elements that are ***children*** of the `table` element
  + `thead` (***no*** category. **content model**: ***zero*** or ***more*** `tr` and ***script-supporting*** elements)
    + can be ***used*** as a ***child*** of a `table` element, ***after*** any `caption` and `colgroup` elements and ***before*** any `tbody`, `tfoot`, and `tr` elements, but ***only*** if there are ***no*** other `thead` elements that are ***children*** of the `table` element
  + `tfoot` (***no*** category, **content model**: ***zero*** or ***more*** `tr` and ***script-supporting*** elements)
    + can be ***used*** as a ***child*** of a `table` element, ***after*** any `caption`, `colgroup`, `thead`, `tbody`, and `tr` elements, but ***only*** if there are ***no*** other `tfoot` elements that are ***children*** of the `table` element
  + `tr` (***no*** category, **content model**: ***zero*** or ***more*** `td`, `th`, and ***script-supporting*** elements)
    + can be ***used*** as a ***child*** of a `thead` element
    + can be ***used*** as a ***child*** of a `tbody` element
    + can be ***used*** as a ***child*** of a `tfoot` element
    + can be ***used*** as a ***child*** of a `table` element, ***after*** any `caption`, `colgroup`, and `thead` elements, but ***only*** if there are ***no*** `tbody` elements that are ***children*** of the `table` element
  + `td` (sectioning root, **content model**: flow content)
    + can be ***used*** as a ***child*** of a `tr` element
      + accepts the `colspan` attribute, which ***indicates*** the number of columns that the **cell** is to ***span***
      + accepts the `rowspan` attribute, which ***indicates*** the number of rows that the **cell** is to ***span***
      + accepts the `headers` attribute, which ***indicates*** the **header cells** for the ***cell***
  + `th` (***no*** category, **content model**: flow content, but with ***no*** `header`, `footer`, sectioning content, or heading content ***descendants***)
    + can be ***used*** as a ***child*** of a `tr` element
      + accepts the `colspan` attribute, which ***indicates*** the number of columns that the **cell** is to ***span***
      + accepts the `rowspan` attribute, which ***indicates*** the number of rows that the **cell** is to ***span***
      + accepts the `headers` attribute, which ***indicates*** the **header cells** for the ***cell***
      + accepts the `scope` attribute, which ***specifies*** which cells the **header cell** applies to
      + accepts the `abbr` attribute, which is an ***alternative*** label to ***use*** for the **header cell** when ***referencing*** the cell in ***other*** contexts
+ **Forms**
  + `form` (flow content, palpable content, **content model**: flow content, but with ***no*** `form` element ***descendants***)
    + can be ***used*** where flow content is ***expected***
      + accepts the `accept-charset` attribute, which ***provides*** the character encodings to ***use*** for `form` submission
      + accepts the `action` attribute, which ***provides*** the URL to ***use*** for `form` submission
      + accepts the `autocomplete` attribute, which ***provides*** the ***default*** setting for the **autofill** feature for ***controls*** in the `form`
      + accepts the `enctype` attribute, which ***provides*** the entry list encoding type to ***use*** for `form` submission
      + accepts the `method` attribute, which ***provides*** the **variant** to ***use*** for `form` submission
      + accepts the `name` attribute, which ***provides*** the name of the `form` to ***use*** in the `document.forms API`
      + accepts the `novalidate` attribute, which ***bypasses*** `form` control validation for `form` submission
      + accepts the `target` attribute, which ***provides*** the browsing context for `form` submission
      + accepts the `rel` attribute, which ***specifies*** the ***relationship*** between the ***current*** document and the ***linked*** document
  + `label` (flow content, phrasing content, interactive content, palpable content, **content model**: phrasing content, but with ***no*** descendant ***labelable*** elements ***unless*** it is the element's **labeled control** (the label's `for` attribute), and ***no*** descendant `label` elements)
    + can be ***used*** where phrasing content is ***expected***
      + accepts the `for` attribute, which ***associates*** the `label` with the `form` control (`input`)
  + `input` (flow content, phrasing content, if the `type` attribute is ***not*** in the Hidden ***state***: interactive content, if the `type` attribute is ***not*** in the Hidden ***state***:  listed, labelable, submittable, resettable, and autocapitalize-inheriting form-associated element, if the `type` attribute ***is*** in the Hidden ***state***: listed, submittable, resettable, and autocapitalize-inheriting form-associated element, and if the `type` attribute is ***not*** in the Hidden ***state***: palpable content, **content model**: none)
    + can be ***used*** where phrasing content is ***expected***
      + contains ***no*** end tag
        + accepts the `accept` attribute, which ***provides*** a hint of the ***expected*** file type in file upload ***controls***
        + accepts the `alt` attribute, which is ***replacement*** text for ***use*** when images are ***not*** available
        + accepts the `autocomplete` attribute, which ***provides*** a hint for the `form` autofill feature
        + accepts the `checked` attribute, which ***indicates*** whether the **control** is ***checked***
        + accepts the `dirname` attribute, which ***provides*** the name of the `form` control to ***use*** for ***sending*** the element's ***directionality*** in `form` submission
        + accepts the `disabled` attribute, which ***indicates*** whether the `form` control is ***disabled***
        + accepts the `form` attribute, which ***associates*** the element with a `form` element
        + accepts the `formaction` attribute, which ***provides*** the URL to ***use*** for `form` submission
        + accepts the `formenctype` attribute, which ***provides*** the entry list encoding type to ***use*** for `form` submission
        + accepts the `formmethod` attribute, which ***provides*** a **variant** to ***use*** for `form` submission
        + accepts the `formnovalidate` attribute, which ***bypasses*** `form` control ***validation*** for `form` submission
        + accepts the `formtarget` attribute, which ***provides*** the browsing context for `form` submission
        + accepts the `height` attribute, which ***provides*** the element's ***vertical*** dimension
        + accepts the `list` attribute, which ***provides*** a list of `autocomplete` options
        + accepts the `max` attribute, which ***provides*** the ***maximum*** value ***allowed***
        + accepts the `maxlength` attribute, which ***provides*** the maximum length ***allowed***
        + accepts the `min` attribute, which ***provides*** the ***minimum*** value ***allowed***
        + accepts the `minlength` attribute, which ***provides*** the minimum length ***allowed***
        + accepts the `multiple` attribute, which ***indicates*** whether to ***allow*** multiple values
        + accepts the `name` attribute, which ***provides*** the name of the element to use for `form` submission
        + accepts the `pattern` attribute, which ***provides*** the ***pattern*** to be ***matched*** by the `form` control's value
        + accepts the `placeholder` attribute, which ***provides*** the ***user-visible*** label to be ***placed*** within the `form` control
        + accepts the `readonly` attribute, which ***indicates*** whether to ***allow*** the value to be ***edited*** by the **user**
        + accepts the `required` attribute, which ***indicates*** whether the control is ***required*** for `form` submission
        + accepts the `size` attribute, which ***provides*** the size of the control
        + accepts the `src` attribute, which ***provides*** the address of the resource
        + accepts the `step` attribute, which ***provides*** granularity to be ***matched*** by the `form` control's ***value***
        + accepts the `type` attribute, which ***provides*** the type of `form` control
        + accepts the `value` attribute, which ***provides*** the value of the `form` control
        + accepts the `width` attribute, which ***provides*** the element's ***horizontal*** dimension
        + accepts the `title` attribute, which has ***special*** semantics on `input`
  + `button` (flow content, phrasing content, interactive content, listed, labelable, submittable, and autocapitalize-inheriting form-associated element, palpable content, **content model**: phrasing content, but there ***must*** be ***no*** interactive content ***descendant*** and ***no*** descendant with the `tabindex` attribute ***specified***)
    + can be ***used*** where phrasing content is ***expected***
      + accepts the `disabled` attribute, which ***indicates*** whether the `form` control is ***disabled***
      + accepts the `form` attribute, which ***associates*** the element with a `form` element
      + accepts the `formaction` attribute, which ***provides*** the URL to ***use*** for `form` submission
      + accepts the `formenctype` attribute, which ***provides*** the entry list encoding type to ***use*** for `form` submission
      + accepts the `formmethod` attribute, which ***provides*** the **variant** to ***use*** for `form` submission
      + accepts the `formnovalidate` attribute, which ***bypasses*** `form` control ***validation*** for `form` submission
      + accepts the `formtarget` attribute, which ***provides*** the browsing context for `form` submission
      + accepts the `name` attribute, which ***provides*** the name of the element to ***use*** for `form` submission
      + accepts the `type` attribute, which ***provides*** the type of button
      + accepts the `value` attribute, which ***provides*** the value to be ***used*** for `form` submission
  + `select` (flow content, phrasing content, interactive content, listed, labelable, submittable, resettable, and autocapitalize-inheriting form-associated element, palpable content, **content model**: ***zero*** or ***more*** `option`, `optgroup`, and ***script-supporting*** elements)
    + can be ***used*** where phrasing content is ***expected***
      + accepts the `autocomplete` attribute, which ***provides*** a hint for the `form` autofill feature
      + accepts the `disabled` attribute, which ***indicates*** whether the `form` control is ***disabled***
      + accepts the `form` attribute, which ***associates*** the element with a `form` element
      + accepts the `multiple` attribute, which ***indicates*** whether to ***allow*** multiple values
      + accepts the `name` attribute, which ***provides*** the name of the element to ***use*** for `form` submission
      + accepts the `required` attribute, which ***indicates*** whether the control is ***required*** for `form` submission
      + accepts the `size` attribute, which ***provides*** the size of the control
  + `datalist` (flow content, phrasing content, **content model**: ***either*** phrasing content, ***or*** zero or more `option` and ***script-supporting*** elements)
    + can be ***used*** where phrasing content is ***expected***
  + `optgroup` (***no*** category, **content model**: ***zero*** or ***more*** `option` and ***script-supporting*** elements)
    + can be ***used*** as a ***child*** of a `select` element
      + accepts the `disabled` attribute, which ***indicates*** whether the `form` control is ***disabled***
      + accepts the `label` attribute, which ***provides*** the ***user-visible*** label
  + `option` (***no*** category, **content model**: if the element ***has*** a `label` attribute ***and*** a `value` attribute: ***none***, if the element ***has*** a `label` attribute but ***no*** `value` attribute: ***text***, if the element has ***no*** `label` attribute and is ***not*** a ***child*** of a `datalist` element: **text** that is ***not*** inter-element whitespace, ***and*** if the element has ***no*** `label` attribute and is a ***child*** of a `datalist` element: **text**)
    + can be ***used*** as a ***child*** of a `select` element
    + can be ***used*** as a ***child*** of a `datalist` element
    + can be ***used*** as a ***child*** of an `optgroup` element
      + accepts the `disabled` attribute, which ***indicates*** whether the `form` control is ***disabled***
      + accepts the `label` attribute, which ***provides*** the ***user-visible*** `label`
      + accepts the `selected` attribute, which ***indicates*** whether the `option` is selected by ***default***
      + accepts the `value` attribute, which ***provides*** the value to be ***used*** for `form` submission
  + `textarea` (flow content, phrasing content, interactive content, listed, labelable, submittable, resettable, and autocapitalize-inheriting form-associated element, palpable content, **content model**: text)
    + can be ***used*** where phrasing content is ***expected***
      + accepts the `autocomplete` attribute, which ***provides*** a hint for the `form` autofill feature
      + accepts the `cols` attribute, which ***provides*** the maximum number of characters per ***line***
      + accepts the `dirname` attribute, which ***provides*** the name of the `form` control to ***use*** for ***sending*** the element's ***directionality*** in `form` submission
      + accepts the `disabled` attribute, which ***indicates*** whether the `form` control is ***disabled***
      + accepts the `form` attribute, which ***associates*** the element with a `form` element
      + accepts the `maxlength` attribute, which ***provides*** the maximum length of a value ***allowed***
      + accepts the `minlength` attribute, which ***provides*** the minimum length of a value ***allowed***
      + accepts the `name` attribute, which ***provides*** the name of the element to ***use*** for `form` submission ***and*** in the `form.elements API`
      + accepts the `placeholder` attribute, which ***provides*** the ***user-visible*** label to be ***placed*** within the `form` control
      + accepts the `readonly` attribute, which ***indicates*** whether to ***allow*** the value to be ***edited*** by the user
      + accepts the `required` attribute, which ***indicates*** whether the control is ***required*** for form submission
      + accepts the `rows` attribute, which ***provides*** the number of lines to ***show***
      + accepts the ***wrap*** attribute, which ***indicates*** how the value of the `form` control is to be ***wrapped*** for `form` submission
  + `output` (flow content, phrasing content, listed, labelable, resettable, and autocapitalize-inheriting form-associated element, palpable content, **content model**: phrasing content)
    + can be ***used*** where phrasing content is ***expected***
      + accepts the `for` attribute, which ***specifies*** controls from which the `output` was ***calculated***
      + accepts the `form` attribute, which ***associates*** the element with a `form` element
      + accepts the `name` attribute, which ***provides*** the name of the element to ***use*** in the `form.elements API`
  + `progress` (flow content, phrasing content, labelable element, palpable content, **content model**: phrasing content, but there must be ***no*** `progress` element ***descendants***)
    + can be ***used*** where phrasing content is ***expected***
      + accepts the `value` attribute, which ***provides*** the ***current*** value of the element
      + accepts the `max` attribute, which ***provides*** the ***upper*** bound of ***range***
  + `meter` (flow content, phrasing content, labelable element, palpable content, **content model**: phrasing content, but there ***must*** be ***no*** `meter` element ***descendants***)
    + can be ***used*** where phrasing content is ***expected***
      + accepts the `value` attribute, which ***provides*** the ***current*** value of the element
      + accepts the `min` attribute, which ***provides*** the ***lower*** bound of ***range***
      + accepts the `max` attribute, which ***provides*** the ***upper*** bound of ***range***
      + accepts the `low` attribute, which ***provides*** the ***high*** limit of ***low*** range
      + accepts the `high` attribute, which ***provides*** the ***low*** limit of ***high*** range
      + accepts the `optimum` attribute, which ***provides*** the ***optimum*** value in ***gauge***
  + `fieldset` (flow content, sectioning content, listed and autocapitalize-inheriting form-associated element, palpable content, **content model**: ***optionally*** a `legend` element, ***followed*** by flow content)
    + can be ***used*** where flow content is ***expected***
      + accepts the `disabled` attribute, which ***indicates*** whether the ***descendant*** `form` controls, ***except*** any ***inside*** `legend`, are ***disabled***
      + accepts the `form` attribute, which ***associates*** the element with a `form` element
      + accepts the `name` attribute, which ***provides*** the name of the element to ***use*** in the `form.elements API`
  + `legend` (***no*** category, **content model**: phrasing content, ***optionally*** inter-mixed with heading content)
    + can be ***used*** as the ***first*** child of a `fieldset` element
+ **Interactive elements**
  + `details` (flow content, sectioning root, interactive content, palpable content, **content model**: ***one*** `summary` element ***followed*** by flow content)
    + can be ***used*** where flow content is ***expected***
      + accepts the `open` attribute, which ***indicates*** whether the `details` are ***visible***
  + `summary` (***no*** category, **content model**: phrasing content, ***optionally*** inter-mixed with heading content)
    + can be ***used*** as the ***first*** child of a `details` element
  + `dialog` (flow content, sectioning root, **content model**: flow content)
    + can be ***used*** where flow content is ***expected***
      + accepts the `open` attribute, which ***indicates*** whether the `dialog` box is ***showing***
+ **Scripting**
  + `script` (metadata content, flow content, phrasing content, script-supporting element, **content model**: if there is ***no*** `src` attribute, ***depends*** on the ***value*** of the `type` attribute, but ***must*** match `script` content restrictions, if there ***is*** a `src` attribute, the element ***must*** be ***either*** empty ***or*** contain ***only*** `script` documentation that ***also*** matches `script` content ***restrictions***)
    + can be ***used*** where metadata content is ***expected***
    + can be ***used*** where phrasing content is ***expected***
    + can be ***used*** where ***script-supporting*** elements are ***expected***
      + accepts the `src` attribute, which ***provides*** the address of the ***resource***
      + accepts the `type` attribute, which ***provides*** the type of ***script***
      + accepts the `nomodule` attribute, which ***prevents*** execution in user agents that ***support*** module scripts
      + accepts the `async` attribute, which ***executes*** a `script` when ***available***, ***without*** blocking ***while*** fetching
      + accepts the `defer` attribute, which ***defers*** script ***execution***
      + accepts the `crossorigin` attribute, which ***indicates*** how the element ***handles*** crossorigin requests
      + accepts the `integrity` attribute, which ***provides*** the integrity metadata ***used*** in the Subresource Integrity checks (`SRI`)
      + accepts the `referrerpolicy` attribute, which ***provides*** the referrer policy for fetches ***initiated*** by the element
  + `noscript` (metadata content, flow content, phrasing content, **content model**: when ***scripting*** is ***disabled***, in a `head` element: in ***any*** order, ***zero*** or ***more*** `link` elements, ***zero*** or ***more*** `style` elements, and ***zero*** or ***more*** `meta` elements, when ***scripting*** is ***disabled***, ***not*** in a `head` element: ***transparent***, but there ***must*** be ***no*** `noscript` element ***descendants***, ***otherwise***: text that ***conforms*** to the ***requirements*** given in the ***prose***)
    + can be ***used*** in a `head` element of an `HTML` document, if there are ***no*** ancestor `noscript` elements
    + can be ***used*** where phrasing content is ***expected*** in `HTML` documents, if there are ***no*** ancestor `noscript` elements
  + `template` (metadata content, flow content, phrasing content, script-supporting element, **content model**: none)
    + can be ***used*** where metadata content is ***expected***
    + can be ***used*** where phrasing content is ***expected***
    + can be ***used*** as a ***child*** of a `colgroup` element that ***doesn't*** have a `span` attribute
  + `slot` (flow content, phrasing content, **content model**: transparent)
    + can be ***used*** where phrasing content is ***expected***
      + accepts the `name` attribute, which ***provides*** the name of the ***shadow tree*** `slot`
  + `canvas` (flow content, phrasing content, embedded content, palpable content, **content model**: transparent, but with ***no*** interactive content ***descendants*** except for `a` elements, `img` elements ***with*** `usemap` attributes, `button` elements, `input` elements whose `type` attribute are in the `Checkbox` or `Radio Button` ***states***, `input` elements that ***are*** `buttons`, and `select` elements with a `multiple` attribute ***or*** a display size ***greater*** than 1)
    + can be ***used*** where embedded content is ***expected***
      + accepts the `width` attribute, which ***provides*** the element's ***horizontal*** dimension
      + accepts the `height` attribute, which ***provides*** the element's ***vertical*** dimension
+ (Autonomous) custom elements

</section>

---

<section class="section">
    <h2 class="sentence">The HTML Tag</h2>

When ***learning*** `HTML`, the ***second*** `HTML` term one should ***tackle*** is the `HTML tag`.

***Whereas*** an `HTML element` ***consists*** of an `opening` and `closing tag`, an `HTML` tag can ***either*** be an `opening` or `closing tag`, or a `self-closing tag`.  

The ***following*** is an **example** of an `opening section element` ***tag***:

```html
<section>
```

The `opening tag` ***starts*** with the less than `<` angle bracket, ***followed*** by the `name` of the `element`, and ***ends*** with the greater than `>` angle bracket.

An ***example*** of a `closing section element` ***tag***:

```html
</section>
```

The `closing tag` ***starts*** with the less than `<` angle bracket, ***followed*** by a forward slash `/`, ***then*** the `name` of the `element`, and ***ending*** with the greater than `>` angle bracket.

</section>

---

<section class="section">
    <h2 class="sentence">The HTML Attribute</h2>

An `HTML attribute` is a **property** which ***provides*** additional ***information*** about an `element`.

An `HTML attribute` is ***always*** placed in the `opening tag` of the `HTML` element, ***if*** there is ***both*** an ***opening*** and ***closing*** `HTML tag`.

The **format** for ***defining*** an `HTML attribute` is the `name` of the `HTML attribute`, ***followed*** by an `=` sign, and ***then*** the `value` of the `attribute`, ***enclosed*** in `quotes`.

</section>

---

<section class="section">
    <h2 class="sentence">Acceptable HTML Attribute values and the value attribute</h2>

***According*** to the **Web Hypertext Application Technology Working Group** (**WHATWG**) [HTML Living Standard specification](https://html.spec.whatwg.org/#attributes-2), `HTML` attributes can be `"specified in four different ways"`:

+ `Empty attribute syntax`: when ***just*** the attribute name is ***provided***. The `value` is ***implicitly*** an `empty string`.

```html
<input required>
```

The `required` attribute is ***added*** with the `empty attribute syntax`.

If an attribute ***using*** the `empty attribute syntax` is ***followed*** by ***another*** attribute, there ***must*** be `whitespace` ***separating*** the two.

+ `Unquoted attribute value syntax`:

> a ***valid*** `unquoted attribute value` in `HTML` is ***any*** string of text that is ***not*** the `empty string` and that ***doesn’t*** contain `spaces`, `tabs`, `line feeds`, `form feeds`, `carriage returns`, <code>"</code>, <code>'</code>, <code>`</code>, <code>=</code>, <code><</code>, or <code>></code>.
> -- <cite>Mathias Byens</cite>

Go to [Unquoted attribute values in HTML and CSS/JS selectors](https://mathiasbynens.be/notes/unquoted-attribute-values) to ***view*** the **original post**.

Mathias [works](https://mathiasbynens.be/) on `Chrome DevTools` and the `V8 JavaScript Engine` at ***Google***.

Example:

```html
<input value=no>
```

+ `Single-quoted attribute value syntax`: ***Valid*** single quotes, and ***not*** apostrophes, are ***permitted*** to use.

Example:

```html
<input value='no'>
```

+ `Double-quoted attribute value syntax`: ***Valid*** double quotes are ***permitted*** to use.

Example:

```html
<input value="no">
```

There is ***usually*** only ***one*** `value` ***attributed*** to the `value` attribute ***per*** element, but if by ***any*** chance there ***had*** to be ***more*** than ***one***, a `whitespace` should be ***placed*** between the ***two*** values.

Example:

```html
<input value="yes no">
```

</section>

---

<section class="section">
    <h2 class="sentence"> The HTML id attribute</h2>

The `id` attribute ***specifies*** a ***unique*** `id` for an `HTML` element. The `value` ***must*** be ***unique*** within the `HTML` document (`web page`). The `id` attribute is ***mostly*** used to ***point*** to a `style` in a `stylesheet`, and by `JavaScript` (***via*** the `HTML DOM`) to ***manipulate*** the **element** with that ***specific*** `id`.

The `id` attribute is a `global` attribute which can be ***used*** in ***any*** `HTML` element.

The `id`'s value ***must not*** contain `whitespace` (`spaces`, `tabs`, etc).

Elements can ***only*** have ONE single `id` value.

```html
<h1 id="main-heading">Maria's Kitchen</h1>
```

</section>

---

<section class="section">
    <h2 class="sentence">The HTML class attribute</h2>

The `class` attribute ***specifies*** one or ***more*** `class` names for an element.

The `class` attribute is ***mostly*** used to ***point*** to a `class` in a `stylesheet`. ***However***, it can ***also*** be ***used*** by `JavaScript` (***via*** the `HTML DOM`) to make ***changes*** to `HTML` ***elements*** with a ***specified*** `class`.

The `class` attribute is a `global` attribute which can be ***used*** in ***any*** `HTML` element.

The `HTML specification` does ***not*** put ***requirements*** on the **naming** of `classes`, but **web developers** and **designers** are ***encouraged*** to use names which ***semantically*** describe the ***purpose*** of the `element` and ***not*** its ***presentation***. ***Semantic*** names are ***still*** understandable when the ***presentation*** of the page ***changes***.

```html
<h1 class="main-heading intro">Maria's Kitchen</h1>
```

</section>

---

<section class="section">
    <h2 class="sentence">What constitutes a simple html web page?</h2>

When I ***create*** an `index.html` **page** with the `touch` ***command*** in **Terminal** `touch index.html` at the ***root*** of my **project folder**, I can go ***into*** that ***page*** inside the `Brackets` ***code editor***, and ***select*** the `HTML Skeleton` ***icon*** located on the ***right*** side of of the `Brackets` ***code editor*** `active window`. A pop-up ***appears*** which ***provides*** me with a ***list*** of ***options***:

```shell
Basic HTML Skeleton
Viewport
External Stylesheet
Inline Stylesheet
External Script
Inline Script
Image
```

In ***order*** to ***generate*** the ***bare minimum*** `html5` ***needed*** to create a ***valid*** `HTML` page, I ***select*** `Basic HTML Skeleton` from the ***pop-up*** under the `Elements` ***heading***, and the ***following*** `HTML` markup is ***generated***:

```html
<!DOCTYPE html>
<html lang="">
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title></title>
</head>

<body>
    
</body>
</html>
```

I ***only*** have to ***make*** a few ***tweaks*** to the `markup`. 

***First***, I ***have*** to ***add*** the ***value*** `"en"` to the `lang` attribute ***inside*** the ***opening*** `html` tag. 

***Next***, I ***change*** the ***lowercase*** `utf` to all ***uppercase*** `UTF` ***inside*** the ***value*** of the `charset` attribute of the ***first*** `meta` element. 

***Third***, I ***have*** to ***add*** content to the `title` element. I call it `My First HTML document`.

</section>

---

<section class="section">
    <h2 class="sentence">Rendering text content to the html page</h2>

***However***, this `markup` ***alone*** does ***not*** render ***anything*** to the `page`. At the very ***least***, I have to add at ***least*** one `text-based` element. I select the `h1` heading element. It ***represents*** the ***primary*** heading of a `page` or `section`.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My First HTML document</title>
</head>
<body>
    <h1>How I created my first html web page</h1>
</body>
</html>
```

</section>

---

<section class="section">
    <h2 class="sentence">Adding a second text-based element</h2>

If I ***wanted*** to get a bit ***fancier***, I ***could*** add a ***text-based*** `p` element to describe ***how*** I actually ***created*** the `page`.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <h1>How I created my first html web page</h1>
    <p></p>
</body>
</html>
```

I am ***leaving*** the `p` element ***empty***, and will leave ***you*** to ***add*** the ***text*** describing ***how*** you came to create ***your*** `HTML` page.

I am ***also*** leaving it to you to ***customize*** the ***content*** of the `title` tag.

</section>

---

<section class="section">
    <h2 class="sentence">!DOCTYPE: what it means</h2>

`<!DOCTYPE>` is required in ***all*** `HTML` documents.

***All*** `HTML` documents ***must*** begin with a `<!DOCTYPE>` ***declaration***. The ***declaration*** is ***not*** an `HTML` tag. It ***provides*** information to the `browser` about what `document type` to ***expect***. In ***our*** case, we are ***informing*** the `browser` that our `document` is an `HTML` ***document***.

```html
<!DOCTYPE html>
```

We can ***tell*** that this is an `HTML5` ***declaration*** because ***older*** declarations, `HTML 4.01`, for ***example,*** looked ***something*** like ***this***:

```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
```

The `<!DOCTYPE html>` declaration is ***not*** case sensitive. But ***convention*** is the ***following***:

```html
<!DOCTYPE html>
```

</section>

---

<section class="section">
    <h2 class="sentence">The html element: its purpose and meaning</h2>

The `html` element ***represents*** the `root`, or `top-level` element, of an `HTML` document. It is ***also*** referred to as the `root` element. ***All*** other elements on the `page` ***must*** be ***descendants*** of the `html` element.

In our ***basic*** `web page`, `Brackets` ***generated*** the ***global*** `lang` attribute ***inside*** the ***opening*** `html` ***tag*** with a `value` of `""` and I added the `en` inside the double quotes. That's ***because*** where we are ***located***, English is the ***dominant*** language.

```html
<html lang="en">
```

</section>

---

<section class="section">
    <h2 class="sentence">The head element: its purpose and meaning</h2>

The ***purpose*** of the `HTML` `head` element is to contain ***machine-readable*** information (`metadata`) about the `document`. Like its `meta` tag(s), `title`, `scripts`, and `style sheets`.

The `head` element ***primarily*** holds information for ***machine processing***, ***not*** human readability. That is ***why*** things like the ***content*** of the `title` element ***don't*** render to the `web page`.

The `name` of the `head` element is ***semantic***. It is the ***first*** element ***wrapped*** inside the `html` element, the element which ***holds*** valuable ***metadata*** about the `page` ***content***, and it ***sits*** at the `"head"` of of the `document`.

</section>

---

<section class="section">
    <h2 class="sentence">The meta element and the charset attribute: their purpose and meaning</h2>

The ***first*** element ***inside*** our ***basic*** `web page`'s `head` element is a `meta` element with the `charset` attribute. The `charset` attribute is ***one*** of the attributes that the `meta` element ***accepts***.

The `meta` element ***defines*** `metadata` about an `HTML` document. `Metadata` is ***data*** (information) about ***data***.

The `meta` element's `charset` attribute ***specifies*** the `character encoding` for the `HTML` `document`.

The `HTML5 specification` ***encourages*** web developers to ***use*** the `UTF-8` ***character set***, because it ***covers*** almost ***all*** of the `characters` and `symbols` ***available*** ["in the world"](https://www.w3schools.com/tags/att_meta_charset.asp).



</section>

---

<section class="section">
    <h2 class="sentence">What does UTF-8 stand for?</h2>

`UTF-8` ***stands*** for `"Unicode Transformation Format - 8 bits”`.

</section>

---

<section class="section">
    <h2 class="sentence">Binary: How Computers store information</h2>

In ***order*** to be able to ***store*** information, computers ***use*** a `binary system`. In `binary`, ***all*** `data` is ***represented*** in ***sequences*** of `0`s and `1`s. The most ***basic*** `unit` in `binary` is a `bit`, which is just ***either*** a `0` or `1`.

The ***next*** largest `unit` of `binary` is a `byte`, which ***consists*** of `8` `bits`.

An ***example*** of a [byte](https://blog.hubspot.com/website/what-is-utf-8) is

```shell
01101011
```

***According*** to ***Jamie Juliver*** in his post [What is UTF-8 Encoding? A Guide for Non-Programmers](https://blog.hubspot.com/website/what-is-utf-8),

> Every digital asset you’ve ever encountered — from software to mobile apps to websites to Instagram stories — is built on this system of bytes, which are strung together in a way that makes sense to computers. When we refer to file sizes, we’re referencing the number of bytes. For example, a kilobyte is roughly one thousand bytes, and a gigabyte is roughly one billion bytes.

And he **goes on** to ***state***

> Text is one of many assets that computers store and process. Text is made up of individual characters, each of which is represented in computers by a string of bits. These strings are assembled to form digital words, sentences, paragraphs, romance novels, and so on.

</section>

---

<section class="section">
    <h2 class="sentence">So what IS UTF-8 and why should you care?</h2>

If one ***uses*** anything ***other*** than the most ***basic*** English text on a `web page`, users may ***not*** be able to ***read*** the content ***unless*** some sort of `character encoding` is [specified](https://www.w3.org/International/questions/qa-what-is-encoding). ***Not*** specifying some sort of `character encoding` could ***also*** mean that the `data` on the `page` might ***not*** be ***found*** by `search engines`, or ***reliably*** processed by ***machines***.

</section>

---

<section class="section">
    <h2 class="sentence">So what is encoding?</h2>

`Encoding` is the ***process*** of ***converting*** characters in `human languages` into `binary sequences` that computers can ***process***.

</section>

---

<section class="section">
    <h2 class="sentence">What then is Unicode?</h2>

`Unicode` is an `encoding system` that ***solved*** the `space issue` of its ***predecessor*** `ASCII` (`American Standard Code for Information Interchange`, a character encoding standard).

Just as `ASCII` ***before*** it, `Unicode` ***assigns*** a ***unique*** code, called a `code point`, to ***each*** character. ***Unlike*** `ASCII`, `Unicode` is ***able*** to ***produce*** over a ***million*** `code points`, ***more*** than ***enough*** to ***account*** for ***every*** character in ***any*** language.

`Unicode` is now the ***universal*** standard for `encoding` ***all*** human languages. It even ***includes*** emojis.

</section>

---

<section class="section">
    <h2 class="sentence">Why Unicode can't be a standalone</h2>

`Unicode` ***can't*** be a `standalone` when it comes to ***encoding*** characters because it does ***not*** store characters in `binary`. And computers ***need*** a way to ***translate*** `Unicode` into `binary` so that its characters can be ***stored*** in `text files`.
</section>

---

<section class="section">
    <h2 class="sentence">So what IS UTF-8 already?!</h2>

`UTF-8` is the `encoding system` for `Unicode`. It can translate ***any*** `Unicode` character to a ***matching*** unique `binary` string, and it can ***also*** translate the `binary` string ***back*** to a `Unicode` character. This is the ***meaning*** of `UTF`, or `Unicode Transformation Format`.

There are ***other*** `encoding systems` for `Unicode` ***other*** than `UTF-8`, but `UTF-8` is ***unique*** in that it ***represents*** characters in `one-byte` ***units***. One `byte` ***consists*** of `8 bits`, so that is ***why*** `UTF-8`!

</section>

---

<section class="section">
    <h2 class="sentence">The advantages of UTF-8</h2>

There are also ***advantages*** to ***using*** `UTF-8`.

***First***, `UTF-8` is spatially ***efficient***. `UTF-8` ***converts*** a `code point` (which ***represents*** a single character in `Unicode`) into a ***set*** of 1 - 4 `bytes`.

The ***first*** 256 characters in the `Unicode` library, which ***include*** the characters in `ASCII`, are ***represented*** as one `byte`. Characters that appear ***later*** in the `Unicode` library are ***encoded*** as `two-byte`, `three-byte,` and `four-byte` ***binary*** units.

***Why***? To ***save memory***. `UTF-8` uses ***less*** space to ***represent*** more ***common*** characters, and ***more*** space for ***less*** common ones. These characters are ***encoded*** into 2 or ***more*** bytes.

***Second***, `UTF-8` is `backwards compatible` with `ASCII`. The ***first*** 128 characters in the `Unicode` library match ***those*** in the `ASCII` library, and `UTF-8` ***translates*** these 128 `Unicode` characters into the ***same*** `binary` strings as `ASCII`. ***That*** means `UTF-8` is able to ***convert*** a text file ***formatted*** by `ASCII` to ***human-readable*** text ***without*** any problem.

</section>

---

<section class="section">
    <h2 class="sentence">UTF-8 characters in web development</h2>

`UTF-8` is the ***most*** common `character encoding method` ***used*** on the `internet`, and it is ***also*** the ***default*** `character set` for `HTML5`.

And of ***course*** text files ***encoded*** with `UTF-8` ***must*** indicate this to the ***software*** or ***machine*** processing it. ***Otherwise***, it ***won't*** translate the `binary` ***back*** into characters ***properly***. That's where our `meta` element's `charset` attribute ***comes*** in (again)!

```html
<meta charset="UTF-8">
```

</section>

---

<section class="section">
  <h2 class="sentence">The viewport and how it relates to the meta element</h2>

The `viewport` is the user's ***visible*** area of the `web page`. The `viewport` ***varies*** with ***different*** devices, and will be ***smaller*** on a `mobile phone` than on a `computer screen`.

***Before*** `tablets` and `mobile phones` came along, `web pages` were ***only*** designed for `computer screens`, and `web page` ***layouts*** were ***static*** (only had ***one*** size).

When `mobile phones` and `tablets` were ***introduced***, `static sites` were ***too*** large to ***fit*** the `viewport` of the `mobile phone` or `tablet`, for ***example***. To ***fix*** this, `browsers` on ***those*** devices ***scaled down*** the ***entire*** `web page` to ***fit*** the screen. This was ***not*** a ***perfect*** solution, only a ***quick fix***.

`HTML5` ***introduced*** a ***method*** to let `web designers` ***take control*** over the `viewport` ***through*** the `meta` element.

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

***This*** `meta viewport tag` should be ***added*** to the `head` of the `HTML` document. It ***gives*** the `browsers` ***instructions*** on ***how*** to control the page's ***dimensions*** and ***scaling***.

The `width=device-width` ***part*** sets the `width` of the ***page*** to ***follow*** the `screen width` of the ***device*** (which will ***vary*** depending on the ***device***).

The `initial-scale=1.0` ***part*** sets the ***initial*** `zoom level` when the ***page*** is ***first*** loaded by the `browser`.

<aside class="note">
    Note: Go into [Responsive Web Design - The Viewport](https://www.w3schools.com/css/css_rwd_viewport.asp) and show the students the examples of pages without viewports and click on the links in my iphone.
</aside>

</section>

---

<section class="section">
  <h2 class="sentence">Sizing content to the viewport</h2>

Users are ***used*** to ***scrolling*** `web pages` ***vertically***, but (***typically***) not ***horizontally***. In ***most*** cases, If the user is ***forced*** to scroll ***horizontally***, or ***zoom out*** to see the ***whole*** `web page`, it ***results*** in a ***poor*** `user experience`.

***Other*** rules to ***follow***:

+ Do ***not*** use ***large***, `fixed-width` elements. if an ***image*** is ***displayed*** at a `width` ***wider*** than the `viewport`, it can ***cause*** the `viewport` to scroll ***horizontally***. ***Adjust*** the ***content*** to ***fit*** within the `width` of the `viewport`.

+ Do ***not*** let the content ***rely*** on a ***particular*** `viewport` ***width*** to ***render*** well. Since `screen dimensions` and `width` in `CSS` pixels vary ***widely*** between ***devices***, ***content*** should ***not*** rely on a ***particular*** `viewport` ***width*** to ***render*** well.

+ ***Use*** `CSS` ***media queries*** to ***apply*** different ***styling*** for ***small*** and ***large*** screens. Setting ***large*** `absolute CSS` ***widths*** for `elements` on the ***page*** will ***cause*** the `element` to be ***too*** wide for the `viewport` on a ***smaller*** device. ***Instead***, consider using ***relative*** `width` ***values***, such as `width: 100%`. ***Also***, be ***careful*** of using ***large*** `absolute positioning` ***values***. It may ***cause*** the `element` to fall ***outside*** the `viewport` on ***small*** devices.

</section>

---

<section class="section">
    <h2 class="sentence">The purpose and meaning of the title element</h2>

***Below*** the `meta` element is a `title` element. It ***defines*** the `document`'s `title` that is ***shown*** in the ***browser's*** `title bar` or a ***page's*** `tab`. It ***only*** contains `text`, and `tags` placed ***within*** the `element` are ***ignored***.

the `title` element is ***required*** in `HTML` documents, and the ***contents*** of a page `title` is ***very*** important for `search engine optimization` (`SEO`).

The page `title` is ***used*** by `search engine` algorithms to ***decide*** its ***order*** in `search` when ***listing*** pages in `search` results.

</section>

---

<section class="section">
    <h2 class="sentence">The purpose and meaning of the body element</h2>

The element which ***follows*** the `head` element on the web page is the `body` element.

The `body` element ***represents*** the ***content*** of an `HTML` document. It is ***semantic***, because a `body` always comes after a `head`, and the term `body` does ***not*** only mean `organized physical substance of an animal or plant`, for ***example***. It ***also*** means the `main structure or part of something inanimate`. The `name` ***provides*** a ***good*** description of what it ***represents*** in the `HTML` document.

</section>

---

<section class="section">
    <h2 class="sentence">The h1 element</h2>

At the ***top*** of the `body` element, right ***below*** the ***opening*** `body` tag, our basic web page ***contains*** an `h1` element. 

The `h1` element is ***used*** to ***indicate*** the ***most*** important (or ***highest-level***) `heading` on the `page`.

The `h1` element's ***contents*** should ***describe*** the overall ***purpose*** of the `page` content. ***If*** the ***content*** of the `h1` element ***does*** successfully ***describe*** the ***overall*** purpose of the `page` content, it will ***improve*** the `SEO` of the `web page`, thereby ***improving*** its ***ranking*** in `search results`. 

It is ***best*** practice to ***avoid*** skipping `heading` levels.

Traditionally, it is ***also*** best practice to ***only*** use one `h1` element ***per*** page. Using ***more*** than one does ***not*** result in an ***error***, but it is ***not*** considered ***best*** practice. To only have ***one*** is ***better*** for `screen readers` and `SEO`.

</section>

---

<section class="section">
    <h2 class="sentence">The p element</h2>

***Also*** textually ***semantic***, the `p` element ***represents*** a paragraph of ***text***.

`Heading` elements (i.e., `h1` element) are ***often*** followed by ***supporting*** `p` elements.

Paragraphs are ***usually*** represented as ***blocks*** of text ***separated*** from ***adjacent*** blocks by ***blank*** lines and/or ***first-line*** indentation, but they can be ***any*** structural grouping of ***related*** content, such as `images` or `form` fields.

</section>

---

<section class="section">
    <h2 class="sentence">Global HTML Attributes</h2>

The ***following*** is the ***latest*** list of `Global HTML Attributes` as ***per*** the **Web Hypertext Application Technology Working Group's** `HTML specification` in their `HTML Living Standard docs`:

+ accesskey
+ autocomplete
+ autofocus
+ class
+ contenteditable
+ data-* - (***custom*** `data` attributes i.e., `data-foldername`, `datamagid`) can be ***specified*** on ***any*** `HTML element` to ***store*** custom data, state, annotations, and ***other*** similar, ***specific*** to the `page`
+ dir
+ draggable
+ enterkeyhint
+ hidden
+ id
+ inputmode
+ is
+ itemid
+ itemprop
+ itemref
+ itemscope
+ itemtype
+ lang
+ nonce
+ slot
+ spellcheck
+ style
+ tabindex
+ title: ***discouraged***, as ***many*** user agents (browsers) do ***not*** expose the `attribute` in an ***accessible*** manner as ***required*** by the `HTML specification` (e.g., ***requiring*** a `pointing device` such as a `mouse` to ***cause*** a `tooltip` to ***appear***, which ***excludes*** `keyboard-only` ***users*** and `touch-only` ***users***, such as ***anyone*** with a ***modern*** phone or tablet)
+ translate

</section>

---

<section class="section">
  <h2 class="sentence">What does it mean to be a global attribute?</h2>

A `global` attribute is one that is ***common*** to ***all*** `HTML` elements. They can be ***used*** on ***all*** elements, even ***though*** they may have ***no*** effect on ***some*** elements.

</section>

---

<section class="section">
    <h2 class="sentence">Global HTML Event Handler Attributes</h2>

The ***following*** is the ***latest*** list of `Global HTML Event Handler Attributes` as ***per*** the **Web Hypertext Application Technology Working Group's** `HTML specification` in their `HTML Living Standard docs`:

+ onabort
+ onauxclick
+ onblur*
+ oncance*l
+ oncanplay
+ oncanplaythrough
+ onchange
+ onclick
+ onclose
+ oncontextmenu
+ oncopy
+ oncuechange
+ oncut
+ ondblclick
+ ondrag
+ ondragend
+ ondragenter
+ ondragleave
+ ondragover
+ ondragstart
+ ondrop
+ ondurationchange
+ onemptied
+ onended
+ onerror*
+ onfocus*
+ onformdata
+ oninput
+ oninvalid
+ onkeydown
+ onkeypress
+ onkeyup
+ onload*
+ onloadeddata
+ onloadstart
+ onmousedown
+ onmousenter
+ onmouseleave
+ onmousemove
+ onmouseout
+ onmouseover
+ onmouseup
+ onpaste
+ onpause
+ onplay
+ onplaying
+ onprogress
+ onratechange
+ onreset
+ onresize*
+ onscroll*
+ onsecuritypolicyviolation
+ onseeked
+ onseeking
+ onselect
+ onslotchange
+ onstalled
+ onsubmit
+ onsuspend
+ ontimeupdate
+ ontoggle
+ onvolumechange
+ onwaiting
+ onwheel

`Note`: The attributes ***marked*** with an `*` (asterisk) have a ***different*** meaning when ***specified*** on the `body` element ***vs*** when elements ***expose*** `event handlers` of the `Window object` with the ***same*** (attribute) names. And ***even though*** these attributes ***apply*** (globally) to ***all*** elements, they are ***not*** useful on ***all*** elements. For ***example***, only `media` elements will ***ever*** receive a `volumechange` event ***fired*** by the **user agent**.

</section>

---

<section class="section">
    <h2 class="sentence">Related Resources</h2>

+ [CodeSandbox](https://codesandbox.io/)

+ [HTML: Wikipedia](https://en.wikipedia.org/wiki/HTML)

+ [Web Design Museum](https://www.webdesignmuseum.org/web-design-history)

+ [2 - A history of HTML: Addison Wesley Longman](https://www.w3.org/People/Raggett/book4/ch02.html)

+ [Learn To Code HTML & CSS: Shay Howe](https://learn.shayhowe.com/)

+ [HTML Elements](https://www.tutorialrepublic.com/html-tutorial/html-elements.php)

+ [Scripting Master](http://www.scriptingmaster.com/html/HTML-terms-glossary.asp)

+ [TutorialReplublic](https://www.tutorialrepublic.com/html-tutorial/)

+ [HTML Living Standard — Last Updated 22 January 2021](https://html.spec.whatwg.org/multipage/introduction.html)

+ [HTML Living Standard — Last Updated 22 January 2021](https://html.spec.whatwg.org/)

+ [What is the difference between phrasing content and flow content?: stackoverflow](https://stackoverflow.com/questions/30233447/what-is-the-difference-between-phrasing-content-and-flow-content)

+ [HTML Content Categories: MDN](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Content_categories)

+ [HTML Tutorial: w3schools](https://www.w3schools.com/html/)

+ [HTML <!DOCTYPE> Declaration: w3schools](https://www.w3schools.com/tags/tag_doctype.asp)

+ [html: The HTML Document / Root element: MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/html)

+ [HTML meta charset Attribute: w3schools](https://www.w3schools.com/tags/att_meta_charset.asp)

+ [Character encodings for beginners: w3.org](https://www.w3.org/International/questions/qa-what-is-encoding)

+ [What is UTF-8 Encoding? A Guide for Non-Programmers: Jamie Juviler](https://blog.hubspot.com/website/what-is-utf-8)

+ [title: The Document Title element: MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/title)

+ [How to Create the Perfect H1 Tag for SEO: Neil Patel](https://neilpatel.com/blog/h1-tag/)

+ [4.3.11.1 Creating an Outline: WHATWG](https://html.spec.whatwg.org/multipage/sections.html#outlines)

+ [HTML class Attribute: w3schools](https://www.w3schools.com/tags/att_class.asp)

+ [class attribute: MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/class)

+ [Responsive Web Design - The Viewport: w3schools](https://www.w3schools.com/css/css_rwd_viewport.asp)

+ [Normal Flow](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Normal_Flow)

</section>
