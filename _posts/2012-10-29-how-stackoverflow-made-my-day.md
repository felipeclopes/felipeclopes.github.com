---
layout: post
category : stackoverflow
tags : [stackoverflow, help, rails]
---
{% include JB/setup %}

This situation happened to me while I was going back from work!

### Stackoverflow answer

It was a normal question, regarding how to parse a JSON that was sent by a rails controller action with JQuery. To be honest the answer was very simple and what the users who asked for it just wanted a second look on his code, like it always happen with many of us.

Basically I answered with a code similar to this:

{% highlight ruby %}

    #In controller set JSON as following:
    format.json{ render json: {errors: @upload.errors.full_messages}, :status =>422}

{% endhighlight %}

{% highlight javascript %}

    //Then with JQuery you can handle like this:
    $('#fileupload').fileupload({
        [...]
        error: function(xhr){
          var errors = $.parseJSON(xhr.responseText).errors
          alert(errors)         
        }
    });
{% endhighlight %}

So it was not that special and how would this made my day?

### E-mail

SO going back whether I was, telling that I was arriving home back from work when I get my smartphone and read a e-mail wich subject was **json answer**.

When I open the e-mail a surprise:

    You made my day.
    I will not be dismissed tomorrow =)
    Thanks.

Well, reading this e-mail made my effort on stackoverflow worth. Since I begin answering questions of programmer in stackoverflow to retribute thousands of questions I found the answer immediatly in this awsome community, this was by far the gratest reward I ever received.

### It happened with you

So I'm sure it happened with you if you contribute on similar sites or even stackoverflow. I'm saying that because most of the times this happens you won't receive the e-mail because people feel shy of doing this. 

I feel lucky to read this e-mail and it made my day. That is why I decided to make this, my first post on this blog.

**\Thank you**

Please take a look at [{{ site.categories.api.first.title }}]({{ BASE_PATH }}{{ site.categories.api.first.url }}) 
or jump right into [Usage]({{ BASE_PATH }}{{ site.categories.usage.first.url }}) if you'd like.