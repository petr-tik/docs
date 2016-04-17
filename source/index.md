---
title: Mondo API Reference

language_tabs:
  - shell: Curl
  - python: Python
  - go: Golang

includes:
  - authentication
  - pagination
  - object_expansion
  - accounts
  - balance
  - transactions
  - feed_items
  - webhooks
  - attachments
  - errors
  - endpoints

search: false
---

# Introduction



> Examples in this documentation are written using [httpie](https://github.com/jkbrzt/httpie) for clarity.

> To install `httpie` on OS X run 

```
brew install httpie
```

> **API endpoint**

```
https://api.getmondo.co.uk
```
```python
User_ID = "your_user_id"
Account_ID = "your_account_number"
Access_token = "your_access_token"
```
```shell
User_ID="your_user_id"
Account_ID="your_account_number"
Access_token="your_access_token"
```

```go
user_ID := "your_user_id"
account_ID := "your_account_number"
access_token := "your_access_token"
```



> <button class="copy_button" onclick="copyToClipboard()" style="background-color:#4AB8DE;border-radius: 4px;border: none;color:#FFFFFF">Copy</button>
  
The Mondo API is designed to be a predictable and intuitive interface for interacting with users' accounts. We offer both a REST API and webhooks.

Our developers' community in Slack is the place to get help with our API, discuss ideas, and show off what you build. Hit the button to join:

<script>
function copyToClipboard() {
    window.getSelection().removeAllRanges();
    var lang = document.querySelector('.lang-selector .active').getAttribute('data-language-name')
    var highlight_code = '.highlight.' + lang
    var code = document.querySelector(highlight_code).children[0]
    
    // Select the email link anchor text  
    var range = document.createRange();  
    range.selectNode(code);  
    window.getSelection().addRange(range);  

    try {  
      // Now that we've selected the anchor text, execute the copy command  
      var successful = document.execCommand('copy');  
      var msg = successful ? 'successful' : 'unsuccessful';  
      console.log('Copy email command was ' + msg);
    } catch(err) {  
      console.log('Oops, unable to copy');  
    }  

    // Remove the selections - NOTE: Should use
    // removeRange(range) when it is supported  
    window.getSelection().removeAllRanges(); 
}
</script>


<script type="text/javascript" src="/app/_copy_clipboard.js"></script>

<script async defer src="https://devslack.getmondo.co.uk/slackin.js"></script>

<aside class="warning">
The Mondo API is under active development. Breaking changes should be expected.
</aside>
