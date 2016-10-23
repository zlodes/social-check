# social-check
JavaScript & JQuery tool for checking auth on popular social services

## Installation
```
bower install https://github.com/zlodes/social-check
```

## Usage
###jQuery
```
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/2.2.4/jquery.min.js"></script>
<script src="bower-components/social-check/jquery.socials-chech.min.js"></script>
<script>
jQuery(function($){
    $.socialCheck(['VK', 'Facebook', 'Twitter']).then(function(res) {
        console.log(res); // res like {'VK': true, 'Facebook': false, 'Twitter': true}
    });
});
</script>
```
### ES6 module
```
import socialCheck from 'bower-components/social-check'

socialCkeck(['VK', 'Facebook', 'Twitter']).then(res => {
    console.log(res); // res like {'VK': true, 'Facebook': false, 'Twitter': true}
});
```
