# Functional Reactive Programming Demo

[Correspond Blog](http://cjting.me/web2.0/intruduction-to-functional-reactive-programming/).

this repo is based on the fantistic [bacon.js registration tutorial](https://baconjs.github.io/tutorials.html) but using RxJS.

Now, think about a registration form, it's the most common thing on the web, normally it's like this:

![](http://ww4.sinaimg.cn/large/9b85365djw1f23hsxwdsaj20tl07iwel.jpg)

But is's not that simple. Consider the following things we need to do:

- Username availability checking while the user is still typing the username
- Throttle the ajax request
- Showing feedback on availability result
- Showing an AJAX indicator while this check is being performed
- Disabling the Register button until both username and fullname have been entered
- Disabling the Register button in case the username is unavailable
- Disabling the Register button while the check is being performed
- Disabling the Register button immediately when pressed to prevent double-submit

Actually, it's pretty hard to make a robust and top notch form, even it's so simple like before.

In this repo, I am gonna use jquery and RxJS to implement these features, so we can clearly see the benefits of functional reactive programming.

## Run the demo

```bash
cd frp-demo
npm install 
npm run dev # now go to localhost:8000/
git checkout jquery # get the implementation using jquery
git checkout rxjs # get the implementation using RxJS
```
