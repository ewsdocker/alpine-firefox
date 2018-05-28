<h1><u>alpine-firefox</u></h1>  

<h2>The Firefox-esr browser in an Alpine Linux Docker image.<h2>  
<hr>
<h2><u>Quick start</u></h2>

<h3><u>Preload the ewsdocker/alpine-firefox docker image</u><h3>

<ul>

```console
docker pull ewsdocker/alpine-firefox 
```
<hr>
</ul>  
<h3><u>Creating a <i>non-persistent</i> container</u></h3>
<ul>
 <b><u>Video only</u></b>

```console
docker run --rm -it -e DISPLAY --userns=host -v /tmp/.X11-unix/:/tmp/.X11-unix ewsdocker/alpine-firefox
```

 <b><u>Video and Audio</u></b>

```console
docker run --rm -it -e DISPLAY --userns=host -v /tmp/.X11-unix/:/tmp/.X11-unix -v /dev/snd:/dev/snd --privileged ewsdocker/alpine-firefox
```

<hr>
</ul>  
<h3><u>Creating a <i>persistent</i> container</u></h3>

<ul>
 <b><u>Video only</u></b>

```console
docker run -it -e DISPLAY --userns=host -v /tmp/.X11-unix/:/tmp/.X11-unix ewsdocker/alpine-firefox
```

 <b><u>Video and Audio</u></b>

```console
docker run -it -e DISPLAY --userns=host -v /tmp/.X11-unix/:/tmp/.X11-unix -v /dev/snd:/dev/snd --privileged ewsdocker/alpine-firefox
```

</ul>  

____  


Original software by [Ivan Davidkov ](https://github.com/ivan-davidkov/sbff).

