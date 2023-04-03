English | [Chinese](./README.md)

<p>
<strong><h2>LiCheng - Home</h2></strong>
It's hard to hold on; But cool
</p>

![李程主页](https://www.lcclc.cn/cc/Sitescreenshot.webp)

>The logo font on the home page has been compressed, so if you use a font other than this logo, it will change back to the default font

### Demo
>Due to CDN caching, you may need `Ctrl` + `F5` to force a browser cache refresh to see the latest results

- [李程 - 今天也要加油吖~](https://www.lcclc.cn/)

### Functions

- [x] Loading animation
- [x] Site description
- [x] Hitokoto
- [x] Date and time
- [x] Live weather
- [x] Time progress bar
- [x] Music player
- [x] Mobile adaptation

* [ ] Remove jQuery dependency
* [ ] VUE refactoring

### Weather

Because the original weather API is unstable, the weather API has been replaced. Now you need to go to the following website to obtain the key  

- to [ROLL] (https://www.mxnzp.com/doc/list) for app_id and app_secret, used to capture the city  

- to [and wind weather] (https://dev.qweather.com/) to obtain the key, is used to get the weather information  

It can also be replaced by other methods

### Music

>This project uses the `Aplayer` music player based on `MetingJS` for quick song list customization  
>*Only supported in **Mainland China**, please replace `music.js` with [the following](https://file.imsyy.top/js/music/music-other.js) in other regions to enable the music player to work properly

Change the parameters of `music.js` to achieve a custom song list

```js
let server = "netease"; //netease; tencent; kugou; xiami; kuwo; 
let type = "playlist"; //song; playlist; album;
let id = "7452421335"; //album ID; song ID; playlist ID;
```

### Fonts
>As Chinese fonts are introduced in this project, Chinese fonts need to be compressed to improve the loading speed of the page (you can also cancel the use of Chinese fonts)

#### Chinese font removal traditional

- Install `Python 3.7` and `pip`
- Run `pip install fonttools`
- Download [sc_unicode.txt](https://gist.githubusercontent.com/imaegoo/d64e5088b723c2e02c40985f55ff12db/raw/5ebd2ce49418c73459a9dfe050483409306a6c1d/sc_unicode.txt)
- Run `pyftsubset font-name.ttf --unicodes-file=sc_unicode.txt`

#### fonts further compressed

- Compile and install ``Google woff2``

```bash
sudo apt-get install -y git g++ make
git clone --recursive https://github.com/google/woff2.git
cd woff2
make clean all
```

- Compress the font again

```
. /woff2_compress . /font_name.ttf
```

- Eventually the original font can be slow loaded, **load the compressed font first**

>For more information, please go to [虹墨空间站](https://www.imaegoo.com/2020/chinese-font-compress/) to view the original article

### Plugins

* [Bootstrap](https://getbootstrap.com/)
* [iziToast](https://izitoast.marcelodolza.com/)
* [Font Awesome](https://fontawesome.com/)
* [jQuery](https://jquery.com/)
* [Aplayer](https://aplayer.js.org/)

<a title="SSL" target="_blank" href="https://myssl.com/www.lcclc.cn?domain=www.lcclc.cn&status=success"><img src="https://img.shields.io/badge/MySSL-安全认证-brightgreen"></a>&nbsp;<a title="CDN" target="_blank" href="https://cdnjs.com/"><img src="https://img.shields.io/badge/CDN-Cloudflare-blue"></a>&nbsp;<a title="Copyright" target="_blank" href="https://www.lcclc.cn/"><img src="https://img.shields.io/badge/Copyright%20%C2%A9%202023-%E6%9D%8E%E7%A8%8B-orange"></a>
