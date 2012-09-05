# HTML IPython Notebook Server for dotCloud


# Howto

Get a [dotCloud](www.dotcloud.com) account and dowload the cli dotcloud

    git clone git://github.com/shoibalc/ipynbserver-dotcloud.git

Follow http://ipython.org/ipython-doc/dev/interactive/htmlnotebook.html#security in your local IPython to generate
a hashed passwd in /nbserver/postinstall in the line.

    c.NotebookApp.password = u'sha1:bcd259ccf...your hashed password here'
    git add -A && git commit -m "Done"
    
Create and push the repository
    
    dotcloud create ipynbserver
    dotcloud push ipynbserver ipynbserver-dotcloud


Enjoy!
