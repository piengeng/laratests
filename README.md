# Manual setup
basic requirements:
- php installed *did not verify the minimum version required.
- ```git clone https://github.com/dericofilho/php.tools``` to basePath 
- ```git clone https://github.com/piengeng/laratests``` to basePath 
*basePath = any working path*

Step 1) folders structure
```
basePath/php.tools/**/*
basePath/laratests/**/*
```
Step 2) copy ```basePath/laratests/laratests.php``` to ```basePath/php.tools/src/laratests.php```

Step 3) download and process *.php styling reference
```
cd laratests/; 
php automate_fetch_github_remove_non_php.php;
```

Step 4) generate the freaking batch processing.
```
cd php.tools/src; 
php laratests.php; # modify if needed
```

Step 5) visual diff (I'm using KDiff3, it will show a quick summary of diff on folder). Continue working on php.fmt
```
cd laratests/; # visual diff from here
```
*'m too lazy to create any script file for this. use at your own risk.*