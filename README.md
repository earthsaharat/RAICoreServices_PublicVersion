# RAICoreServices_PublicVersion

This is the template of Django project of Robotics Laboratory 3 (Smart Lab)

You need to follow this project format before upload your code to the real server

## Installation

1. Download this git
2. Run server

now you can run this project

## File system

<img src="https://github.com/earthsaharat/RAICoreServices_PublicVersion/blob/master/git_supportfile/file_structure_full.png" width="200"/>

### Application/Module
You application/module are stored in 

```
RAICoreServices_PublicVersion/rai_modules/<your_module_name>
```
This folder will contain all of your python file. Such as views.py, urls.py, models.py

> Module name should be leading by `rai_`. For Example, `rai_exampleapp`

### Template

Html file

```
RAICoreServices_PublicVersion/rai_modules/<your_module_name>/template/<your_html_file>.html
```

### Static file

Such as css, javascript, image

```
RAICoreServices_PublicVersion/static/<your_module_name>/<your_static>
```

### Media file

When you have database that contain images. Images will save to the folder media. The image field of model in models.py should set argument like this `image = models.ImageField(upload_to='<your_module_name>/image')`

The image that user uploaded, it saved in

```
RAICoreServices_PublicVersion/media/<your_module_name>/<your_static>
```
