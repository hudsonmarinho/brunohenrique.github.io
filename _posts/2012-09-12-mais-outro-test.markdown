---
layout: post
title: Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit...
categories: recursos priorização pt
---

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla eleifend diam ut libero semper faucibus vel nec dui. Duis sapien erat, varius sit amet fringilla sit amet, sagittis a lorem. Aliquam sit amet sem quam, a egestas urna. Phasellus ac dui odio, at adipiscing ligula. Cras et felis ac dui lobortis ullamcorper. Sed euismod dolor id urna ultrices auctor. Etiam quis justo at justo malesuada aliquam ac at urna. Morbi cursus dapibus risus ac dictum. Suspendisse semper eleifend leo, eget suscipit risus tempus ac. Cras vel tellus sit amet magna accumsan dictum a id risus. In purus turpis, ultrices vitae iaculis ut, ullamcorper vitae nibh. Morbi tortor arcu, tincidunt vel condimentum eu, dapibus sed urna. Vestibulum commodo felis eget sapien feugiat porttitor. Aliquam erat volutpat.
<!-- more start -->
Vivamus lorem ipsum, mollis quis varius at, laoreet vitae tortor. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Nulla vitae orci id tortor vehicula mollis viverra ullamcorper justo. Aenean dolor magna, mattis ac posuere nec, adipiscing nec quam. Aliquam mi leo, porta ut cursus ac, porttitor bibendum nunc. Duis ornare justo non mauris vulputate hendrerit iaculis ante tempor. Etiam sed mi sit amet elit pellentesque pretium eget vitae velit. Maecenas a ante lectus, placerat pretium neque. Praesent adipiscing elit at turpis lobortis sed posuere dui convallis. Morbi velit dui, placerat vitae scelerisque porta, pulvinar eget turpis.

{% highlight ruby linenos %}
require 'sinatra'
require 'nokogiri'
require 'open-uri'
require 'json'

post '/search' do
    url_search = params[:urlSearch]
    page = Nokogiri::HTML(open(url_search))
    crawler_return = []
    page.xpath('//img').each do |node|
        crawler_return << node.to_html
    end
    crawler_return.to_json
end

{% endhighlight %}
Nullam non augue quam. Morbi lacinia, metus et posuere tristique, metus nulla dignissim leo, a rhoncus quam augue et nisi. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Fusce metus dui, rutrum ut commodo in, fringilla id purus. Nunc sed mauris enim. Aliquam id turpis magna, et blandit justo. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed turpis risus, malesuada nec tincidunt nec, lobortis sed eros.

Nulla quis velit eu leo aliquet facilisis sed non massa. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas placerat erat in neque congue aliquet. Nunc sem risus, iaculis tempor iaculis commodo, consectetur a nisl. Pellentesque eget sodales ipsum. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Donec quam nunc, scelerisque eget rhoncus vitae, ultricies nec tellus. Duis adipiscing dapibus sem, in tristique enim euismod in.

Donec cursus erat porttitor odio aliquam ultrices elementum mi fringilla. Pellentesque blandit tincidunt neque a vestibulum. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque blandit auctor pretium. Morbi fringilla vestibulum velit ut adipiscing. Suspendisse potenti. Maecenas ante libero, scelerisque eu imperdiet sit amet, egestas in nunc. Nunc consequat fermentum vehicula. Morbi id metus felis, quis pulvinar mauris.

<!-- more end -->
