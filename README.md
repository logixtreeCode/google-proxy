# Python Proxy Script

[![Contact Us](http://logixtree.in/contact-us.svg)](http://logixtree.in)

Simple proxy scirpt for setting up the personnel proxy server on the Google App Engine.(Adjusted with the new google app engine changes)

## To Do List : 
	* POST requests are not be handling properly
	* URI handling is not being working properly 

## Instructions : 
1. Create project in google app engine dashboard 
2. Setup the git reponsitories and sync the source code 
3. In the console, Run the following :

```bash 
$ gcloud config set project logixtree-proxy \
  			&& gcloud source repos clone default \
    			~/src/logixtree-proxy/python_gae_quickstart  \
  			&& cd ~/src/logixtree-proxy/python_gae_quickstart \
  			&& git checkout gcloud
```

4. Change the above 'logixtree-proxy' with your application Unique ID
5. Run the app with preview window. Here you can test your application before deploying 

```bash		
$ dev_appserver.py $PWD
```

6. After setting all deploy it to the cloud

```bash 
$ gcloud app deploy app.yaml
```

## Issues 
+ POST requests are not being handling properly
+ URI handling is not being working properly 

## Usage

After deployment, If there is no error in console. you can happily access the changes in 

[logixtree-proxy.appspot.com](http://logixtree-proxy.appspot.com/)



## Concerns

If you have concerns or issues, please email us info@logixtree.in or can use the issue tracker.

## References

- [Labnol](http://twitter.com/labnol)
- [Tutorial](http://www.labnol.org/internet/setup-proxy-server/12890/)
- [Video Instructions](https://www.youtube.com/watch?v=3f6Zq4prys0)
- [All Contributors](../../contributors)
