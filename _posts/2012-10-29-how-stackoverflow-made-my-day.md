---
layout: post
category : stackoverflow
tags : [stackoverflow, help, rails]
---
{% include JB/setup %}

This situation happened to me while I was going back from work!

### Stackoverflow answer

It was a normal question, regarding how to parse a JSON with JQuery. It was a JSON returned from a a rails controller action. To be honest, the answer was very simple and the users who made the question needed was a second look on his code, it ususally happens when we are stresses or under pressure and too much time in the same defect.

Basically my answer was a code similar to this:

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

It was not that special, so how would this made my day?

### E-mail

I was arriving home, back from work when I get my smartphone and read an e-mail with the subject **"json answer"**.

When I openen the e-mail, a surprise:

    You made my day.
    I will not be dismissed tomorrow =)
    Thanks.

Well, reading this e-mail made my effort on stackoverflow worth. Since I begin answering programmers questions in stackoverflow to retribute thousands of questions I found the answer immediatly in this awesome community, this was by far the gratest reward I ever received.

### It happened with you

So I'm sure it happened with you if you contribute on similar sites or even stackoverflow. I'm saying that because most of the times this happens you won't receive the e-mail because people feel shy of doing this. Anyways, you can be sure that you are helping hundres to thousants of people from similar situations.

I feel lucky to read this e-mail and it made my day. That is why I decided to make my first post on this blog about what happened.

**Regards, Felipe Lopes!**

Please take a look at [{{ site.categories.api.first.title }}]({{ BASE_PATH }}{{ site.categories.api.first.url }}) 
or jump right into [Usage]({{ BASE_PATH }}{{ site.categories.usage.first.url }}) if you'd like.