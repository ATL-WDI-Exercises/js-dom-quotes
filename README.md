# js-dom-quotes
## Set up

1. In exercises or sandbox directory
2. `git clone https://github.com/ATL-WDI-Exercises/js-dom-quotes.git`
3. `cd js-dom-quotes`
4. `open index.html`
5. <kbd>command + option + j</kbd>
6. Select "elements" from top ribbon
7. Click ' >_ ' on right of ribbon to open the console

## Exercise - Selecting DOM elements

1. Using relative selection, select the &lt;p&gt; element containing the second Mark Twain quote

```javascript
document.getElementById('mark-twain-second').children[0];
// or
document.getElementById('mark-twain-second').getElementsByTagName('p')[0];
// or
document.getElementsByTagName('blockquote')[3].children[0];
// <p>​The best way to cheer yourself up is to try to cheer somebody else up.​</p>​
```

2. Do the same using a query selector

```javascript
document.getElementById('mark-twain-second').querySelector('p');
// <p>​The best way to cheer yourself up is to try to cheer somebody else up.​</p>​
```

3. Select all of the elements with class .quote

```javascript
document.querySelectorAll('.quote');
document.querySelectorAll('.quote').length;   // 6
```

4. Select the 'Quotes About Motivation' heading

```javascript
document.querySelector('.motivation').getElementsByTagName('h2');
// or even better:
document.querySelector('.subject.motivation h2');
```

5. Select all of the elements with class .subject

```javascript
document.querySelectorAll('.subject');
document.querySelectorAll('.subject').length;   // 3
```

### Bonus
The first section has a class subject. Add a class 'simplicity' from the console

```javascript
document.querySelector('.subject').className += ' simplicity';
```
