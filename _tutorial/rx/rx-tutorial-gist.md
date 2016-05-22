---
layout: tutorial
order: 100
title: Rx Gist Sample
---

# Gist sampler

U ovom odeljku ćemo govoriti o kreiranju *Rx* operatora. Za analizu
smo izabrali __delay__ operator. 

{% gist 6d434c0538f2dd656560  %}

... vs ...

{% highlight java linenos %}
package rx;

public class Observable<T> {

  // ...
  
  public final Observable<T> delay(long delay, TimeUnit unit) {
    return delay(delay, unit, Schedulers.computation());
  }
  
  // ...
}
{% endhighlight %}




