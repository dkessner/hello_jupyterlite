# Hello JupyterLite 

## [Live site](https://dkessner.github.io/hello_jupyterlite/)


## Notes

nickmcintyre/ipycc package for turtle graphics in Jupyter:    
[https://github.com/nickmcintyre/ipycc](https://github.com/nickmcintyre/ipycc)

Install stuff in Jupyter via pip:  
```python
%pip install -q ipycanvas
%pip install -q ipycc
import ipycanvas
import ipycc
```

Example from nickmcintyre:  
```python
from ipycc import Turtle

t = Turtle()
t.draw()
t.bgcolor('midnightblue')
t.pencolor('ghostwhite')
t.pendown()
side = 5
while side < t.width:
    t.forward(side)
    t.left(90)
    await t.delay(0.1)
    side += 5
```



## Local development

Build (and specify content directory)
```console
jupyter lite build --contents content
```

Serve locally
```console
jupyter lite serve
```

## Reference

[JupyterLite Demo template](https://github.com/jupyterlite/demo)


