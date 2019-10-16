# **Fetch**

## Introduction
The ES6 feature that I will be demonstrating is **fetch**. This function is similar to that of XHR, as it allows you to make network requests. The key difference of these two features is that **fetch** uses *Promises*. A *promise* produces a value in 3 potential states: fufilled, pending, or rejected. Overall, these enable a much simpler API, and also a much cleaner API, which ultimately avoids callback hell.

* [*Fetch*](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)
* [*Promises*](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)
* [*Callback Hell*](https://http://callbackhell.com/)


# **Example**
```
document.getElementById("youranswer").addEventListener('click', getAnswer);

async function getAnswer(){

  const res = await fetch('https://yesno.wtf/api');
  
  const data = await res.json();
  
  answer.innerHTML = (`<img src="${data.image}"/>`);
}
btn.addEventListener('click',getAnswer);
```

![](https://github.com/scagy/lab6-albert/blob/master/img.PNG)
