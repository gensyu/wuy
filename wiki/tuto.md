## Create an App/Window

Create a python file "web.py", and copy/paste this:

```python
import wuy

class index(wuy.Window)
    pass

index()
```
Run it, like this :

    $ python3 web.py

It will create a "web/index.html", the defaut front-end ;-)

Edit "web/index.html", like this :

```html
<script src="wuy.js"></script>
<button onclick="wuy.myadd(42,13).then( alert )">test</button>
```

Edit "web.py", like this :

```python
import wuy

class index(wuy.Window)
    size=(640,480)
    def myadd(self, a,b):
        return a+b

index()
```

and rerun your script :

    $ python3 web.py

and you can start to code

**TIP** : if you want the server mode (aka : use many clients from anywhere) ; just replace _wuy.Window_ by _wuy.Server_ !