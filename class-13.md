## Local Storage

[Home](README.md)
> before using local storage you should  check if the browser supports it by either using 

`function supports_html5_storage() {
  try {
    return 'localStorage' in window && window['localStorage'] !== null;
  } catch (e) {
    return false;
  }
}`

> or using a modernizer

`if (Modernizr.localstorage) {
  // window.localStorage is available!
} else {
  // no native support for HTML5 storage :(
  // maybe try dojox.storage or a third-party solution
} `


>html5 storange is base on key value pairs and your stored data  can be accessed via that relation

> you can track changes in local storage with logic such as 

`if (window.addEventListener) {
  window.addEventListener("storage", handle_storage, false);
} else {
  window.attachEvent("onstorage", handle_storage);
};`

## Storageevent object

- key, string (the named key was added removed or modified);
- oldValue, any (the previous value or null if a new item was added)
- newValue, any (the new value,or null if an item was removed)
- url string (the page which called a method that triggered this change)