# css-version

# Installation

`composer require elminson/css-version`

# After install execute

`composer run post-install-cmd`

This command will install the pre-commit file on .git folder

# How to use it
### in your core html template load the version

```php
<?php
$cssVersion = file_get_contents("css_version");
?>


#implementation in all your css link href
<link href="<?=base_url();?>css/app.css?v=<?=$cssVersion?>" rel="stylesheet">
<link href="<?=base_url();?>css/morestyles.css?v=<?=$cssVersion?>" rel="stylesheet">
...
```

<img src="tests/css_version_test.png">