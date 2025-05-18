03-05-2025


Promises are used in handling asynchronous operations.
What are asynchronous operations? Essentially - Blocks of code that don't block the main thread and rather run "in the background". So things like subscribing to push notifications, getting a response from the server etc. don't block the user interface.
An example flow of promises:
```javascript
navigator.serviceWorker.register(...)
  .then(function(registration) { ... })
  .then(function(subscription) { ... })
  .catch(function(error) { ... });
```
Each promise in this flow waits for the previous one, but the whole flow runs in the background.
### Hashtags:
#webdev #coding #javascript #async 


### References (source material, similar notes):
