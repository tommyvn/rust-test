# Pushing to drie push

To push to drie push, first use the below command to generate a random app name
```
app_name=rust-$(curl -s http://m.rang.push.drieapp.co)
echo $app_name
```

And then add drie as a remote and push it
```
git remote add drie ${app_name}.app@push.drieapp.co:code.git
git push drie master
```

Once the build completes you'll be told the url to access the app in your browser.

https://drie.github.io/push-docs/
