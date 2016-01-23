### Scrapy
+ install :`pip install Scrapy`
+ `Detected a distutils installed project ('six') which we cannot uninstall. The metadata provided by distutils does not contain a list of files which have been installed, so pip does not know which files to uninstall.`
<br/>  resolve :`pip install Scrapy --upgrade --ignore-installed six`
+ `ImportError: cannot import name xmlrpc_client`
<br/>  resolve :
`sudo rm -rf /Library/Python/2.7/site-packages/six*`
`sudo rm -rf /System/Library/Frameworks/Python.framework/Versions/2.7/Extras/lib/python/six*`
`sudo pip install six`

+ Creating a project
`scrapy startproject tutorial`

<http://doc.scrapy.org/en/1.0/intro/tutorial.html>

<pre>
tutorial/
    scrapy.cfg            # deploy configuration file

    tutorial/             # project's Python module, you'll import your code from here
        __init__.py

        items.py          # project items file

        pipelines.py      # project pipelines file

        settings.py       # project settings file

        spiders/          # a directory where you'll later put your spiders
            __init__.py
</pre>

+ To put our spider to work, go to the project’s top level directory and run: `scrapy crawl dmoz`


### PyCharm
1. open project
2. preferences -> interpreter -> 2.7.6


