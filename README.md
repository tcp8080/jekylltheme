This is the demo from https://jekyllrb.com/docs/step-by-step/01-setup/

It provided the easiest jekyll blog with no theme used


Q&A:
1. Env
make sure ruby installed and in path
```
source /opt/EE_LinSEE/bin/seesetenv ruby=2.7.1
```

2. after https://jekyllrb.com/docs/step-by-step/01-setup/
> -bash: jekyll: command not found
```
gem env //get gempath like /opt/ruby/x86_64/2.7.1-1/lib/ruby/gems/2.7.0/
        //then you cant get jekyll bin folder
        //like /opt/ruby/x86_64/2.7.1-1/lib/ruby/gems/2.7.0/gems/jekyll-4.1.1/exe
cd /usr/bin 
ln -s /opt/ruby/x86_64/2.7.1-1/lib/ruby/gems/2.7.0/gems/jekyll-4.1.1/exe/jekyll jekyll
```

3. run
```
bundle exec jekyll serve -w --host=0.0.0.0
```
then you can input http://jekyllserverIp:4000 on all the browsers in the same wlan
